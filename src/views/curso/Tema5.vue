<template lang="pug">
.curso-main-container.pb-3
  BannerInterno(titulo="5. Tarifas")
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5
    figure.mb-5
      img(src="@/assets/curso/tema5/tema5-main.jpg")

    p Los hoteles manejan diferentes tarifas, para diversos tipos de clientes. El mercado turístico como cualquier otro mercado se rige por el libre juego de la oferta y la demanda, en ese sentido cualquier hotel u organización puede ofrecer sus servicios bajo estos principios; así mismo los conceptos de temporadas  alta y baja demanda, si se trata de baja demanda los precios tenderán a la reducción y si es de alta demanda obligará al incremento.

    .row.justify-content-between
      .col-12.col-md-5.my-4.my-md-0
        .border.p-5.fs-3.fw-light.border-radius-20.lh-sm
          span Generalmente los hoteles aplican las tarifas ya establecidas por ventas a las reservaciones que se generen por parte de compañías, agencias de viajes, líneas aéreas o dependencias gubernamentales (Fernández, 2011).
      .col-12.col-md-6.my-4.my-md-0
        figure
          img(src="@/assets/curso/tema5/tarifa1.jpg")
          p Muchos elementos influyen en la determinación de tarifas de una habitación.  Categoría del hotel. Tipo de hotel. Temporada. Día de la semana. Tiempo de estancia. Ubicación del hotel. Ubicación dentro del hotel. Tamaño de la habitación. Plan de alimentación. Tarifas promocionales. Tipo de cambio y si el cliente hace parte de un grupo.

    h2.h3#t_5_1 5.1 Tipos
    ul
      li <strong>Tarifa oficial o Rack (Rack Rate):</strong> <br/> es la tarifa minorista oficial  pública y se aplica en épocas de alta ocupación.
      li <strong>Tarifa BAR (Best Available Rate):</strong> <br/> mejor tarifa disponible del día, suelen ser precios flexibles, basados en descuentos sobre la tarifa rack, según las condiciones del mercado.
      li <strong>Tarifa Promocional: </strong> <br/> Cualquier tarifa especial o paquete que se ofrece por tiempo limitado y en ocasiones anclada a un evento especial para incrementar la venta de habitaciones.
      li <strong>Tarifa de agencias para reservas individuales: </strong> <br/> puede ser la tarifa rack o BAR neta, es decir, con la comisión de la agencia ya descontada, se pueden dar los precios brutos, sin descontar la comisión.
      li <strong>Tarifa Corporativa: </strong> <br/> tarifa especial acordada para viajeros de negocios y  empresas, cuyo precio está en función del número de habitaciones anuales, es confidencial sujeta a las condiciones de un contrato.
      li <strong>Tarifa Preferencial: </strong> <br/> es una corporativa con precios muy reducidos para empresas que generan gran volumen de negocio para el hotel, son revisadas anualmente y están sujetas al nivel de facturación acordado.
      li <strong>Tarifa FIT (Foreign International Travel): </strong> <br/> es una tarifa para agencias mayoristas internacionales, a precios muy reducidos, y que suele incluir varios servicios (media pensión o pensión completa).
      li <strong>Tarifa Grupal: </strong> <br/> son acordadas con las agencias mayoristas y minoristas, en función de la facturación de la agencia y de las condiciones del grupo. 
      li <strong>Tarifa de compra anticipada: </strong> <br/> especial para pasajeros que puedan cambiar la flexibilidad de su viaje por una tarifa con descuento adicional.
      li <strong>Tarifa de Día: </strong> <br/> especial para pasajeros que puedan cambiar la flexibilidad de su viaje por una tarifa con descuento adicional.
      li <strong>Tarifa profesional: </strong> <br/> solo se otorga a ciertos profesionales como personal de aerolíneas, militares, agentes de viajes, diplomáticos, clérigos.
      li <strong>Tarifa de la tercera edad: </strong> <br/> descuento que se ofrece al adulto mayor, cada hotel maneja su política en cuanto a la edad (más de 55, 60 y 65 años).
      li <strong>Tarifa de fin de semana: </strong> <br/> diferente a las tarifas normales entre semana, puede ser menor o más alta y varia de un hotel a otro.
      li <strong>Paquetes de Estancia: </strong> <br/> son tarifas que engloban un conjunto de servicios con un único precio final para ser  vendidos, igual que la tarifa oficial, durante todo un año y con diferente precio por temporada.
      li <strong>Ofertas y Promociones: </strong> <br/> se crean para incentivar la venta en momentos de baja ocupación, son similares a los paquetes, pero con una vigencia más corta y con precios más bajos que los establecidos en la tarifa oficial.
      li <strong>Gratuidad: </strong> <br/> Alojamiento gratuito para clientes, clientes potenciales, clientes descontentos. Normalmente es decisión del director del establecimiento.
      
    h2.h3#t_5_2 5.2 Planes
    p Generalmente, el precio que pagamos por el hospedaje en un establecimiento de alojamiento incluye un conjunto de servicios dentro del <strong>"plan de alojamiento"</strong> que hemos contratado, entre estos se encuentra los servicios de alimentación, entretenimiento y los básicos incluidos en el alojamiento como el descanso y la limpieza.

    .tarjeta--color-curso-i.px-4.pt-4.pt-md-1.mb-4
        .row.py-md-3.align-items-center
          .col-12.col-md-3.col-lg-2.d-flex.align-items-center
            img.auto(src="@/assets/curso/tema5/plan1.png")
          .col
            p <strong>Plan Europeo.</strong> Tarifa de hotel que incluye la habitación sin ningún alimento.

    .tarjeta--color-curso-i.px-4.pt-4.pt-md-1.mb-4
        .row.py-md-3.align-items-center
          .col-12.col-md-3.col-lg-2.d-flex.align-items-center
            img.auto(src="@/assets/curso/tema5/plan2.png")
          .col
            p <strong>Plan Continental.</strong> Incluye el servicio de habitación además de un desayuno básico (pan tostado, mantequilla, mermelada y jugo de naranja, café o té). 
            p Muchos hoteles en la actualidad han cambiado este plan incluyendo desayunos más completos o incluyendo un servicio de buffet para la primera comida del día

    .tarjeta--color-curso-i.px-4.pt-4.pt-md-1.mb-4
        .row.py-md-3.align-items-center
          .col-12.col-md-3.col-lg-2.d-flex.align-items-center
            img.auto(src="@/assets/curso/tema5/plan3.png")
          .col
            p <strong>Plan Americano.</strong> Tarifa de hotel que incluye el alojamiento y  tres comidas al día (desayuno, almuerzo y cena). Se conoce como pensión completa o alojamiento completo.

    .tarjeta--color-curso-i.px-4.pt-4.pt-md-1.mb-4
        .row.py-md-3.align-items-center
          .col-12.col-md-3.col-lg-2.d-flex.align-items-center
            img.auto(src="@/assets/curso/tema5/plan4.png")
          .col
            p <strong>Plan Americano Modificado.</strong> Incluye la habitación, el desayuno y una de las comidas (almuerzo o cena), queda a elección del huésped.

    .tarjeta--color-curso-i.px-4.pt-4.pt-md-1.mb-4
        .row.py-md-3.align-items-center
          .col-12.col-md-3.col-lg-2.d-flex.align-items-center
            img.auto(src="@/assets/curso/tema5/plan5.png")
          .col
            p <strong>Plan Todo Incluido.</strong> Es uno de los planes más populares, pues por un solo precio incluye las tres comidas del día, snacks, bocadillos y bebidas. Es común en centros vacacionales, resorts y cadenas hoteleras. También conocido como All Inclusive o plan Absolute.

    .tarjeta--color-curso-i.px-4.pt-4.pt-md-1.mb-4
        .row.py-md-3.align-items-center
          .col-12.col-md-3.col-lg-2.d-flex.align-items-center
            img.auto(src="@/assets/curso/tema5/plan6.png")
          .col
            p <strong>Bed & Breakfast (B&B).</strong> Ofrece una habitación con desayuno completo (cama y desayuno).

    Slider#slider-tema-5
      .row.justify-content-between
        .col-12.col-md-4.text-end
          p.h2.ps-4.lh-sm La revolución de la hotelería moderna
          p Vino con la Revolución industrial y la generalización de los medios de transporte que permitió a las personas desplazarse de forma masiva de un lugar a otro. Por aquel entonces, <strong>los viajes estaban reservados a clases más adineradas que podían salir de vacaciones y por tanto exigían alojamientos acorde a su nivel económico</strong>. Se generalizan establecimientos para comer y pernoctar, y surge así lo que conocemos como hotelería moderna.
        .col-12.col-md-8
          figure.ps-5
            img(src="@/assets/curso/tema5/slide1.jpg")

      .row.justify-content-between
        .col-12.col-md-4.text-end
          p.h2.ps-4.lh-sm La revolución de la hotelería moderna
          p El primer hotel de concepción moderna en 1807 fue el <strong>"Badische Hof"</strong>, construido en Alemania, comenzó con 18 columnas dóricas que se extendían a lo largo de tres pisos, lo que hizo que el comedor fuera el centro de atención y con algunos aspectos novedosos para la época como sala de lectura o biblioteca.
        .col-12.col-md-8
          figure.ps-5
            img(src="@/assets/curso/tema5/slide2.jpg")

      .row.justify-content-between
        .col-12.col-md-4.text-end
          p.h2.ps-4.lh-sm La revolución de la hotelería moderna
          p Con la aparición del ferrocarril, también surgen los hoteles "término" para dar alojamiento a los viajeros al lado de las estaciones.
        .col-12.col-md-8
          figure.ps-5
            img(src="@/assets/curso/tema5/slide3.jpg")

      .row.justify-content-between
        .col-12.col-md-4.text-end
          p.h2.ps-4.lh-sm La revolución de la hotelería moderna
          p Con la aparición del ferrocarril, también surgen los hoteles "término" para dar alojamiento a los viajeros al lado de las estaciones.
        .col-12.col-md-8
          figure.ps-5
            img(src="@/assets/curso/tema5/slide4.jpg")

      .row.justify-content-between
        .col-12.col-md-4.text-end
          p.h2.ps-4.lh-sm La revolución de la hotelería moderna
          p Francia fue el gran referente en la industria hotelera desde mediados del siglo XIX hasta que a finales del siglo XX, Estados Unidos tomó el relevo con sus grandes cadenas hoteleras y gigantes establecimientos. 
        .col-12.col-md-8
          figure.ps-5
            img(src="@/assets/curso/tema5/slide5.jpg")

</template>

<script>
import BannerInterno from '../../components/plantilla/BannerInterno'
import Tabs from '../../components/Tabs'
import Slider from '../../components/Slider'
export default {
  name: 'Tema5',
  components: {
    BannerInterno,
    Tabs,
    Slider,
  },
}
</script>

<style lang="sass" scoped></style>
