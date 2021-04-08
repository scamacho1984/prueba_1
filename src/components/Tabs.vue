<template lang="pug">
.tabs.my-5.pb-5
  .tabs__triggers
    .row
      .col-12.col-md-6.col-lg.text-center.my-2.my-lg-0(v-for="elm of triggers" :key="`trigger-${elm.id}`" :class="isActive(elm.id) ? 'active':''")
        a( @click="setActive(elm.id)") {{elm.title}}

  .tabs__contenido
    div.panel(v-for="elm of elementos" :key="elm.id" v-html="elm.html" :class="isActive(elm.id)?'active':''")

  .tabs-slot
    slot

</template>

<script>
export default {
  name: 'Tabs',
  data: () => ({
    mainId: Math.floor(Math.random() * 10000000),
    activeItem: 0,
    triggers: [],
    elementos: [],
  }),
  methods: {
    crearElementos() {
      this.triggers = this.$slots.default.map((elemento, index) => ({
        id: this.mainId + index + 1,
        title: elemento.data.attrs.titulo,
      }))
      this.elementos = this.$slots.default.map((elemento, index) => ({
        id: this.mainId + index + 1,
        html: elemento.elm.outerHTML,
      }))
      this.activeItem = this.elementos[0].id
    },
    isActive(menuId) {
      return this.activeItem == menuId
    },
    setActive(menuId) {
      this.activeItem = menuId
    },
  },
  mounted() {
    this.$nextTick(() => {
      if (!this.elementos.length) {
        this.crearElementos()
      }
    })
  },
}
</script>

<style lang="sass" scoped>
.tabs
  &__triggers
    .col-12
      padding: 0
      padding-bottom: 10px
      border-bottom: 3px solid #E8E8E8

      &.active,
      &:hover
        border-color: $color-curso-e

        a
          font-weight: bold

          &::after
            content: ''
            border-color: $color-curso-e transparent transparent transparent
            border-style: solid
            border-width: 6px
            width: 0
            height: 0
            position: absolute
            left: 50%
            bottom: -25px

      a
        display: block
        border-left: 1px solid #E8E8E8
        position: relative

      a
        border-right: 1px solid #E8E8E8

  &__contenido
    border: 1px solid #E8E8E8


    .panel
      display: none
      transition: all 0.5s ease-out

      &.active
        display: block

.tabs-slot
  display: none

@media (min-width: $bp-min-lg)
  .tabs
    &__triggers
      .col-12:first-child
      margin-left: 12px

      .col-12:last-child
        margin-right: 12px
</style>
