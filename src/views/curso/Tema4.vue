<template lang="pug">
.curso-main-container.pb-3
  BannerInterno(titulo="4. Estructura organizacional.")
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5
    p La misión del hotel es garantizar un servicio de alojamiento personalizado con calidad, comodidad y seguridad en un entorno confortable, siempre con el objetivo del bienestar y la satisfacción de las necesidades de los huéspedes.

    p Por tal razón se requiere de una estructura que permita lograr el objetivo. La estructura organizacional es el modo en que una empresa planifica y distribuye su trabajo, cada empresa tiene su propia estructura.

    figure.mb-5
      img(src="@/assets/curso/tema4/tema4-main.png")

    p Los hoteles se estructuran con la sectorización de las labores en distintas unidades llamadas departamentos. Cada departamento atiende un conjunto específico de necesidades del cliente.

    p La representación gráfica de <strong>la estructura organizacional de una empresa se conoce como organigrama,</strong> no existe un organigrama que indique la distribución de los departamentos, y que sea válido para todos los hoteles, ya que esto depende de la capacidad y la categoría del hotel, de las características físicas de la edificación, del tipo de organización y de servicio que se desea proporcionar. También se presentan organigramas para áreas específicas.

    .tarjeta.bg-amarillo.p-3.mb-5
      .row.justify-content-around.align-items-center
        .col
          .row.justify-content-between.align-items-center
            .col-5.mb-3.mb-sm-0.px-5
              .h5.mb-0 Aquí encontraras los tres ejemplos de modelos de estructura de organigrama.
            .col-sm-auto
              a.boton.boton--color-sistema-a(href="/downloads/modelos.pdf" target="_blank")
                strong Descargar aqui

    p Gráficamente en general se presenta de la siguiente forma:

    p Los puestos de trabajo y los procesos están sometidos a una reglamentación y estandarización los cuales son respaldados por manuales de funciones y procesos:

    .row.justify-content-between.mt-5.align-items-end
      .col-12.col-md-6
        p <strong>Manual de funciones:</strong> es un instrumento de trabajo que contiene el conjunto de normas y tareas que desarrolla cada funcionario en sus actividades cotidianas y es elaborado técnicamente basados en los respectivos procedimientos, sistemas y normas del establecimiento.

        p <strong>Son guías y orientaciones para desarrollar las rutinas o labores cotidianas de cada uno de los trabajadores</strong> quienes podrán tomar las decisiones más acertadas apoyadas por las directrices de los superiores, y estableciendo con claridad la responsabilidad y las obligaciones que cada uno de los cargos conlleva.

        .row.bg-amarillo-claro.p-4 Incluye brevemente cada una de las funciones y responsabilidades básicas describiendo adecuadamente los límites y la esencia del cargo.

      .col-12.col-md-5
        img(src="@/assets/curso/tema4/funcion-1.png")
    .row.justify-content-between.mt-5.align-items-end
      .col-12.col-md-5
        img(src="@/assets/curso/tema4/funcion-2.png")
      .col-12.col-md-6
        p <strong>Manual de procedimientos:</strong> el manual de procedimientos es <strong><i>"un instrumento de apoyo en el que se encuentran de manera sistemática los pasos a seguir, para ejecutar las actividades de un puesto determinado y/o funciones de la unidad administrativa".</i></strong> (Gómez, 2001).

        p Se puede decir entonces que es un documento de apoyo para el personal de una empresa, el cual contiene políticas y detalles de las actividades a realizarse en funciones específicas.
    .row.justify-content-between.mt-5.align-items-end
      .col-12.col-md-6
        p <strong>Formatos:</strong>  el formato es el conjunto de las características técnicas y de presentación de un texto, objeto o documento en distintos ámbitos, tanto reales como virtuales.

        p Sirven para:

        ul.ms-4
          li El control y mantenimiento de los servicios que se prestan.
          li Apoyan a controlar la calidad y resultado que se ofrece en el establecimiento.
          li Para planificar, controlar y evaluar el trabajo.
          li Para la garantía de la eficiencia del servicio.
          li Optimización de la prestación del servicio.

      .col-12.col-md-5
        img(src="@/assets/curso/tema4/funcion-3.png")

    .tarjeta.bg-amarillo.p-3.mb-5.my-5
      .row.justify-content-around.align-items-center
        .col
          .row.justify-content-between.align-items-center
            .col-sm-auto.px-5
              img.auto(src="@/assets/curso/tema3/importante.png")
            .col.mb-3.mb-sm-0.px-5
              .h4.mb-0 <strong>En el establecimiento hotelero se utilizan para todas las áreas cada uno con su fin, algunos son comunes a todas las áreas: ejemplo: “Lista de huéspedes”</strong>

</template>

<script>
import BannerInterno from '../../components/plantilla/BannerInterno'
export default {
  name: 'Tema4',
  components: {
    BannerInterno,
  },
}
</script>
