# Reproducción de "Bio-inspired algorithms for diagnosis of breast cancer"

Este proyecto reproduce y extiende los experimentos del artículo *“Bio-inspired algorithms for diagnosis of breast cancer”*, aplicando algoritmos metaheurísticos bioinspirados para la selección de características en el conjunto de datos **Wisconsin Diagnostic Breast Cancer (WDBC)**.  

Se implementaron los algoritmos **Binary Ant Colony Optimization (BACO)**, **Binary Artificial Bee Colony (BABCO)**, **Binary Firefly Algorithm (BFA)** y **Binary Particle Swarm Optimization (BPSO)**, utilizando los clasificadores **KNN** y **SVM**.  
Las mejoras propuestas incluyen el uso de **validación cruzada estratificada (StratifiedKFold)** en lugar de la validación tradicional y ajustes en los parámetros de cada algoritmo. Además, se exploró un experimento adicional con **NSGA-II** para comparar un enfoque multiobjetivo.

---

## Instalación

Sigue estos pasos para configurar y ejecutar el proyecto:

### 1️ Clonar el repositorio
```bash
git clone https://github.com/usuario/nombre-proyecto.git
cd nombre-proyecto

### 2 Crear entonro virtual
python -m venv venv
source venv/bin/activate   # macOS/Linux
venv\Scripts\activate      # Windows


### 3 Instalar dependencias
pip install -r requirements.txt

## Ejecutar experimentos:

Los scripts originales del artículo están en la carpeta src/ (réplica directa del código original).

Las versiones modificadas se encuentran en experiments/, donde se implementaron los cambios en validación y parámetros.


## Figuras

Las gráficas utilizadas en el reporte se generan desde un notebook en la carpeta figures/.
El notebook toma los resultados de results/, agrupa las métricas y genera comparaciones visuales con matplotlib.

## Descripción de los archivos principales
Carpeta / Archivo	Descripción
src/	Contiene la réplica del código original del paper sin modificaciones.
experiments/	Incluye los scripts modificados con StratifiedKFold, ajustes de parámetros y el experimento con NSGA-II.
data/	Archivos del conjunto de datos o scripts de preprocesamiento.
results/	Resultados generados tras ejecutar los experimentos (métricas promedio).
figures/	Figuras y gráficas comparativas utilizadas en el reporte final.
requirements.txt	Lista de librerías y versiones necesarias para ejecutar el proyecto.

Resultados generales

El algoritmo BABCO mostró los mayores incrementos en estabilidad y generalización tras aplicar los cambios.
El uso de validación estratificada redujo la varianza entre ejecuciones y mejoró la confiabilidad de las métricas.
El experimento adicional con NSGA-II confirmó el potencial de los enfoques multiobjetivo para equilibrar precisión y simplicidad del modelo.


