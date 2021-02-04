<template>
  <base-section
    id="map"
    space="0"
  >
    <iframe
      src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3721.361559169383!2d-101.67728748570029!3d21.1380048894171!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x842bbf17a99bb269%3A0xb266de420bc3922a!2sTanc%C3%ADtaro%20218%2C%20San%20Agustin%2C%2037240%20Le%C3%B3n%2C%20Gto.!5e0!3m2!1ses!2smx!4v1612456492284!5m2!1ses!2smx"
      width="100%"
      height="450"
      frameborder="0"
      style="border:0;"
      allowfullscreen=""
      aria-hidden="false"
      tabindex="0"
    />
  </base-section>
</template>

<script>
  export default {
    name: 'SectionMap',

    provide: {
      heading: { align: 'center' },
    },
  }
</script>
