<template lang="pug">
.slider(:style="{height: rendered ? getActiveHeight() : 0}")
  .slider__slide(v-for="elm in elementos" :key="elm.id" :ref="elm.id" v-html="elm.html" :class="slideClass(elm.id)")

  //- Separo el diseño de los botones para que se puedan personalizar
  .slider__action-buttons
    a.prev(@click="prevSlide()")
      i.fas.fa-chevron-left
    a.next(@click="nextSlide()")
      i.fas.fa-chevron-right

  .slider-slot
    slot
</template>

<script>
export default {
  name: 'Slider',
  data: () => ({
    mainId: Math.floor(Math.random() * 10000000),
    activeSlide: 0,
    elementos: [],
    height: 0,
    rendered: false,
  }),
  mounted() {
    this.$nextTick(() => {
      if (!this.elementos.length) {
        this.crearElementos()
      }
    })
  },
  methods: {
    crearElementos() {
      this.elementos = this.$slots.default.map((elemento, index) => ({
        id: this.mainId + index + 1,
        html: elemento.elm.outerHTML,
      }))
      this.domUpdated()
      this.activeSlide = this.elementos[0].id
    },
    slideClass(elmId) {
      let smallestId = this.mainId + 1
      let biggestId = this.mainId + this.$slots.default.length
      if (elmId == this.activeSlide) return 'activeSlide'
      if (
        elmId == this.activeSlide - 1 ||
        (this.activeSlide - 1 < smallestId && elmId == biggestId)
      )
        return 'lastSlide'
      if (
        elmId > this.activeSlide ||
        (this.activeSlide + 1 > biggestId && elmId == smallestId)
      )
        return 'nextSlide'
      return 'nextSlide'
    },
    prevSlide() {
      let prevId = this.activeSlide - 1
      let smallestId = this.mainId + 1
      let biggestId = this.mainId + this.$slots.default.length
      if (prevId < smallestId) {
        this.activeSlide = biggestId
      } else {
        this.activeSlide = prevId
      }
    },
    nextSlide() {
      let nextId = this.activeSlide + 1
      let smallestId = this.mainId + 1
      let biggestId = this.mainId + this.$slots.default.length
      if (nextId > biggestId) {
        this.activeSlide = smallestId
      } else {
        this.activeSlide = nextId
      }
    },
    getActiveHeight() {
      return this.$refs[this.activeSlide][0].scrollHeight + 'px'
    },
    domUpdated() {
      this.rendered = false
      setTimeout(() => {
        this.rendered = true
      }, 500)
    },
  },
}
</script>

<style lang="sass">
.slider
  display: flex
  position: relative
  margin-top: 4rem
  overflow: hidden

  &__slide
    left: 0
    position: absolute
    top: 0
    transition: all 0.5s ease-out

    &.activeSlide
    opacity: 1
    transform: translateX(0)

    &.lastSlide
      opacity: 0
      transform: translateX(-100%)

    &.nextSlide
      opacity: 0
      transform: translateX(100%)

.slider-slot
  display: none
</style>
