# Proyecto 6: Análisis de ConnectaTel

## Objetivo del proyecto

Analizar el comportamiento de los clientes de ConnectaTel en
Latinoamérica durante 2024, utilizando información de usuarios, planes
contratados y registros de uso. El propósito es identificar patrones de
consumo, segmentos de clientes y oportunidades que permitan mejorar la
oferta comercial y apoyar la toma de decisiones del negocio.

## Datasets utilizados

El análisis utiliza tres conjuntos de datos en formato CSV:

-   **`plans.csv`**: contiene las características de los planes
    disponibles, como cuota mensual, minutos, mensajes y datos
    incluidos, así como los costos por consumo adicional.
-   **`users_latam.csv`**: contiene información de los clientes, como
    edad, ciudad, fecha de registro, plan contratado y fecha de
    cancelación.
-   **`usage.csv`**: contiene los registros de llamadas y mensajes, con
    información de fechas, duración de llamadas y longitud de mensajes.

## Etapas del análisis

1.  **Carga y exploración de datos:** lectura de los archivos, revisión
    de dimensiones, tipos de datos y estructura de los datasets.
2.  **Identificación de problemas de calidad:** detección de valores
    nulos, datos inválidos, valores especiales y fechas fuera del
    periodo esperado.
3.  **Limpieza y preparación:** corrección de valores inválidos,
    conversión de fechas y revisión de valores faltantes. Se conservaron
    los nulos que representan información no aplicable, como la duración
    en registros de mensajes y la longitud en registros de llamadas.
4.  **Integración y agregación:** cálculo de mensajes, llamadas y
    minutos por usuario, y unión de estos resultados con la información
    de clientes.
5.  **Análisis estadístico y visualización:** cálculo de estadísticas
    descriptivas y elaboración de histogramas y diagramas de caja para
    estudiar la distribución del uso y detectar posibles valores
    atípicos.
6.  **Segmentación de clientes:** clasificación por nivel de uso (bajo,
    medio y alto) y por edad (joven, adulto y adulto mayor), seguida de
    visualizaciones de los segmentos.
7.  **Conclusiones y recomendaciones:** elaboración de un análisis
    ejecutivo con los principales hallazgos y oportunidades comerciales
    para ConnectaTel.

## Cómo abrir y ejecutar el notebook

1.  Descarga o clona el repositorio que contiene este README, el
    notebook y los archivos CSV.
2.  Para consultar el notebook sin ejecutarlo, abre el repositorio en
    GitHub y selecciona el archivo `.ipynb`. GitHub muestra una vista
    del notebook.
3.  Para ejecutar las celdas, abre el notebook en un entorno compatible
    con Jupyter, como Jupyter Notebook, JupyterLab o Google Colab.
4.  Asegúrate de que los tres archivos CSV estén disponibles en la ruta
    que utiliza el notebook. Si es necesario, ajusta las rutas de
    lectura.
5.  Ejecuta las celdas en orden, desde la carga de librerías y datasets
    hasta las visualizaciones y conclusiones.

## Guía breve para reproducir el análisis

-   Utiliza Python 3 y las librerías `pandas`, `numpy`, `seaborn` y
    `matplotlib`.
-   Coloca `plans.csv`, `users_latam.csv` y `usage.csv` en la carpeta
    esperada por el notebook o actualiza sus rutas.
-   Ejecuta todas las celdas en orden para reproducir la exploración,
    limpieza, integración, análisis estadístico, visualizaciones y
    segmentación.
-   Revisa los resultados de las celdas de salida, ya que las cantidades
    y estadísticas presentadas en las conclusiones dependen de los datos
    procesados.
-   Conserva los registros atípicos identificados en este análisis, pues
    no se encontró evidencia suficiente para considerarlos errores;
    deben interpretarse como posibles patrones reales de consumo.

## Resultado esperado

Al finalizar, se obtiene una base de usuarios enriquecida con métricas
de consumo y segmentos por edad y nivel de uso, además de
visualizaciones y conclusiones que ayudan a identificar oportunidades
para adaptar los planes, fortalecer la fidelización y mejorar la
estrategia comercial de ConnectaTel.
