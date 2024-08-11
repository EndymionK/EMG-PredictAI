# Análisis Exploratorio de Datos (EDA) - Proyecto EMG-PredictAI

## Descripción del Proyecto

Este proyecto se centra en la realización de un Análisis Exploratorio de Datos (EDA) sobre un dataset que contiene actividad electromiográfica registrada en el miembro superior de 40 sujetos sanos. El objetivo es explorar los datos, identificar valores atípicos, analizar la distribución de las variables y las relaciones entre ellas, y generar visualizaciones para comprender mejor la información contenida en el dataset.

El enlace al paper es el siguiente: [Electromyography data for non-invasive naturally-controlled robotic hand prostheses](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4421935/)

- El ejercio de nuestro equipo es el ejercicio D, que corresponde a 9 movimientos básicos de los dedos.
- El dedo que será analizado es el dedo medio
- Las clases a tener en cuenta son: 0,3,5,8

Imagen de las clases:

![Imagen de las clases](https://github.com/EndymionK/EMG-PredictAI/blob/main/Images/Classes_ExerciseD.png)

## Dataset

El dataset utilizado es `Data\E3_database.csv`, que contiene 69 columnas:

- **Columnas [0-2]:** Información general (ID del sujeto, etiqueta del ejercicio, clase del ejercicio).
- **Columnas [3-8]:** Ángulos de posición de los dedos.
- **Columnas [9-68]:** Características extraídas de los 12 electrodos de electromiografía:
  - **Columnas [9-20]:** Mean Absolute Value Slope (MAVs)
  - **Columnas [21-32]:** Root Mean Square (RMS)
  - **Columnas [33-44]:** Zero Crossing (ZC)
  - **Columnas [45-56]:** Slope Sign Change (SSC)
  - **Columnas [57-68]:** Waveform Length (WL)

## Proceso de Análisis

1. **Carga de Datos:** Importación del dataset, visualización de las primeras fila e información general.
2. **Limpieza de Datos:** Identificación y manejo de valores atípicos utilizando Z-Score y visualización de Boxplots.
3. **Análisis de Variables:** Exploración de la distribución de las variables y relaciones entre ellas.
4. **Visualizaciones:** Generación de gráficos para visualizar la información contenida en el dataset.

## Requisitos

Para ejecutar el EDA se debe tener las siguientes librerías instaladas:

numpy
pandas
matplotlib
seaborn
scipy

Para instalar las librerías, se puede utilizar el siguiente comando en la terminal:
    
    ```
    pip install -r requirements.txt
    ```

## Autores

- [Andrés Arroyave Carmona]
- [Andrés Felipe Calvo]
- [Andrés Guillermo Toloza]
