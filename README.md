Telecom X: Proyecto de Análisis de Churn (ETL)
Este proyecto forma parte del desafío de Oracle Next Education. Como analista de datos en formación, mi objetivo fue realizar un proceso completo de ETL (Extract, Transform, Load) sobre los datos de una empresa de telecomunicaciones para identificar las causas de la evasión de clientes (Churn).

Objetivo del Proyecto
Extraer, limpiar y transformar datos provenientes de una API (simulada mediante un archivo JSON) para entregar un dataset optimizado al equipo de Ciencia de Datos, permitiendo el desarrollo de modelos predictivos precisos.

Tecnologías Utilizadas
Lenguaje: Python 3.x

Librerías: * Pandas: Manipulación y limpieza de datos.

JSON/Requests: Extracción de datos.

Matplotlib & Seaborn: Visualización exploratoria.

Proceso Realizado
1. Extracción (Extract)
Se realizó la lectura de los datos en formato JSON. Dado que la información venía con estructuras anidadas (objetos dentro de objetos), se utilizó la técnica de aplanamiento de datos (json_normalize) para llevar la información a un formato tabular (Filas y Columnas).

2. Transformación (Transform)
En esta etapa de "limpieza profunda" se realizaron las siguientes acciones:

Renombrado de columnas: Eliminación de prefijos innecesarios para mejorar la legibilidad.

Corrección de tipos de datos: Conversión de la columna TotalCharges de texto a numérico.

Tratamiento de Nulos: Gestión de valores faltantes y eliminación de registros sin etiqueta de Churn.

Estandarización: Mapeo de valores binarios para mantener la consistencia en el dataset.

3. Carga y Análisis (Load)
Exportación: El dataset final se guardó en un archivo TelecomX_Clean_Data.csv.

Análisis Exploratorio (EDA): Se crearon visualizaciones clave que muestran la relación entre el tipo de contrato, los cargos mensuales y la probabilidad de fuga del cliente.

Hallazgos Clave
Los clientes con contratos mes a mes tienen una tasa de evasión significativamente mayor.

Existe una correlación directa entre altos cargos mensuales y la decisión de abandonar el servicio.
