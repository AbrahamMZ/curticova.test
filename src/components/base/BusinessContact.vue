<template>
  <v-theme-provider :dark="dark">
    <div>
      <base-info-card
        :title="title"
        color="primary"
      >
        <slot />
      </base-info-card>

      <template v-for="({ icon, text, title: t }, i) in business">
        <base-avatar-card
          :key="i"
          :icon="icon"
          :outlined="false"
          :title="!dense ? t : undefined"
          color="transparent"
          horizontal
          space="0"
        >
          <div v-html="text" />
        </base-avatar-card>

        <v-divider
          v-if="i + 1 !== business.length"
          :key="`divider-${i}`"
          class="my-0"
        />
      </template>
    </div>
  </v-theme-provider>
</template>

<script>
  export default {
    name: 'BaseBusinessContact',

    props: {
      dark: Boolean,
      dense: Boolean,
      title: String,
    },

    data: () => ({
      business: [
        {
          icon: 'mdi-map-marker-outline',
          title: 'Address',
          text: 'Tancitaro 218 Col. San Agustín c.p 37240 León, Guanajuato',
        },
        {
          icon: 'mdi-phone',
          title: 'Phone',
          text: '<a href="tel:4773954427">(477)395-44-27</a>',
        },

        {
          icon: 'mdi-email-outline',
          title: 'Email',
          text: '<a href="mailto:ventas@curticova.com">ventas@curticova.com</a>',
        },
      ],
    }),
  }
</script>
