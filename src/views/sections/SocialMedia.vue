<template>
  <v-theme-provider dark>
    <base-section
      id="social"
      class="accent text-center"
      space="56"
    >
      <base-icon class="mb-8">
        mdi-facebook
      </base-icon>

      <base-section-heading
        color="transparent"
        title="Redes Sociales"
      >
        Visita nuestra Pagina
      </base-section-heading>

      <!-- <a
        class="d-inline-block mb-8"
        href="https://fb.me/curticova"
        style="text-decoration: none;"
        target="_blank"
      >
        https://fb.me/curticova
      </a>

      <div class="py-4" /> -->

      <v-btn
        class="font-weight-bold"
        color="white"
        href="https://fb.me/curticova"
        light
        min-width="168"
        target="_blank"
        x-large
      >
        Siguenos

        <v-icon right>
          mdi-open-in-new
        </v-icon>
      </v-btn>
    </base-section>
  </v-theme-provider>
</template>

<script>
  export default {
    name: 'SectionNews',

    provide: {
      heading: { align: 'center' },
    },
  }
</script>
