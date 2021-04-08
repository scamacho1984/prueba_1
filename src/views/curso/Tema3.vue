<template lang="pug">
.curso-main-container.pb-3
  BannerInterno(titulo="3. Habitaciones hoteleras")
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5

    p Dentro de la Norma técnica sectorial colombiana NTSH006 se deben considerar los siguientes aspectos en las habitaciones: seguridad, dimensiones en donde se incluye el baño y closet, muebles, conexiones eléctricas, ropa de cama, piso, ventanas, iluminación, baños y sus componentes entre otros ducha, toallas, presión del agua

    figure.mb-5
      img(src="@/assets/curso/tema3/tema3-main.png")

    h2.h3#t_3_1 3.1 Tipo de habitaciones y acomodación:

    .row.py-5.mb-4.g-4.justify-content-md-left
      .col-12.col-md-6.col-lg-4
        .p-4.bg-azul-claro.h-100
          img.auto(src="@/assets/curso/tema3/individual.png")
          p <strong>Individual:</strong> una habitación asignada a una persona. Las medidas de las camas individuales pueden ser: 90 centímetros de ancho por 190 de largo. Acomodación: puede tener una o más camas pero solo es ocupada por una persona.
      .col-12.col-md-6.col-lg-4
        .p-4.bg-azul-claro.h-100
          img.auto(src="@/assets/curso/tema3/doble.png")
          p <strong>Doble:</strong> una habitación asignada a dos personas. Las medidas de las camas dobles pueden ser: 140 centímetros de ancho por 190 de largo. Acomodación: puede tener una o más camas.
      .col-12.col-md-6.col-lg-4
        .p-4.bg-azul-claro.h-100
          img.auto(src="@/assets/curso/tema3/triple.png")
          p <strong>Triple:</strong> una habitación asignada a tres personas. Acomodación: puede tener dos o más camas.

      .col-12.col-md-6.col-lg-4
        .p-4.bg-azul-claro.h-100
          img.auto(src="@/assets/curso/tema3/queen.png")
          p <strong>Queen:</strong> una habitación con una cama de matrimonio. Las medidas de las camas Queen Size son 1,5 metros de ancho por 2 metros de largo. Acomodación: puede ser ocupado por una o más personas.
      .col-12.col-md-6.col-lg-4
        .p-4.bg-azul-claro.h-100
          img.auto(src="@/assets/curso/tema3/king.png")
          p <strong>King:</strong> una habitación con una cama king-size. las medidas de las camas King Size son de 2 metros de ancho x 2 metros de largo. Acomodación: puede ser ocupado por una o más personas.
      .col-12.col-md-6.col-lg-4
        .p-4.bg-azul-claro.h-100
          img.auto(src="@/assets/curso/tema3/twin.png")
          p <strong>Twin:</strong> una habitación con dos camas iguales. Acomodación: puede ser ocupado por una o más personas.

      .col-12.col-md-6.col-lg-4
        .p-4.bg-azul-claro.h-100
          img.auto(src="@/assets/curso/tema3/suite.png")
          p <strong>Suite:</strong> un salón o sala de estar conectada a uno o más dormitorios. Acomodación: de acuerdo al número de camas puede ser asignada a una persona o más.
      .col-12.col-md-6.col-lg-4
        .p-4.bg-azul-claro.h-100
          img.auto(src="@/assets/curso/tema3/junior_suite.png")
          p <strong>Junior Suite:</strong> una habitación individual con una cama y una sala de estar. A veces, el área para dormir está en un dormitorio separado del salón o la sala de estar. <strong>Acomodación:</strong> por su tamaño generalmente puede ser ocupada por dos máximo tres personas.
      .col-12.col-md-6.col-lg-4
        .p-4.bg-azul-claro
          img.auto(src="@/assets/curso/tema3/habitaciones_comunicadas.png")
          p <strong>Habitaciones comunicadas:</strong> habitaciones con puertas de entrada individuales desde el exterior y una puerta de conexión entre ellas. Los huéspedes pueden moverse entre habitaciones sin pasar por el pasillo.

      .col-12.col-md-6.col-lg-4
        .p-4.bg-azul-claro
          img.auto(src="@/assets/curso/tema3/habitaciones_contiguas.png")
          p <strong>Habitaciones contiguas:</strong> habitaciones con una pared común, pero sin puerta de conexión.
      .col-12.col-md-6.col-lg-4
        .p-4.bg-azul-claro
          img.auto(src="@/assets/curso/tema3/habitaciones_adyacentes.png")
          p <strong>Habitaciones adyacentes:</strong> habitaciones cercanas, tal vez al otro lado del pasillo.


    h2.h3#t_3_2 3.2 Servicios complementarios

    .row.align-items-stretch
      .col-12.col-md-4.px-4.py-5(style="background: #42C9EC")
        img.auto(src="@/assets/curso/tema3/control.png" width="46" height="74")
        p <strong>El planning nominal.</strong>
        p Es el más indicado para pequeños establecimientos, en los que resulta posible realizar la reserva y asignación de la habitación en un mismo momento. Es  una planilla en la que se incorporan las fechas del mes y la numeración de las habitaciones, puede ir acompañada de información relativa a sus características, los servicios  y  la ubicación.
      .col-12.col-md-4.px-4.py-5(style="background: #FFB74D")
        img.auto(src="@/assets/curso/tema3/control.png" width="46" height="74")
        p <strong>El planning numérico.</strong>
        p Su utilización es válida para establecimientos de cualquier tamaño, pero está especialmente pensado para hoteles con mucho movimiento.
      .col-12.col-md-4.px-4.py-5(style="background: #471E89")
        img.auto(src="@/assets/curso/tema3/control.png" width="46" height="74")
        p(style="color: white") <strong>El planning forecast.</strong>
        p(style="color: white") Se utiliza en hoteles de gran capacidad y notable movimiento de entradas y salidas, generalmente motivado por una estancia media muy baja, de escaso uso en la actualidad, se configura para impresos mensuales.

    p Se consideran servicios complementarios los siguientes:

    .row.g-4.mb-4.pb-4
      .col-12.col-md-6.px-5
        .row.justify-content-between.mt-5.p-4.bg-azul-claro.h-100
          .col-12.col-md-3
            img.auto(src="@/assets/curso/tema3/servicios-1.png")
          .col-12.col-md-9
            p <strong>Recepcion y atencion permanente</strong>
      .col-12.col-md-6.px-5
        .row.justify-content-between.mt-5.p-4.bg-azul-claro.h-100
          .col-12.col-md-3
            img.auto(src="@/assets/curso/tema3/servicios-2.png")
          .col-12.col-md-9
            p <strong>Limpieza periódica del alojamiento.</strong>
      .col-12.col-md-6.px-5
        .row.justify-content-between.mt-5.p-4.bg-azul-claro.h-100
          .col-12.col-md-3
            img.auto(src="@/assets/curso/tema3/servicios-3.png")
          .col-12.col-md-9
            p <strong>Recepcion y atencion permanente</strong>
      .col-12.col-md-6.px-5
        .row.justify-content-between.mt-5.p-4.bg-azul-claro.h-100
          .col-12.col-md-3
            img.auto(src="@/assets/curso/tema3/servicios-4.png")
          .col-12.col-md-9
            p <strong>Limpieza periódica del alojamiento.</strong>
      .col-12.col-md-6.px-5
        .row.justify-content-between.mt-5.p-4.bg-azul-claro.h-100
          .col-12.col-md-3
            img.auto(src="@/assets/curso/tema3/servicios-5.png")
          .col-12.col-md-9
            p <strong>Cajilla de seguridad.</strong>
      .col-12.col-md-6.px-5
        .row.justify-content-between.mt-5.p-4.bg-azul-claro.h-100
          .col-12.col-md-3
            img.auto(src="@/assets/curso/tema3/servicios-6.png")
          .col-12.col-md-9
            p <strong>También se incluye los servicios de restaurante y room services</strong>
      .col-12.col-md-6.px-5
        .row.justify-content-between.mt-5.p-4.bg-azul-claro
          .col-12.col-md-3
            img.auto(src="@/assets/curso/tema3/servicios-7.png")
          .col-12.col-md-9
            p <strong>Prestación de servicios adicionales como: lavandería, custodia de maletas, prensa, etc</strong>
      .col-12.col-md-6.px-5
        .row.justify-content-between.mt-5.p-4.bg-azul-claro
          .col-12.col-md-3
            img.auto(src="@/assets/curso/tema3/servicios-8.png")
          .col-12.col-md-9
            p <strong>Salones de eventos.</strong>
        .row.justify-content-between.mt-5.p-4.bg-azul-claro
          .col-12.col-md-3
            img.auto(src="@/assets/curso/tema3/servicios-9.png")
          .col-12.col-md-9
            p <strong>Locales comerciales.</strong>


    h2.h3#t_3_3 3.3 Convenciones

    p Las convenciones son las reglas o lineamientos simbólicos que se emplean en el diseño cartográfico para evitar malentendidos y confusiones en el momento de mostrar características geográficas o lugares. En los hoteles se trabaja con una gran cantidad de siglas y símbolos como instrumento para conocer el estado de las habitaciones y las tarifas entre otros; para facilitar el trabajo.

    p Se utiliza con símbolos, una letra o un par de letras que indican el estado de las habitaciones.

    p Estas siglas no son universales, aunque sí se declinan por la simplicidad y la no-duplicación de siglas.

    .custom-alert.container.tarjeta.tarjeta__template--verde.px-3.pt-3.pb-2.px-sm-5.my-5
      .float-image.d-none.d-lg-block
        img.auto(src="@/assets/curso/tema3/importante.png")
      .ms-lg-3.ps-lg-5
        p.ms-lg-5 <strong>En los hoteles se trabaja con una gran cantidad de siglas y símbolos como instrumento para conocer el estado de las habitaciones y las tarifas entre otros.</strong>

</template>

<script>
import BannerInterno from '../../components/plantilla/BannerInterno'
import Tabs from '../../components/Tabs'
import Slider from '../../components/Slider'
export default {
  name: 'Tema3',
  components: {
    BannerInterno,
    Tabs,
    Slider,
  },
}
</script>

<style lang="sass" scoped>
.tarjeta-bg-over
  &:hover
    background-color: $color-sistema-g

table.table, tr, td
  border: none
  color: $color-sistema-a

table.table
  caption
    color: $color-sistema-a

  tr
    background-color: $color-sistema-e
    td:first-child
      width: 25%
      text-align: center
      font-weight: bold
      border-right: 2px solid $color-sistema-a

  tr:nth-child(even)
    background-color: $color-sistema-g
</style>
