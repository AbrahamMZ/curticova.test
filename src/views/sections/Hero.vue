<template>
  <section id="hero">
    <v-img
      :min-height="minHeight"
      :src="require('@/assets/skin-2.jpg')"
      class="white--text"
      gradient="to bottom, rgba(11, 28, 61, .5), rgba(0,0,0,.4)"
    >
      <v-container class="fill-height px-4 py-12">
        <v-responsive
          class="d-flex align-center mx-auto"
          height="100%"
          max-width="700"
          width="100%"
        >
          <base-subheading
            weight="regular"
            title="NOS ENCANTA HACER LAS COSAS SIMPLES E INCREÍBLES"
          />

          <base-heading
            size="text-h2"
            title="BIENVENIDO A CURTICOVA S.A. DE C.V."
            weight="medium"
          />

          <base-body>
            Somos una empresa constituida para atender las necesidades de la
            industria del cuero y del calzado.
          </base-body>

          <div
            :class="
              $vuetify.breakpoint.smAndDown
                ? 'flex-column align-start'
                : 'align-center'
            "
            class="d-flex flex-wrap"
          >
            <!-- <base-btn>
              Discover More
            </base-btn>

            <span class="font-weight-bold ml-6 mr-4 my-4">or</span>

            <base-btn
              :ripple="false"
              class="pa-1"
              height="auto"
              text
            >
              Get Started Now
            </base-btn> -->
          </div>
        </v-responsive>
      </v-container>
    </v-img>
  </section>
</template>

<script>
  export default {
    name: 'SectionHero',

    provide: {
      theme: { isDark: true },
    },

    computed: {
      minHeight () {
        const height = this.$vuetify.breakpoint.mdAndUp ? '100vh' : '50vh'

        return `calc(${height} - ${this.$vuetify.application.top}px)`
      },
    },
  }
</script>
