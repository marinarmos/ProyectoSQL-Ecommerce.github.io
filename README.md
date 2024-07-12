# marinaramos.github.io
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
https://github.com/marinarmos/marinaramos.github.io/blob/main/osito%20feliz%20diagrama.png

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

(Colocar aquí las soluciones o análisis detallados)
