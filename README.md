# SRF - Separador de Registros Multilinea en Excel

SRF es una herramienta diseñada para detectar y transformar registros de Excel que contienen multiples lineas en una misma celda, generando un registro limpio por cada valor separado. Ideal para preparar datos antes de cargas masivas a bases de datos o sistemas de integracion.

## Objetivo

Automatizar la limpieza y normalizacion de archivos Excel que presentan problemas de lectura por saltos de linea internos, especialmente en tablas como REL_DIM.

## Tecnologias y Herramientas Utilizadas

- Lenguaje principal: Python
- Entorno de desarrollo: Google Colab
- Procesamiento de Excel: pandas, openpyxl
- Carga de archivos: Google Colab files.upload
- Exportacion final: Excel .xlsx

## Instalacion y Ejecucion

1. Abrir Google Colab: https://colab.research.google.com
2. Crear un nuevo cuaderno o subir el notebook separador_multilineas_REL_DIM.ipynb
3. Ejecutar las celdas:
   - Subir el archivo Excel cuando se solicite
   - El sistema detectara automaticamente las columnas con saltos de linea y expandira los registros
   - Descargar el archivo transformado

## Funcionamiento Basico

- Detecta columnas con saltos de linea (\n)
- Separa los valores en filas independientes
- Duplica el resto de las columnas para mantener la integridad de los datos
- Restaura los valores nulos originales para mantener la calidad del dato

## Entrada esperada

Archivo Excel que puede contener saltos de linea en columnas como:
- Tabla Origen
- Tablas Stg
- proceso
- Tablas Destinos

## Salida generada

Archivo Excel limpio, sin saltos de linea internos y con un registro unico por cada valor expandido, listo para ser utilizado en procesos de carga o integracion.

