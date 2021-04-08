<template lang="pug">
.curso-main-container.pb-3
  BannerInterno(titulo="3. Comunicación")
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5

    figure.mb-5
      img(src="@/assets/curso/tema3/tema3-main.jpg")

    p La empresa hotelera capta sus ingresos en los productos y servicios que genera para vender, la venta de habitaciones es la razón de ser del hotel, así como también  el área que  mayores ganancias genera.

    p Una reservación es un acuerdo, verbal o escrito, que se establece entre el hotel y una persona natural o jurídica, donde el primero se compromete a realizar una prestación de alojamiento y demás servicios en una fecha preestablecida y por un periodo determinado; y el segundo, a recibir la prestación del servicio en la fecha reservada y  a realizar el pago del servicio, con consecuencia de penalización por cancelación.

    h2.h3#t_3_1 3.1 Objetivo de la gestión de reservas
    figure.my-5
      img(src="@/assets/curso/tema3/video.jpg")

    .row.justify-content-between.align-items-end
      .col-12.col-md-5
        blockquote.fs-3.fw-light(style="background-color: transparent") La gestión de reservas tiene como objetivo <span class="fw-normal">llevar un control permanente y actualizado de la ocupación del establecimiento hotelero</span>, teniendo en cuenta las entradas del día, habitaciones ocupadas, de salidas, cancelaciones de reservas, clientes no show, entre otros.
      .col-12.col-md-7
        .tarjeta.tarjeta__template--azul-claro.p-5
          p Requiere de acciones que permitan promover la venta  de habitaciones y conocer el comportamiento de la ocupación en el transcurso de un año, mediante  la elaboración de gráficas de ocupación mensual, <strong>con el fin de implementar las estrategias de ventas en determinados periodos</strong>, para lo cual es necesario  el manejo de un sistema de reservaciones y el conocimiento del servicio, la disponibilidad, tarifas, paquetes y promociones; también depende de la habilidad del agente de reservas, para lograr atraer al cliente y efectuar la venta. 

    h2.h3#t_3_2.my-5.pt-4 3.2 Componentes
    p Un PNR (Passenger Name Record) contiene los detalles de la reserva del pasajero o huésped, en relación con el viaje o permanencia en el hotel y sus <strong>componentes se denominan elementos, estos pueden ser obligatorios, OMC y tarifa.</strong>

    figure.my-5
      img(src="@/assets/curso/tema3/componentes.jpg")

    p Cuando se crea una reserva se pueden ingresar los elementos en cualquier orden, todos los elementos son numerados consecutivamente.

    h2.h3#t_3_3 3.3  Tipos
    p Se pueden distinguir:

    .row
      .col-12.col-md-6.col-lg-4.d-flex.align-items-stretch
        .tarjeta.tarjeta-bg-over.p-4
          img.auto(src="@/assets/curso/tema3/tipos1.png" width="72" height="70")
          p <strong>Reservas individuales</strong>
          p Aquellas realizadas de forma independiente para un número de personas inferior a 10. <strong>Puede proceder de un cliente particular</strong>, o haber sido realizadas por una agencia de viajes o una empresa.
      .col-12.col-md-6.col-lg-4.d-flex.align-items-stretch
        .tarjeta.tarjeta-bg-over.p-4
          img.auto(src="@/assets/curso/tema3/tipos2.png" width="72" height="70")
          p <strong>Reservas para grupos</strong>
          p Se considera grupo a partir de 10 personas que viajan juntas o tienen un nexo común y se alojan en el hotel en el mismo período de tiempo. <strong>Se reserva con antelación mediante un contrato entre el hotel y la agencia o empresa</strong>, o entre el hotel y el responsable del grupo, por el número de habitaciones bloqueadas.
      .col-12.col-md-6.col-lg-4.d-flex.align-items-stretch
        .tarjeta.tarjeta-bg-over.p-4
          img.auto(src="@/assets/curso/tema3/tipos3.png" width="72" height="70")
          p <strong>Confirmadas o no garantizadas</strong>
          p Son reservaciones provenientes de particulares o intermediarios, <strong>en las cuales no media ninguna garantía</strong>. El hotel fija una hora límite de chek-in que usualmente son las 18:00 horas, después de la cual, si los huéspedes no se presentan, la reservación se da de baja.
      .col-12.col-md-6.col-lg-4.d-flex.align-items-stretch
        .tarjeta.tarjeta-bg-over.p-4
          img.auto(src="@/assets/curso/tema3/tipos4.png" width="72" height="70")
          p <strong>Garantizadas</strong>
          p Una reservación garantizada significa que el hotel, si los huéspedes no se presentan en la fecha estipulada, le cobrará el importe correspondiente a una noche de alojamiento. <strong>Para garantizar la reserva de una habitación, se tiene que consignar el 50% del valor total de la estadía</strong>. Además, se puede garantizar a través de tarjetas de crédito, o cartas de las empresas.
      .col-12.col-md-6.col-lg-4.d-flex.align-items-stretch
        .tarjeta.tarjeta-bg-over.p-4
          img.auto(src="@/assets/curso/tema3/tipos5.png" width="72" height="70")
          p <strong>Tentativas</strong>
          p Cuando el cliente hace una reserva de prueba en temporada alta, <strong>el hotel le hace un seguimiento continuo</strong>, porque él debe ver la disponibilidad de habitaciones para reservar definitivamente o no.

    h2.h3#t_3_4 3.4 Estados
    p Este aspecto presenta tres opciones diferentes:

    .tarjeta--color-curso-m.my-3
      .row.align-items-stretch.justify-content-between
        .col-12.col-md-2.col-lg-2.d-flex.align-items-stretch
          div.bg-color-curso-g.px-4.d-flex.align-items-center.border-left-radius-20.py-3
            img.auto(src="@/assets/curso/tema2/target.png")
        .col-12.col-md.col-lg
          p Si la reserva se confirma, se marca la casilla correspondiente (OK).
    .tarjeta--color-curso-m.my-3
      .row.align-items-stretch.justify-content-between
        .col-12.col-md-2.col-lg-2.d-flex.align-items-stretch
          div.bg-color-curso-g.px-4.d-flex.align-items-center.border-left-radius-20.py-3
            img.auto(src="@/assets/curso/tema2/target.png")
        .col-12.col-md.col-lg
          p En el caso que la reserva no pueda confirmarse o no se ha garantizado mediante algo que el hotelero puede demandar, se puede solicitar la garantía y mientras se hace efectiva, la reserva queda bajo petición o solicitada (RQ).
    .tarjeta--color-curso-m.my-3
      .row.align-items-stretch.justify-content-between
        .col-12.col-md-2.col-lg-2.d-flex.align-items-stretch
          div.bg-color-curso-g.px-4.d-flex.align-items-center.border-left-radius-20.py-3
            img.auto(src="@/assets/curso/tema2/target.png")
        .col-12.col-md.col-lg
          p Por último, puede darse el caso de que no exista disponibilidad en el momento de la reserva, pero el cliente prefiera esperar hasta que se produzca una cancelación  o alguna habitación sea liberada, se marca como lista de espera (WL).

    h2.h3#t_3_5 3.5 Convenciones de estados de habitaciones

    p.h4.fw-light En los hoteles el estado de habitaciones se guía por códigos o abreviaturas que <span class="fw-normal">facilitan la elaboración de reportes de estado de habitaciones</span>, algunos hoteles utilizan convenciones en inglés y otros en español: 

    .row
      .col-12.col-md-4
        table.table.caption-top.border-top-radius-20
          caption.fw-bold.p-3.fs-6.text-center.border-top-radius-20.bg-color-curso-o Convenciones de estados de habitaciones ( Ingles)
          tbody
            tr
              td OC
              td Busy Clean
            tr
              td BD
              td Busy Dirty
            tr
              td BV
              td Dirty Vacancy
            tr
              td CV
              td Clean vacancy
            tr
              td  OS
              td Out of service (fuera de servicio)
            tr
              td  DND
              td Please do not disturb (Favor no molestar)
      .col-12.col-md-4
        table.table.caption-top.border-top-radius-20
          caption.fw-bold.p-3.fs-6.text-center.border-top-radius-20.bg-color-curso-o Convenciones de estados de habitaciones (Español)
          tbody
            tr
              td O
              td Ocupada
            tr
              td VL
              td Vacía Limpia
            tr
              td BS
              td Vacía Sucia
            tr
              td NM
              td No molestar
            tr
              td  F
              td  Fuera de Servicio
            tr
              td OSE
              td Ocupada sin equipaje
            tr
              td OND
              td Ocupada no durmió
            tr
              td ONS
              td Ocupada no desea servicio

    h2.h3#t_3_6 3.6 Procedimiento para reservar
    .row.justify-content-between
      .col-12.col-md-6
        p.h4.fw-light El proceso de reserva es aquel por medio del cual, un huésped <span class="fw-normal">solicita que se le garantice una habitación</span> para determinada fecha y hora, considerando las condiciones y necesidades,
        p expresada por el huésped, este proceso es muy completo porque se obtiene la información de  los datos del huésped: nombre, contacto, tipo de habitación, fecha y hora de llegada, tiempo de permanencia, fecha de salida, entre otros.

        p Las reservas llevan asociados una serie de procedimientos en los que se <strong>basa su recepción, aceptación y confirmación y en algunos casos su modificación o cancelación.</strong>

        p El procedimiento para atender las reservaciones que lleguen por los diferentes medios de comunicación: plataformas de reservas, reservas para grupos, agencias de viajes, manejar dinero proveniente de depósitos para garantizar las reservas; teniendo en cuenta los siguientes ítems:
        
      .col-12.col-md-5.d-flex.flex-column
        .d-flex.align-items-center.my-2
          img.auto(src="@/assets/curso/tema3/reserva1.png" width="92" height="92")
          p.fw-bold.ms-4 Manejo de solicitudes de reserva.
        .d-flex.align-items-center.my-2
          img.auto(src="@/assets/curso/tema3/reserva2.png" width="92" height="92")
          p.fw-bold.ms-4 Control de disponibilidad de habitaciones por medio del rack.
        .d-flex.align-items-center.my-2
          img.auto(src="@/assets/curso/tema3/reserva3.png" width="92" height="92")
          p.fw-bold.ms-4 Determinar la disponibilidad de fecha, hora y tarifas.
        .d-flex.align-items-center.my-2
          img.auto(src="@/assets/curso/tema3/reserva4.png" width="92" height="92")
          p.fw-bold.ms-4 Toma de reserva manual o mediante software.
        .d-flex.align-items-center.my-2
          img.auto(src="@/assets/curso/tema3/reserva5.png" width="92" height="92")
          p.fw-bold.ms-4 Archivar y documentar la reserva.

    h2.h3#t_3_7 3.7 Control de disponibilidad
    p Consiste en comprobar una vez que se recibe una solicitud de reserva, las posibilidades para garantizar su aceptación. Este control se realiza mediante la consulta de los medios que se disponga para ello, manualmente se realizará a partir del  planning de reservas.

    p El planning se define como la representación gráfica del estado de reserva y disponibilidad del establecimiento hotelero, por tanto, debe facilitar la cantidad de habitaciones libres y ocupadas para cada tipo y  fechas específicas. Así mismo, debe reflejar información acerca del estado de los cupos y habitaciones bloqueadas.

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
