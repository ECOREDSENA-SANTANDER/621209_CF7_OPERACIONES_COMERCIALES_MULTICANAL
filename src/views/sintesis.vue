<template lang="pug">
.curso-main-container.pb-3
  BannerInterno(icono="fas fa-sitemap" titulo="Síntesis")
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5
    p.mb-5 La correcta exhibición de productos en un punto de venta es vital para el éxito comercial, ya que afecta la decisión de compra del cliente. Una organización estratégica y una presentación eficaz no solo optimizan el espacio, sino que también mejoran la experiencia de compra y pueden incrementar las ventas. Una planificación adecuada en la disposición del surtido es clave para captar la atención del consumidor y facilitar su búsqueda de productos. A continuación, se presenta la temática relacionada con el componente: 

    .row.justify-content-center
      .col-lg-12
        .bg1.p-1.mb-5
          figure.my-3
            img(src="@/assets/curso/sintesis.svg", alt="Mapa conceptual titulado “Exhibición y vitrinismo en el formato comercial”. El esquema organiza la información en tres ejes principales: retail, surtido y muebles en el punto de venta. En retail se explican el establecimiento comercial, la arquitectura del establecimiento y los formatos comerciales. En surtido se presentan la estructura del surtido, el layout, el vitrinismo o visual merchandising, la señalización comercial, el planograma o planimetría, la exhibición de productos, el merchandising y los dispositivos de seguridad. En muebles en el punto de venta se abordan los tipos de muebles, la codificación de productos, la activación de marca, la rotación de categorías y el precio. El mapa muestra cómo estos elementos contribuyen a organizar los productos, facilitar la compra, atraer la atención del consumidor, proteger los productos y aumentar las ventas.")
      .col-auto
        a.anexo.mb-5(:href="obtenerLink('/downloads/Sintesis.pdf')" target="_blank")
          .anexo__icono
            img(src="@/assets/template/icono-pdf.svg")
          .anexo__texto
            p Anexo. Síntesis

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
