# Análisis de Comportamiento de Clientes: ConnectaTel 📊

##  Objetivo del Proyecto
El objetivo principal de este proyecto es actuar como **Analista de Datos** para la empresa de telecomunicaciones **ConnectaTel**. Se busca evaluar el comportamiento de los clientes (con datos registrados hasta el año 2024) para identificar patrones de consumo, detectar comportamientos atípicos (outliers) y crear segmentos de clientes que permitan diseñar estrategias de retención y mejoras en la oferta comercial.

##  Datasets Utilizados
Para este análisis se utilizaron tres archivos principales:
- **`plans.csv`**: Información de los planes actuales (precios, minutos incluidos, mensajes, GB y costos extra).
- **`users.csv`**: Datos demográficos de los clientes (edad, ciudad, fecha de registro, plan contratado y estatus de cancelación).
- **`usage.csv`**: Detalle del uso real de los servicios (llamadas realizadas, duración y mensajes enviados).

## Etapas del Análisis
El análisis se dividió en las siguientes fases:
1.  **Exploración y Limpieza de Datos**: Identificación de valores nulos, corrección de tipos de datos y tratamiento de valores atípicos (como edades inconsistentes).
2.  **Ingeniería de Características**: Consolidación de datos de uso por usuario para calcular métricas mensuales de consumo.
3.  **Análisis de Outliers**: Aplicación del método de **Rango Intercuartílico (IQR)** para detectar usuarios con consumos extremos y decidir su tratamiento para el negocio.
4.  **Segmentación de Clientes**: Creación de nuevas categorías basadas en lógica condicional (Edad y Nivel de Uso) utilizando funciones personalizadas y el método `.apply()`.
5.  **Visualización**: Generación de histogramas, boxplots y countplots con **Seaborn** para validar las hipótesis de negocio.
6.  **Análisis Ejecutivo**: Traducción de los hallazgos técnicos en recomendaciones estratégicas para los stakeholders.

##  Cómo ejecutar el notebook
Este proyecto fue desarrollado en un entorno de Jupyter Notebook. Puedes ejecutarlo de la siguiente manera:

### 1. Google Colab (Recomendado)
- Abre [Google Colab](https://colab.research.google.com/).
- Sube el archivo `.ipynb` de este repositorio.
- Asegúrate de subir los archivos `.csv` a la sección de archivos del entorno de ejecución antes de correr las celdas.
