<template>
  <base-section
    id="affiliates"
    space="16"
  >
    <v-container>
      <base-section-heading
        title="Agradecemos a todos nuestros clientes por su confianza en nuestros primeros 5 años de operacion, comprometiendonos como siempre en brindarles la mejor calidad en nuestros productos con los mejores precios competitivos y seguimos inovando para ofrecer el mejor servicio."
      />

      <!-- <v-slide-group>
        <template v-for="n in 6">
          <v-slide-item
            :key="n"
            class="align-self-center"
          >
            <base-img
              :src="require(`@/assets/logo-${n}-${$vuetify.theme.isDark ? 'dark' : 'light'}.png`)"
              color="grey"
              contain
              height="40"
              width="128"
            />
          </v-slide-item>

          <v-responsive
            v-if="n < 6"
            :key="`divider-${n}`"
            class="text-center"
            height="56"
            width="48"
          >
            <v-divider vertical />
          </v-responsive>
        </template>
      </v-slide-group> -->
    </v-container>
  </base-section>
</template>

<script>
  export default {
    name: 'SectionAffiliates',
  }
</script>
