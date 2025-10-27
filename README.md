# 🧠 Reproducción de "Bio-inspired algorithms for diagnosis of breast cancer"

Este proyecto reproduce y extiende los experimentos del artículo *“Bio-inspired algorithms for diagnosis of breast cancer”*, aplicando algoritmos metaheurísticos bioinspirados para la selección de características en el conjunto de datos **Wisconsin Diagnostic Breast Cancer (WDBC)**.  

Se implementaron los algoritmos **Binary Ant Colony Optimization (BACO)**, **Binary Artificial Bee Colony (BABCO)**, **Binary Firefly Algorithm (BFA)** y **Binary Particle Swarm Optimization (BPSO)**, utilizando los clasificadores **KNN** y **SVM**.  
Las mejoras propuestas incluyen el uso de **validación cruzada estratificada (StratifiedKFold)** en lugar de la validación tradicional y ajustes en los parámetros de cada algoritmo. Además, se exploró un experimento adicional con **NSGA-II** para comparar un enfoque multiobjetivo.

---

## ⚙️ Instalación

Sigue estos pasos para configurar y ejecutar el proyecto:

### 1️⃣ Clonar el repositorio
```bash
git clone https://github.com/usuario/nombre-proyecto.git
cd nombre-proyecto
