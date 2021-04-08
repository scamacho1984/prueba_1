<template lang="pug">
section
  BannerPrincipal

  //- Resultados de aprendizaje
  #resultados.pb-5
  .container.tarjeta.tarjeta__template--azul-claro.px-3.py-4.px-sm-5
    div.row.align-items-center
      .titulo__template--a.col-2
        span.h6 Resultado<br>de aprendizaje

      .col-12.col-md.ps-md-5.mt-4.mt-md-0
        span Ofrecer servicios del establecimiento de acuerdo con portafolio, tipo de hotel y protocolos.

  //- Desarrollo de contenidos
  #contenidos.pb-5
  .container.tarjeta.tarjeta__template--azul-claro.px-3.py-4.px-sm-5.pb-sm-5
    .titulo__template--a.mb-4
      span.h6 Desarrollo<br>de contenidos

    .tarjeta--blanca.p-3.p-sm-4
      .desarrollo-contenidos
        router-link.desarrollo-contenidos__item(
          v-for="item of desarrolloContenidosData"
          :key="'desarrollo-'+item.nombreRuta"
          :to="{name: item.nombreRuta}"
        )
          .desarrollo-contenidos__item__texto
            span.desarrollo-contenidos__item__icono(v-if="item.hasOwnProperty('numero')" ) {{item.numero}}
            i.desarrollo-contenidos__item__icono(v-else :class="item.icono")
            span {{item.titulo}}

          a.boton--sm.d-none.d-md-block
            span Ver más

  //- Tarjeta Naranja
  .custom-alert.container.tarjeta.tarjeta__template--naranja.px-3.py-4.px-sm-5.mt-5
    .float-image.d-none.d-lg-block
      img(src="@/assets/curso/listo.png")
    .row.align-items-center.ps-lg-5
      .col-sm-12.col-lg.ps-lg-5.ms-lg-5
        span.h3.ms-lg-5.mb-lg-4 ¿Todo listo para iniciar?
      .col-sm-12.col-lg
        span Es momento de empezar tu proceso académico, descubre y explora todas las habilidades cognitivas en este nuevo curso.
      .col-sm-12.col-lg-1.ms-lg-5.mt-sm-4.mt-lg-0
        router-link.boton--color-sistema-a.boton--sm.mt-4.mt-lg-0(:to="{name: 'tema1'}")
          span.me-1 Iniciar
          i(class="fas fa-angle-right")

  //- Créditos
  #creditos.pb-5
  .container.tarjeta.tarjeta__template--azul-claro.px-3.py-4.px-sm-5.mb-5
    .titulo__template--a.mb-4
      span.h6 Créditos

    CreditosComp

  Footer
  

</template>
<script>
import { menuPrincipal } from '../config/global'
import BannerPrincipal from '../components/plantilla/BannerPrincipal'
import CreditosComp from '../components/plantilla/CreditosComp'
import Footer from '../components/plantilla/Footer'
export default {
  name: 'Inicio',
  components: {
    BannerPrincipal,
    CreditosComp,
    Footer,
  },
  data: () => ({
    menuPrincipalData: menuPrincipal,
  }),
  computed: {
    desarrolloContenidosData() {
      const allMenuData = [
        ...this.menuPrincipalData.menu,
        ...this.menuPrincipalData.subMenu,
      ]
      return allMenuData.filter(item => item.desarrolloContenidos)
    },
  },
}
</script>

<style lang="sass" scoped>
.float-image
  height: 100px
  width: 149px

.row
  padding-left: 15px

.resultados-aprendizaje
  &__item
    margin-bottom: 20px
    &:last-child
      margin-bottom: 0

.desarrollo-contenidos
  &__item
    display: flex
    align-items: center
    justify-content: space-between
    margin-bottom: 25px
    padding: 5px
    border-radius: $base-border-radius

    &__texto
      display: flex
      align-items: center

    &__icono
      display: block
      background-color: $color-sistema-g
      font-size: 20px
      font-weight: $base-black-font-weight
      text-align: center
      padding: 10px
      line-height: 1em
      width: 40px
      margin-right: 15px

    &:last-child
      margin-bottom: 0

    &:hover
      background-color: $color-sistema-g
      font-weight: $base-black-font-weight
      color: $color-sistema-a
</style>
