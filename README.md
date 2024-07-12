# Proyecto Ecommerce

## Glosario del Proyecto

**Ventas brutas**: Es el total facturado sin restar ni excluir ningún gasto.

- Fórmula en este proyecto: `SUM(price_usd * items_purchased)`

**Margen de ganancia sobre ventas (ventas netas)**: Indica la rentabilidad de un producto, servicio o negocio. Es expresado en porcentaje; mientras más alto sea el número, más rentable es el negocio. Se calcula como la diferencia entre las ventas de un producto y su costo.

- Fórmula en este proyecto: `SUM((price_usd - cogs_usd) * items_purchased) / SUM(price_usd * items_purchased)`

**Margen Absoluto**: Es el margen en términos monetarios, no en porcentaje.

- Fórmula en este proyecto: `SUM((price_usd - cogs_usd) * items_purchased)`

**Campañas**: Conjunto de anuncios o anuncio para un período de tiempo determinado (Ejemplo: campaña de Black Friday, campaña de Navidad).

**Ads o anuncios**: Publicidad en marketing digital que se crea en internet.

**Sesiones**: La cantidad de veces que se ingresa a una página web, sin importar el usuario.

## El Cliente

Te han contratado para la empresa de ecommerce online llamada “ositofeliz” que se dedica a vender ositos de peluche super atractivos. Actualmente, cuenta con 4 modelos de peluches.

## El Problema

Como miembro del equipo de la startup, te va a tocar trabajar con el CEO, el director de marketing y el Gerente de la web para analizar ciertas métricas que queremos medir.

Tu objetivo será analizar la situación actual de la empresa, medir la conversión de la web y usar datos para entender las ventas e impacto de los productos.

## Esquema de Relaciones

![Esquema de relaciones](https://raw.githubusercontent.com/marinarmos/marinaramos.github.io/main/osito%20feliz%20diagrama.png)

## Crear Base de Datos y Tablas

### Los Datos

Base de datos `.sql`:
- [Descargar base de datos](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/0c278049-c263-4752-9517-f0893880a27d/osito_feliz.7z)

### Análisis Previo

Antes de comenzar a responder a las preguntas de negocio que se nos solicita, debemos entender las tablas, cómo están compuestas y cómo se relacionan.

#### Puntos Detectados:

- Rango de tiempo de la tabla de pedidos.
- Cada pedido de la tabla de pedidos tiene más de 1 elemento, por eso se relaciona con la tabla `order_item`.
- Entendemos que se relaciona con la tabla `items_purchase`.

## Ejecución

### Análisis de Ventas

1. Queremos saber cuáles son las ventas por año y por mes en términos brutos y luego el margen absoluto.

2. ¿Cuáles son las ventas brutas medias de cada mes y año? Devuelve los TOP 3. ¿Qué puedes observar?

3. ¿Cuál es el producto que más vende en términos monetarios (Ventas brutas)?

4. ¿Cuál es el producto que deja más margen en términos monetarios?

5. ¿Podemos saber cuál es la fecha de lanzamiento de cada producto?

### Análisis de Tráfico Web

8. ¿Cuáles son los ads (anuncios) o contenidos que han atraído más sesiones?

9. ¿Es lo mismo sesiones que usuarios? ¿Cuál es la cantidad de usuarios individuales?

10. ¿Y por source o fuente? Cantidad de usuarios únicos y sesiones?

11. ¿Cuáles son las sources o fuentes que han dado más ventas?

12. ¿Cuáles son los meses que han atraído más tráfico?

13. Ya que vimos el mes que ha tenido más tráfico, ¿podrías ver de ese mes la cantidad de sesiones que han venido por móvil y la cantidad que han venido por ordenador?

14. ¿Qué campañas son las que han dado más margen por productos?


## Solución

### Conclusiones del Proyecto Ecommerce

1. **Ventas por Año y Mes en Términos Brutos y Margen Absoluto**:
   - Las ventas brutas y el margen absoluto aumentan significativamente durante los meses festivos, como noviembre y diciembre, indicando una tendencia estacional en las ventas.

2. **Ventas Brutas Medias de Cada Mes y Año, TOP 10**:
   - Los meses con mayores ventas brutas medias tienden a ser los últimos meses del año, lo que confirma la tendencia estacional. Los picos en las ventas promedio se deben a promociones y campañas de marketing intensivas durante estos meses.

3. **Producto que Más Vende en Términos Monetarios**:
   - El producto "Osito Cariñoso" es el que genera más ingresos, lo que indica su popularidad entre los clientes. Esto sugiere que la empresa debe continuar enfocándose en este producto.

4. **Producto que Deja Más Margen en Términos Monetarios**:
   - "Osito Amor Por Siempre" es el producto con el mayor margen de ganancia, lo que sugiere que este producto es altamente rentable. Promocionarlo más intensamente podría aumentar la rentabilidad general.

5. **Fecha de Lanzamiento de Cada Producto**:
   - Las fechas de lanzamiento de los productos pueden correlacionarse con los picos de ventas, proporcionando información útil para planificar futuros lanzamientos de productos.

6. **Ventas Netas por Año y Margen por Producto**:
   - Las ventas netas y los márgenes de cada producto se mantienen constantes o aumentan, lo que indica un desempeño saludable de los productos a lo largo del tiempo.

7. **Meses con Ventas Brutas Más Fuertes**:
   - Los meses con mayores ventas brutas son noviembre y diciembre, lo que sugiere que las campañas de marketing durante estos meses son efectivas.

8. **Ads o Contenidos que Atraen Más Sesiones**:
   - Los anuncios relacionados con promociones especiales atraen más sesiones, lo que indica que las campañas publicitarias específicas son más efectivas en atraer tráfico.

9. **Diferencia entre Sesiones y Usuarios**:
   - Hay una alta recurrencia de usuarios, lo que sugiere que los visitantes están interesados en regresar al sitio web.

10. **Source o Fuente de Usuarios y Sesiones**:
    - La mayoría del tráfico proviene de Google, lo que sugiere que las estrategias de SEO y SEM son efectivas.

11. **Sources o Fuentes que Generan Más Ventas**:
    - Google no solo trae más tráfico, sino que también genera más ventas, indicando la efectividad de este canal.

12. **Meses que Atraen Más Tráfico**:
    - Los meses de mayor tráfico son noviembre y diciembre, coincidiendo con las campañas de ventas y festividades.

13. **Dispositivos que Atraen Más Sesiones en el Mes con Más Tráfico**:
    - La mayoría de las sesiones provienen de dispositivos móviles, lo que indica que el sitio web está bien optimizado para usuarios móviles.

14. **Campañas que Generan Más Margen por Productos**:
    - Las campañas en redes sociales que se enfocan en los productos más rentables generan el mayor margen, lo que sugiere que estas campañas son las más efectivas.
