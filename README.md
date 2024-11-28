# Análisis de Datos de Tiros en Baloncesto: Mejorando el Rendimiento de Jugadores Universitarios

### Objetivos

- 🗺️ Explorar: Identificar la distancia desde el aro en la que cada jugador tiene mayor probabilidad de anotar un tiro, utilizando los datos disponibles.
- 📊 Visualizar: Generar gráficos que muestren las posiciones de los tiros en la cancha, diferenciando entre los resultados (acierto/fallo) y los cuatro jugadores analizados.
- 🔎 Analizar: Evaluar si existe una relación directa entre la proximidad al aro y la probabilidad de anotar un tiro, basada en los patrones identificados en los datos.

---

### Contexto

Un equipo de baloncesto universitario busca aprovechar el análisis de datos para optimizar el desempeño de sus jugadores. Como proyecto inicial, se han proporcionado datos históricos de tiros en la NBA correspondientes a cuatro jugadores específicos. El objetivo es determinar si estos datos pueden ofrecer recomendaciones personalizadas sobre las áreas de mayor efectividad en la cancha para cada jugador.

El entrenador plantea una pregunta clave:
> ¿Es posible generar estrategias basadas en datos para aumentar la probabilidad de éxito en los tiros de cada jugador?

---

## Metodologia

### Datos

El *dataset* esta disponible [aqui](https://kaggle.com/datasets/163acec12e8bdb031c78f4912406ee3e68e3a423529469b4d07a0637c0f96bfc). Contamos con una cantidad de **776** registros para su analisis acerca de los jugadores **Chris Paul, Russell Westbrook, Seth Curry,Trae Young**.El dataset utilizado está disponible aquí e incluye 776 registros correspondientes a los siguientes jugadores:

- Chris Paul
- Russell Westbrook
- Seth Curry
- Trae Young

### Diccionario de datos

|variable|clase|descripción|
|---|---|---|
|SHOOTER|String|Nombre del jugador que realiza el tiro|
|X|float|Distancia horizontal del tiro realizado desde el aro en pies|
|Y|float|Distancia vertical del tiro realizado desde el aro en pies|
|RANGE|String|Rango de radio del tiro realizado desde el aro en pies|
|DEFENDER|String|Nombre del jugador que defiende el tiro|
|SCORE|String|'MADE' si el tiro es anotado, de lo contrario 'MISSED'|


### Procesamiento

Un análisis inicial reveló que el conjunto de datos no presentaba valores faltantes ni inconsistencias. Por lo tanto, no fue necesario realizar una limpieza extensiva. Los pasos clave incluyeron:

1. **Revisión exploratoria**: Inspección de la distribución de las variables y detección de posibles anomalías.
2. **Verificación de calidad**: Confirmación de que los datos eran consistentes y adecuados para el análisis.

### Tools 

- Python: Versión 3.12
- Conda: 24.9.2 (gestión de entornos)
- Plotly: 5.24.1 (visualización interactiva)
- Scipy: 1.14.1 (análisis estadístico)
- Pandas: 2.2.2 (procesamiento y manipulación de datos)
- Numpy: 1.26.4 (cálculos numéricos)
