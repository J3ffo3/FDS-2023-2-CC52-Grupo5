## CC216-Fundamentos de Data Science
# TRABAJO FINAL
### 2023-02

## **Objetivo del proyecto**

El objetivo principal es dar respuesta a cuatro tipos de requerimientos los cuales cuentan con una cierta cantidad de preguntas y de esa manera sacar conclusiones con buen fundamento a raíz de los datos analizados.

## Por Categoría de Videos
1. ¿Qué categorías de videos son las de mayor tendencia?
2. ¿Qué categorías de videos son los que más gustan? ¿Y las que menos gustan?
3. ¿Qué categorías de videos tienen la mejor proporción (ratio) de “Me gusta” / “No megusta”?
4. ¿Qué categorías de videos tienen la mejor proporción (ratio) de “Vistas” /“Comentarios”?

## Por el tiempo transcurrido
5. ¿Cómo ha cambiado el volumen de los videos en tendencia a lo largo del tiempo?

## Por Canales de YouTube
6. ¿Qué Canales de YouTube son tendencia más frecuentemente? ¿Y cuáles con menos frecuencia?

## Por la geografía del país
7. ¿En qué Estados se presenta el mayor número de “Vistas”, “Me gusta” y “No me gusta”?

## Adicionalmente, al cliente le gustaría conocer si:
8. ¿Es factible predecir el número de “Vistas” o “Me gusta” o “No me gusta”?
9. ¿Los videos en tendencia son los que mayor cantidad de comentarios positivos reciben?

## **Integrantes**
- U20191e742 Alcalde Gonzalez Renato Alberto
- U202017033 Datto Aponte Antonio Francisco
- U202124269 Diaz Villanueva Jeffrey Ulises

## **Descripción del Conjunto de Datos**
- video_id: id del video
- trending_date: día en que el video se hizo viral
- title: título del vídeo
- channel_title: nombre del canal que subio el video
- category_id: categoría del video
- publish_time: fecha de publicación
- tags: tags que el usuario le puso al video
- views: número de visualizaciones
- likes: número de likes
- dislikes: número de dislikes
- state: nombre del Estado perteneciente al país (incorporado de forma aleatoria).
- lat: latitud geográfica de ubicación del Estado. 
- lon: longitud geográfica de ubicación del Estado.
- geometry: registra las coordenadas de las geometrías donde su ubica el Estado dentro del planeta. Es de utilidad si se decide utilizar la librería GeoPandas para la elaboración de mapas.

## **Conclusiones**
- Se concluyó que de las tres variables solicitadas, según los resultados de las validaciones de los modelos utilizados, es más factible predecir el número de “dislikes” que tendría un video.
- Con respecto a la metodología crisp-dm nos ha ayudado a trabajar de manera ordenada. ciertamente pudimos haber estudiado un poco más los datos y crear nuevas columnas a raíz de las que ya se disponían en el dataframe.
- La exploración detallada de los datos reveló patrones interesantes, como las categorías de vídeo más populares, la distribución geográfica de las métricas y la evolución temporal de las tendencias en YouTube. - Este análisis proporcionó información valiosa para alcanzar los objetivos del proyecto.
- La correcta preparación y limpieza de los datos fue esencial para garantizar la calidad de los resultados. Se abordaron los valores nulos y los valores atípicos y se introdujeron modificaciones para mejorar la precisión de los modelos predictivos.
- Se identificaron las categorías de vídeos más populares y se analizaron las tendencias a lo largo del tiempo. Además, se evaluaron los canales de YouTube más y menos populares, lo que permitió conocer en profundidad la plataforma.
- El análisis geográfico reveló la distribución de métricas como visionados, "me gusta" y "no me gusta" en los distintos estados. Esto proporciona una visión única de cómo varían geográficamente las preferencias y reacciones.
- La elección de un modelo de regresión lineal simple para predecir parámetros específicos se basó en la naturaleza de los datos. Sin embargo, los resultados de la evaluación (MAE, MSE, RMSE) indican la necesidad de considerar enfoques más avanzados o características adicionales para mejorar la precisión.
- La interpretación del modelo de regresión produjo coeficientes para aversiones, gustos y comentarios frente a vistas. Estos coeficientes proporcionan información sobre cómo un cambio en cada métrica afecta a las visualizaciones de un vídeo.
- A pesar de los resultados, reconocemos que el análisis puede mejorarse mediante un análisis más profundo de los datos y la creación de nuevas columnas derivadas. Además, podría ser útil explorar modelos más avanzados y recursos adicionales.
- Existe una correlación positiva entre el número de vídeos sobrevalorados y el número de comentarios positivos, con cierta variación mensual. Es importante señalar que la correlación no implica causalidad y que otros factores pueden influir en los resultados.

## **Licencia de Uso**
Este trabajo está bajo la Licencia MIT.
