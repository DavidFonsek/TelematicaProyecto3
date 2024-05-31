# Proyecto3
# ST0256 Tópicos Especiales en Telemática

## Estudiante:
- Nombre: David Fonseca Lara
- Correo: dfonsecal@eafit.edu.co

## Profesor:
- Nombre: Álvaro Ospina
- Correo: aeospinas@eafit.edu.co

# Proyecto 3 - Spark con Notebooks y PySpark
Este proyecto se enfoca en el uso de Spark con Notebooks y PySpark. Se hará uso de Google Colab para ejecutar PySpark.
En dataset que se usará es el de [Casos positivos de COVID 19 en Colombia](https://www.datos.gov.co/api/views/gt2j-8ykr/rows.csv?accessType=DOWNLOAD).

## 1. Subiendo los datos en Google Drive
Primero, se sube el archivo Casos_positivos_de_COVID-19_en_Colombia.csv a Google Drive. Este archivo contiene información sobre los casos positivos de COVID-19 en Colombia.
![](./Images/ArchivoDrive.png)
Además subí el acrhivo al colab y cree el dataframe leyéndolo
![](./Images/ArchivoyDF.png)

## 2. Análisis exploratorio de los datos
### 2.1 Listar columnas
![](./Images/2-1.png)

### 2.2 Tipos de datos
![](./Images/2-2.png)

### 2.3 Seleccionar algunas columnas
![](./Images/2-3.png)

### 2.4 Renombrar columnas
![](./Images/2-4.png)

### 2.5 Agregar columna
![](./Images/2-5.png)

### 2.6 Borrar columnas
![](./Images/2-6.png)

### 2.7 Filtrar datos
![](./Images/2-7.png)

### 2.8 Ejecutar una función UDF
![](./Images/2-8.png)

## 3. Preguntas de negocio
Formulamos las preguntas y almacenamos los resultados en un archivo CSV, que luego se guarda en S3.

### 3.1 Los 10 departamentos con más casos de COVID-19 ordenados de mayor a menor
![](./Images/3-1.png)

### 3.2 Las 10 ciudades con más casos de COVID-19 ordenadas de mayor a menor
![](./Images/3-2.png)

### 3.3 Los 10 días con más casos de COVID-19 ordenados de mayor a menor
![](./Images/3-3.png)

### 3.4 Distribución de casos de COVID-19 por edades en Colombia
![](./Images/3-4.png)

### 3.5 Distribución de casos de COVID-19 por departamentos en Colombia
![](./Images/3-5.png)

## 4. Subir archivos a Amazon S3
Hacemos la conexión con el Bucket de AWS
![](./Images/ConexionBucket.png)

Creamos la carpeta en el bucket llamada colab/
![](./Images/Carpeta.png)

Transformé los df a CSV y los subí al bucket
![](./Images/SubiendoArchivosS3.png)

Y verifiqué que hayan quedado en el bucket
![](./Images/ArchivosEnS3.png)

