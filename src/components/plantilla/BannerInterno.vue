<template lang="pug">
.container-fluid.banner-interno
  .banner-interno__fondo(:style="{'background-image': `url(${globalData.fondoBannerPrincipal})`}")
  .container
    .banner-interno__titulo.py-5.position-relative
      .banner-interno__titulo__icono.me-3(v-if="icono.length")
        i(:class="icono")
      h1.h3.mb-0 {{titulo}}
      img.imagenBannerPrincipal.d-none.d-md-block(:src="globalData.imagenBannerPrincipal")
      
</template>

<script>
import { global } from '../../config/global'
export default {
  name: 'BannerInterno',
  props: {
    icono: {
      type: String,
      default: '',
    },
    titulo: {
      type: String,
      default: '',
    },
  },
  data: () => ({
    globalData: global,
  }),
}
</script>

<style lang="sass" scoped>
.banner-interno
  position: relative

  &__fondo
    position: absolute
    top: 0
    bottom: -50px
    left: 0
    right: 0
    background-size: cover
    background-position: center

  &__titulo
    display: flex
    align-items: center
    color: $color-banner-text
    &__icono
      display: block
      width: 32px
      height: 32px
      border-radius: 50%
      background-color: $color-banner-text
      position: relative
      i
        position: absolute
        left: 50%
        top: 50%
        transform: translate(-50%,-50%)
    .imagenBannerPrincipal
      width: 411px
      height: 297px
      position: absolute
      bottom: -22px
      right: 0
    h1
      color: $color-banner-text
      line-height: 1.1em

    @media(max-width: $bp-max-md)
      .imagenBannerPrincipal
        width: 300px
        height: 200px
</style>
