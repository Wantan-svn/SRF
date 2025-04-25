📄 SRF - Separador de Registros Multilínea en Excel
SRF es una herramienta diseñada para detectar y transformar registros de Excel que contienen múltiples líneas en una misma celda, generando un registro limpio por cada valor separado.
Ideal para preparar datos antes de cargas masivas a bases de datos o sistemas de integración.

🚀 Objetivo
Automatizar la limpieza y normalización de archivos Excel que tienen problemas de lectura por saltos de línea internos, especialmente en tablas como REL_DIM.

🔧 Tecnologías y Herramientas Utilizadas
Lenguaje principal: Python

Entorno de desarrollo: Google Colab

Procesamiento de Excel: pandas, openpyxl

Carga de archivos: Google Colab files.upload

Exportación final: Excel .xlsx descargable

🛠️ Instalación y Ejecución
Abre Google Colab: https://colab.research.google.com

Crea un nuevo cuaderno o sube el notebook separador_multilineas_REL_DIM.ipynb.

Ejecuta las celdas:

Sube tu archivo Excel cuando se solicite.

El sistema detectará automáticamente las columnas con saltos de línea y expandirá los registros.

Descarga el archivo transformado listo para carga.

⚙️ Funcionamiento Básico
Detecta columnas con saltos de línea (\n).

Separa los valores en filas independientes.

Duplica el resto de las columnas para mantener la consistencia.

Restaura los valores nulos originales (sin alterar otros datos).

📁 Entrada esperada
Archivo Excel con celdas que contienen múltiples líneas en columnas como:

Tabla Origen

Tablas Stg

proceso

Tablas Destinos

📤 Salida generada
Archivo Excel limpio, sin saltos de línea internos y con un registro único por valor.
