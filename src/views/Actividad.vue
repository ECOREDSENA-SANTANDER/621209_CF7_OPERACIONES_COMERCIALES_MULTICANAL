<template lang="pug">
  .curso-main-container.pb-3
    BannerInterno(icono="far fa-question-circle" titulo="Actividad didáctica")
    .container.tarjeta.tarjeta--blanca.p-4.p-md-5
      // Para cuestionario usar: ActividadController(:cuestionario="cuestionario") 
      // Para parrafo usar: ActividadController(:parrafo="parrafo")
      ActividadController(:cuestionario="cuestionario")
  </template>

<script>
import ActividadController from '@ecored-sena/base-kit/plugin/components/actividad/ActividadController.vue'

export default {
  name: 'ActividadDidactica',
  components: {
    ActividadController,
  },
  data: () => ({
    cuestionario: {
      tema: 'Cuestionario: exhibición y vitrinismo en el formato comercial. ',
      titulo: 'Cuestionario',
      introduccion:
        '<b> Objetivo:</b> verificar la comprensión de los conceptos fundamentales relacionados con el <i>retail</i>, el establecimiento comercial, la arquitectura del punto de venta, el surtido, el planograma, el <i>layout</i>, la exhibición de productos, el vitrinismo, el <i>merchandising</i>, la señalización, los dispositivos de seguridad y el mobiliario comercial. ',
      barajarPreguntas: true,
      titulo_aprobado: '¡BUEN TRABAJO!',
      titulo_reprobado: 'VUELVA A INTENTARLO',
      preguntas: [
        {
          id: 1,
          texto:
            'En el contexto del formato comercial, el <i>retail</i> se entiende principalmente como:',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Un proceso exclusivo de fabricación industrial.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Un sistema de venta al detalle que entrega el producto directamente al cliente.',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto: 'Una técnica contable para registrar inventarios.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Un documento legal de compra y venta.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 2,
          texto:
            'Para que exista un establecimiento comercial se requieren, entre otros elementos:',
          imagen: require('@/assets/actividad/imagen2.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Espacio físico, productos, vendedores y compradores.',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto: 'Solo bodegas, facturas y transporte.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Únicamente vitrinas y publicidad exterior.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Equipos de seguridad y reportes financieros.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 3,
          texto: 'El escaparate cumple una función estratégica porque:',
          imagen: require('@/assets/actividad/imagen3.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Reemplaza todos los procesos de venta interna.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Sirve únicamente para almacenar mercancía.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Comunica la identidad del establecimiento y atrae al cliente en pocos segundos.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto: 'Impide que el cliente conozca el surtido.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 4,
          texto:
            'La arquitectura interior del establecimiento busca principalmente:',
          imagen: require('@/assets/actividad/imagen4.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Reducir la circulación del cliente.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Crear una circulación lógica y fluida por las secciones del local.',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto: 'Eliminar las zonas calientes del punto de venta.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Ubicar todos los productos cerca de la salida.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 5,
          texto: 'Una zona fría se caracteriza porque:',
          imagen: require('@/assets/actividad/imagen05.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Recibe circulación natural y constante de clientes.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Solo se usa para cajas registradoras.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'No requiere estrategias de ubicación.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto:
                'Tiene poco tránsito y puede activarse con productos de alta rotación o promociones.',
              esCorrecta: true,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 6,
          texto: 'Un local ultraespecializado se diferencia porque:',
          imagen: require('@/assets/actividad/imagen6.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Posee una sola sección con alto nivel de especialización.',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto: 'Ofrece todas las categorías de productos posibles.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'No requiere profundidad en el surtido.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Funciona únicamente como mercado municipal.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 7,
          texto: 'El surtido se refiere a:',
          imagen: require('@/assets/actividad/imagen7.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'La cantidad de cajas existentes en bodega.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'El número de vendedores disponibles en la tienda.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'El conjunto y variedad de productos ofrecidos para la compra del consumidor.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto: 'La señalización de seguridad del establecimiento.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 8,
          texto: 'La coherencia del surtido se logra cuando:',
          imagen: require('@/assets/actividad/imagen8.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Se eligen productos sin analizar el cliente.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Hay equilibrio entre rotación, margen, superficie disponible y necesidades de la clientela.',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto: 'Solo se prioriza la cantidad sobre la variedad.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Todas las referencias tienen el mismo precio.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 9,
          texto:
            'Si un establecimiento ofrece muchas familias de productos y muchas referencias por familia, tiene un surtido:',
          imagen: require('@/assets/actividad/imagen9.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Estrecho y poco profundo.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Estrecho y profundo.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Amplio y poco profundo.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Amplio y profundo.',
              esCorrecta: true,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 10,
          texto: 'Un planograma es útil porque:',
          imagen: require('@/assets/actividad/imagen10.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Diseña la ubicación de artículos, <i>facings</i> y espacios para mejorar exhibición y ventas.',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto: 'Sustituye la necesidad de revisar inventarios.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Elimina la relación entre surtido y lineal.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Impide ajustar la reposición de productos.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 11,
          texto:
            'En un planograma, el término <i>facing</i> hace referencia a:',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'La distancia entre la puerta y la caja.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'El número de caras visibles de un mismo producto para el cliente.',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto: 'El costo de fabricación del artículo.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'La sección fría del establecimiento.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 12,
          texto: 'El <i>layout</i> en <i>retail</i> se relaciona con:',
          imagen: require('@/assets/actividad/imagen2.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'El precio final de un producto.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'La capacitación de los vendedores.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'La disposición estratégica de productos, sectores o categorías en el punto de venta.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto: 'El trámite de devoluciones con proveedores.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 13,
          texto: 'El diseño diagonal de <i>layout</i> se recomienda porque:',
          imagen: require('@/assets/actividad/imagen3.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Mejora la visibilidad para cajeros y clientes y favorece el flujo de tráfico.',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto: 'Es exclusivo para productos congelados.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Impide que el cliente circule libremente.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Siempre es el diseño más económico.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 14,
          texto: 'La exhibición de productos tiene como propósito:',
          imagen: require('@/assets/actividad/imagen4.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Ocultar los artículos de mayor rotación.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Evitar el uso del mobiliario comercial.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Reducir las compras por impulso.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto:
                'Llamar la atención, facilitar y motivar la acción de compra.',
              esCorrecta: true,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 15,
          texto:
            'La exhibición en <i>check out</i> se caracteriza por ubicar productos:',
          imagen: require('@/assets/actividad/imagen05.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'En la zona de almacenamiento.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Cerca de las cajas para estimular compras por impulso.',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto: 'Solo en vitrinas cerradas con llave.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Fuera del establecimiento.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 16,
          texto:
            'El vitrinismo o <i>visual merchandising</i> se entiende como:',
          imagen: require('@/assets/actividad/imagen6.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Un conjunto de técnicas para diseñar vitrinas que atraigan e inviten a comprar.',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto: 'Una norma para codificar productos en bodega.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Un sistema de control de facturas.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Una estrategia para eliminar la comunicación visual.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 17,
          texto: 'El <i>merchandising</i> de seducción se orienta a:',
          imagen: require('@/assets/actividad/imagen7.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Ordenar productos sin considerar la experiencia del cliente.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Definir solo el precio de lanzamiento.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Crear impacto visual y convertir la tienda en una experiencia atractiva.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto: 'Registrar códigos en el sistema de bodegas.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 18,
          texto: 'La señalización comercial contribuye a:',
          imagen: require('@/assets/actividad/imagen8.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Aumentar los puntos ciegos del establecimiento.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Orientar al visitante, facilitar la circulación e informar situaciones de riesgo.',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto: 'Eliminar la identidad visual de la marca.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Sustituir los dispositivos de seguridad.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 19,
          texto: 'Las etiquetas antihurto adhesivas funcionan porque:',
          imagen: require('@/assets/actividad/imagen9.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Activan sensores de alarma ante intentos de robo y se desactivan al comprar.',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto: 'Ocultan el precio del artículo.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Reemplazan completamente la vigilancia del personal.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Solo sirven para productos perecederos.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 20,
          texto:
            'Según el método ABC, los artículos de rotación A deben recibir atención especial porque:',
          imagen: require('@/assets/actividad/imagen10.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Son los menos solicitados por los clientes.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'No requieren control de inventario.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Siempre se ubican en vitrinas cerradas.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto:
                'Tienen alta rotación, aportan gran parte de los ingresos y no deben presentar roturas de <i>stock</i>.',
              esCorrecta: true,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
      ],
      mensaje_final_aprobado: 'Ha superado la actividad.',
      mensaje_final_reprobado:
        'Le recomendamos volver a revisar el componente formativo e intentar nuevamente la actividad didáctica.',
    },
  }),
}
</script>
