# Proyecto Final Módulo 3

## Análisis de ventas

En este proyecto trabajé con una data de ventas. Primero tuve que revisar los datos, arreglar algunos errores y después hacer los análisis y los gráficos.

La idea de este proyecto fue practicar lo que aprendí en el módulo usando Python y pandas.

## Limpieza de la data

Primero revisé la data para ver si tenía valores vacíos, datos repetidos o algún otro problema.

Encontré datos vacíos en las columnas descuento y género. En descuento puse 0 porque entendí que esas ventas no tenían descuento. En género puse "No especificado" para no borrar la venta completa.

También encontré algunos id repetidos. Los eliminé porque cada venta debe tener un id diferente.

Después convertí las fechas a su formato correcto y también las cantidades, precios, descuentos y edades a datos numéricos.

Organicé los textos para quitar espacios de más y para que los nombres tuvieran un mismo formato.

También revisé que los precios y las cantidades fueran mayores que cero y que los descuentos estuvieran entre 0 y 1.

## Transformación

Después de limpiar la data creé la venta bruta y la venta neta.

La venta bruta la saqué multiplicando la cantidad por el precio del producto. Para la venta neta tomé en cuenta el descuento de cada venta.

También saqué el mes y el trimestre de cada fecha.

Luego clasifiqué las ventas como bajas, medias y altas usando pd.cut().

También hice una tabla con metas para cada región y la uní con la data principal usando merge().

## Análisis

Para analizar las ventas utilicé groupby() y agg().

Las preguntas que quise responder fueron:

1. ¿Cuál región vendió más?
2. ¿Cuál categoría generó más dinero?
3. ¿Cuál vendedor tuvo mejores resultados?

## Resultados

La región Norte fue la que más vendió con RD$516,875.00. La región Este fue la que tuvo el total más bajo con RD$271,743.00.

La categoría Electrónica fue la que más dinero generó con RD$760,915.00. Alimentación fue la que menos generó con RD$79,063.00.

Ana Garcia fue la vendedora con el total de ventas más alto, llegando a RD$516,875.00. Su promedio fue de RD$25,843.75 por venta. Después quedó Luis Soto con RD$319,947.50.

## Gráficos

Hice cuatro gráficos para poder ver mejor los resultados:

* Un gráfico de barras con las ventas por región.
* Un gráfico de línea con las ventas por mes.
* Un histograma de las ventas netas.
* Un gráfico de dispersión para comparar el precio con la venta neta.

Todos los gráficos tienen título y los nombres de los ejes. También utilicé RD$ para representar el dinero y guardé los gráficos como imágenes PNG.

## Conclusión

Con este proyecto pude practicar mejor cómo trabajar con una data usando Python.

Algo que aprendí fue que antes de comenzar a analizar hay que revisar bien los datos, porque pueden aparecer valores vacíos, repetidos o datos que no estén en el formato correcto.

Después de organizar la data fue más fácil sacar los resultados y hacer los gráficos. Los gráficos también me ayudaron a entender mejor cuáles regiones, categorías y vendedores tuvieron las ventas más altas.
