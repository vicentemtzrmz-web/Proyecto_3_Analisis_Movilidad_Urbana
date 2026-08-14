# Proyecto_3_Analisis_Movilidad_Urbana
**Descripción:** Se realizó un análisis que nos permitía conocer si la movilidad urbana en Latinoamérica influenciaba la productividad económica. Se trabajo con 2 Datasets [TomTom Traffic Index y OECD Cities] con mas de 1M entradas. 

**Titulo:** Detección de patrones y performance por región, para la toma de decisiones. 

- **Desafío:** El cliente no podía confirmar si había alguna relación entre el desempeño económico y la eficiencia del transporte.
  
- **Proceso:**  Se trabajo con 2 datasets distintos uno con mas de 1M entradas donde cada fila representaba un escaneo del equipo utilizado para medir la contaminación. El segundo dataset nos mostraba el desempeño económico de distintas ciudades latinoamericanas. Primero empecé limpiando los datos, asegurándome de que estos tenían el formato indicado. Además de hacer una estandarización de columnas para facilitar el JOIN. Ya con las columnas renombradas y estandarizadas procedimos a filtrar el dataset para solo trabajar con el Año 2024. Por esto se aseguró que la fecha se mostrara en el formato correcto. A medida que avanzaba, noté que había valores nulos y también algunos sentinels que estaban afectando el análisis. Para evitar errores se reemplazo los sentinels haciendo una imputacion de la media, ya que era la que menos afectaba el análisis. A su vez se hizo un promedio del tiempo que se perdia en el trafico de la ciudad, para confirmar si esto tenia relación directa con el desempeño económico. Ya con los datos limpios y estandarizados se hizo un Inner Join para solo mantener los datos relevantes. Con los promedios verificados y el PIB de las ciudades pudimos graficar los resultados para una fácil digestión de los datos.

- **Metodología:** La limpieza comenzó con la estandarización de columnas: se renombraron campos para facilitar la unión de tablas a medida que avanzaba el análisis, y se estandarizaron los tipos de datos para garantizar un análisis coherente y libre de errores. Se filtró la información por año y se agrupó por ciudad para obtener un análisis específico. Posteriormente, se utilizó un **inner join** para integrar los datos de tráfico y economía que compartían año y ciudad, asegurando resultados más precisos y comparables.

**Insights:**
Las visualizaciones permitieron interpretar los hallazgos de forma más clara:
- La distribución del PIB se concentra principalmente entre **10,000 y 15,000**.
- Los *outliers* son más notorios en los datos de tráfico, probablemente asociados a ciudades con alta congestión y tiempos de traslado elevados.
- Los valores altos de PIB pueden explicarse por múltiples factores subyacentes, como la inversión y el gasto público.
- Se hizo la recomendación de hacer inversiones fuertes en movilidad en las ciudades que mostraban mayor tiempo en el trafico, para verificar si lo encontrado era correcto.


- **Resultado:** Se logró comprobar con ejemplos verídicos como una movilidad urbana no solo generaba trafico y retrasos, sino que tenia un impacto directo en la productividad económica.
