## Análisis Exploratorio del Dataset de Automóviles

Este repositorio contiene un análisis exploratorio de datos (EDA) sobre un dataset de automóviles. El objetivo principal es comprender las relaciones entre especificaciones técnicas del vehículo, su rendimiento y su precio, con el fin de descubrir patrones relevantes para la industria automotriz, la toma de decisiones y el aprendizaje de análisis de datos.

---

## Contenido del proyecto

- Carga y previsualización de datos
- Limpieza de columnas innecesarias y tratamiento de valores faltantes
- Análisis exploratorio con visualizaciones detalladas
- Insights técnicos sobre rendimiento, potencia y relación con el tipo de combustible y motor

---

## Dataset utilizado

Se trabajó con el archivo `Automobile_data.csv`, que contiene 26 columnas con información técnica y comercial de automóviles, incluyendo:

Contiene especificaciones varias como typo de motor, cilindraje, dimensiònn de cilindros, rendimiento por revoluciones en ciudad y carreta y caballos de fuerza

---

## Limpieza de datos

Durante el análisis se realizaron las siguientes tareas de limpieza:

- Se eliminaron las columnas `engine-location`, `normalized-losses` y `num-of-doors` por falta de información o redundancia.
- Se convirtieron los valores de `price` a tipo numérico y se eliminaron los registros con precios faltantes (`NaN`).
- Se inspeccionaron otras columnas como `bore`, `stroke` y `peak-rpm` para identificar y manejar valores inconsistentes o ausentes.

Estas acciones fueron necesarias para garantizar la calidad del análisis y evitar sesgos o errores durante las visualizaciones y agrupaciones.

---

## Análisis realizado

### 1. **Autos más caros**
Gráfico de barras que muestra las marcas con los precios más altos.

### 2. **Caballos de fuerza según tipo de combustible**
Un gráfico de violín muestra la distribución del `horsepower` (potencia del motor) en función del `fuel-type`. Permite observar si los autos a gasolina o diésel tienden a tener mayor potencia.

### 3. **Distribución de autos por marca y tipo de combustible**
Gráfico de barras agrupadas que compara cuántos autos a gas o diésel tiene cada marca. Esto permite ver si hay una tendencia por parte de ciertos fabricantes a usar más un tipo de combustible.

### 4. **Distribución de revoluciones por tipo de motor**
Un boxplot compara el `peak-rpm` de los autos según el `engine-type`, ayudando a identificar qué tipo de motor tiende a operar a mayores revoluciones.

### 5. **Relación entre consumo en ciudad y carretera**
Gráfico de dispersión (`scatterplot`) que muestra la correlación entre `city-mpg` y `highway-mpg`, diferenciando por marca. Este análisis permite evaluar la eficiencia de combustible.

---

## Dependencias usadas

El análisis fue realizado con las siguientes bibliotecas de Python:

- `pandas`: Manipulación de datos tabulares
- `matplotlib`: Visualizaciones básicas
- `seaborn`: Gráficos estadísticos avanzados
- `plotly`: Visualizaciones interactivas (opcional, no utilizada directamente en los gráficos mostrados)

---

##  Decisiones que se pueden tomar

A partir del análisis realizado, se pueden tomar decisiones como:

- Evaluar qué marcas producen vehículos con mayor rendimiento por tipo de combustible
- Elegir autos con mejor eficiencia en ciudad o carretera
- Determinar el tipo de motor más eficiente en revoluciones
- Identificar tendencias de diseño y mercado por fabricante

---
