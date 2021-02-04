<template>
  <base-section
    id="features"
    class="secondary"
  >
    <v-responsive
      class="mx-auto"
      max-width="1350"
    >
      <v-container fluid>
        <v-row justify="center">
          <v-col
            v-for="card in cards"
            :key="card.title"
            cols="12"
            sm="4"
            md="5"
          >
            <base-info-card
              align="center"
              dark
              v-bind="card"
            />
          </v-col>
        </v-row>
      </v-container>
    </v-responsive>
  </base-section>
</template>

<script>
  export default {
    name: 'SectionFeatures',

    data: () => ({
      cards: [
        {
          icon: 'mdi-google-analytics',
          title: 'Mision',
          text:
            'El Mostrar a la sociedad todo el tratamiento del cuero para convertirlo en uno de los artículos más usados dentro de la sociedad, implantándose en ella como un producto que demuestra elegancia y sofisticación.',
        },
        {
          icon: 'mdi-eye-settings-outline',
          title: 'Vision',
          text:
            'Lograr un posicionamiento local y regional, convirtiéndonos en una empresa líder en la producción, venta y distribución del cuero en su producto final, para brindar alta calidad y satisfacción con un precio acorde a los requerimientos y procesos que el cliente necesite. ',
        },
      ],
    }),
  }
</script>
