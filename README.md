# Modelo de Machine Learning para predecir si un futuro procedimiento policial terminará en arresto.

## Descripción del proyecto

Este proyecto tiene como objetivo realizar un proceso completo de análisis y modelado de datos utilizando Python y técnicas de Machine Learning. Utilizaremos el set de datos de los policias de New York del año 2009 y 2010. (2009_1perc.csv y 2010_1perc.csv). Los datos contienen información de características de los procedimientos policiales realizados en esos años. Algunas características son: fecha y hora de detención, tipo de sospecha, género, raza, ciudad, sector, lugar de detención, tipo de identificación y la característica a predecir "arstmade": arresto realizado, con las opciones Si y No.

La variable 'arstmade' indica si un procedimiento policial ha terminado en arresto o no.

El flujo del proyecto incluye:

- Descarga de datos 
- Preprocesamiento de datos
- Análisis exploratorio de datos (EDA)
- Entrenamiento de modelos de Machine Learning y evaluación y comparación de modelos

Los modelos implementados son:

- Random Forest
- Gradient Boosting

---

# Tecnologías utilizadas

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
- Plotly
- Jupyter Notebook
- Graphviz
- ipykernel
- nbformat
- pyarrow

---

# Estructura del proyecto

AL-KE-LA-PREDICCION_ARRESTOS/

├── data/

│   ├── 2009-1perc.zip

│   ├── 2010-1perc-csv.zip

├── notebooks/

│   ├── 01_Descarga_de_datos.ipynb

│   ├── 02_Preprocesamiento_de_datos.ipynb

│   ├── 03_Analisis_exploratorio.ipynb

│   ├── 04_Modelos.ipynb
  
 

│── .gitignore

├── README.md

├── main.py

├── pyproject.toml

├── requirements.txt

└── uv.lock

# Requisitos Previos

- Python 3.14.4 o superior

- uv (gestor de paquetes)

- Para poder utilizar el export_graphviz para la visualización de 3 árboles, es necesario instalar: 

https://graphviz.org/download/?utm_source=chatgpt.com

1. Instalar Graphviz en Windows
: Descárgalo desde el sitio oficial:

[Graphviz Downloads](https://graphviz.org/download/?utm_source=chatgpt.com)

Instala la versión para Windows o MAC.

2. Ubicar carpeta bin que normalmente queda en:

C:\Program Files\Graphviz\bin

Ahí debe existir: 
dot.exe

3. Agregar Graphviz al PATH

En Windows, buscar:

Variables de entorno

Abrir:

Editar las variables de entorno del sistema

Luego:

Variables de entorno

En Path → Editar → Nuevo

Agregar:

C:\Program Files\Graphviz\bin

4. Guardar TODO y reiniciar VS Code


Cerrar VS Code completamente y abrirlo nuevamente para que la terminal necesita recargue el PATH.

# Instalación del proyecto

1. Clonar el repositorio:

 git clone https://github.com/lauramh922-bit/al-ke-la-prediccion_arrestos.git

2. Entrar a la carpeta:

cd al-ke-la-prediccion_arrestos

3. Verificar que uv esté instalado

uv --version

Si no está instalado:

Windows:

powershell -ExecutionPolicy ByPass -c "irm https://astral.sh/uv/install.ps1 | iex"

Luego reiniciar VS Code

4. Crear el entorno virtual con UV para que se cree la carpeta .venv

uv venv

5. Activar el entorno virtual para que se visualice (venv):

### Windows

.\.venv\Scripts\activate.ps1

### Mac/Linux

source venv/bin/activate

6. Instalar dependencias:

uv sync

7. Instalar el kernel:

uv add ipykernel

8. Ejecutar el proyecto

uv run main.py

# Flujo del proyecto

1. Consolidación de datos: 
Se realiza la carga y unión de 2 datasets CSV para generar un dataset consolidado.

2. Preprocesamiento
Las actividades realizadas incluyen:

Tratamiento de valores nulos
Selección de variables
Eliminación de variables no necesarias
Encoding de variables categóricas
Escalamiento de variables numéricas
Pipeline de transformación

3. Análisis Exploratorio de Datos (EDA)

Se desarrollan análisis visuales y estadísticos para identificar:

Distribuciones
Variables relevantes
Patrones en los datos

4. Modelos implementados

- Random Forest
Modelo basado en árboles de decisión ensamblados para clasificación/predicción.

- Gradient Boosting
Modelo secuencial basado en boosting para optimizar precisión predictiva.

5. Evaluación de modelos

Los modelos son evaluados utilizando métricas como:

Accuracy
Precision
Recall
F1-Score


Librerías principales

- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
- Plotly
- Graphviz
- ipykernel
- nbformat
- pyarrow

# Consideraciones

- La carpeta .venv/ no se incluye en el repositorio por lo tanto esta ignorada mediante .gitignore.

Se recomienda utilizar Python 3.14.4 

# Autores

Maria Alejandra Villa

Kelly Panizza

Laura Marcela Hoyos
