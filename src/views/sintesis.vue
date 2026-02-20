<template lang="pug">
.curso-main-container.pb-3
  BannerInterno(icono="fas fa-sitemap" titulo="Síntesis")
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5

    p El siguiente mapa integra los criterios y especificidades de los conocimientos expuestos en el presente componente formativo:
   
    .row.justify-content-center
      .col-lg-10.mb-5
        figure
          img(src="@/assets/curso/temas/figuras/sintesis.svg", alt="La administración nos plantea cinco enfoques, los cuales son: 1. Enfoque en las tareas, el cual se relaciona con la administración científica. 2. Enfoque en las personas, el cual se asocia a la teoría del desarrollo organizacional, a la teoría del comportamiento organizacional y a la teoría de las relaciones humanas. 3. Enfoque en la estructura, relacionado con la teoría estructuralista, la teoría de la burocracia y la teoría clásica. 4. Enfoque en el ambiente, relacionado con la teoría estructuralista y la teoría contingencial. 5. Enfoque en la tecnología, que se maneja en la teoría contingencial. En la imagen también se presenta la administración estratégica como un proceso de diagnóstico y análisis empresarial. Además, se describen las diferentes etapas del proceso administrativo: planeación, organización, dirección y control.")
    .row.justify-content-center
      .col-lg-3
        a.anexo.mb-4(:href="obtenerLink('/downloads/Sintesis.pdf')" target="_blank")
          .anexo__icono
            img(src="@/assets/template/icono-pdf.svg")
          .anexo__texto
            p Anexo. Sintesis.pdf

</template>

<script>
export default {
  name: 'Sintesis',
  data: () => ({
    // variables de vue
  }),
  mounted() {
    this.$nextTick(() => {
      this.$aosRefresh()
    })
  },
  updated() {
    this.$aosRefresh()
  },
}
</script>

<style lang="sass"></style>
