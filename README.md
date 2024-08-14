# S3DataPipeline - Consumo de Agua en CDMX

## Descripción

Este proyecto es un pipeline ETL (Extracción, Transformación y Carga) diseñado para procesar datos de consumo de agua en la Ciudad de México. El objetivo es explicar el consumo de agua por delegación y zona, utilizando datos extraídos de la plataforma de [Datos Abiertos CDMX](https://datos.cdmx.gob.mx/dataset/consumo-agua). Los datos se procesan para estandarizar nombres de columnas, permitir ajustes en la granularidad (anual, semestral, mensual), y se cargan en un bucket de S3 en AWS. Estos datos son posteriormente utilizados en un dashboard en Python para análisis y visualización.

## Estructura del Proyecto

El proyecto se divide en tres partes principales:

1. **Planeación del Pipeline**
   - Diseño del flujo de datos desde la extracción hasta la carga en S3.
   - Definición de las transformaciones necesarias para cumplir con los requisitos del cliente.

2. **Extracción y Carga de Datos**
   - Obtención de los datos desde Datos Abiertos CDMX.
   - Almacenamiento de los datos en un bucket de S3 en AWS.

3. **Transformación de Datos**
   - Estandarización de los nombres de columnas (todo en minúsculas, sin espacios ni caracteres especiales).
   - Ajustes en la granularidad de los datos según las necesidades del cliente (anual, semestral, mensual).

## Requisitos

- **Python 3.x**
- **AWS SDK (boto3)**
- **Pandas**
- **Requests**
- **Jupyter Notebook**

## Instalación

1. Clonar el repositorio:

   ```bash
   git clone https://github.com/tu-usuario/S3DataPipeline.git

## Uso

1. Abre el Jupyter Notebook:

   ```bash
   jupyter notebook
