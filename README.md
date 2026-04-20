# Analítica Para Negocios

[![documentation](https://img.shields.io/badge/📖-docs-brightgreen)](https://fralfaro.github.io/ICS40125/)

<img src="docs/images/logo3.png" alt="Analítica Para Negocios" align="center" width="420"/>

## Contenidos

### Analítica & Negocios

**Analítica para la toma de decisiones:**  
Este curso introduce herramientas estadísticas y computacionales para entender datos, construir modelos y transformar resultados analíticos en recomendaciones de negocio. A lo largo del semestre trabajamos con casos aplicados, ejercicios y proyectos donde los datos se conectan con problemas reales de decisión.

**Motivación:**  
La analítica se ha vuelto una capacidad central para organizaciones que necesitan medir, comparar, predecir y actuar. En este curso usamos Python como lenguaje de trabajo para desarrollar una base sólida en análisis exploratorio, inferencia y modelamiento estadístico.

### Sobre el curso

**Trabajo con datos:**  
Partimos con una introducción al entorno de trabajo en Python y al uso de herramientas fundamentales como `NumPy` y `pandas`, enfocándonos en manipulación de datos, tablas y operaciones numéricas.

**Inferencia estadística:**  
Estudiamos cómo extraer conclusiones desde muestras, interpretar estimadores y aplicar test de hipótesis para responder preguntas relevantes en contextos de negocio.

**Modelos de regresión:**  
Desarrollamos regresión lineal, validación cruzada, bootstrap y regularización. Estas herramientas permiten explicar relaciones entre variables, evaluar desempeño y controlar problemas como el sobreajuste.

**Modelos de clasificación:**  
El curso incorpora regresión logística, métricas de clasificación, SVM y modelos basados en árboles para abordar problemas donde el objetivo es predecir categorías o eventos.

**Interpretación y comunicación:**  
No solo se busca ajustar modelos, sino también interpretar resultados, comunicar hallazgos y convertir análisis cuantitativos en recomendaciones accionables.

### Material disponible

**Clases:**  
El repositorio incluye notebooks con el desarrollo de las clases del curso:

- `clase_01.ipynb` a `clase_05.ipynb`: fundamentos, inferencia y test de hipótesis
- `clase_06.ipynb` a `clase_10.ipynb`: regresión, resampling, regularización y modelos no lineales
- `clase_11.ipynb`, `clase_12a.ipynb` y `clase_12b.ipynb`: clasificación, métricas, SVM y árboles

**Ejercicios:**  
Se incluyen actividades prácticas para reforzar conceptos del curso, junto con notebooks de apoyo y soluciones.

**Datasets:**  
El material considera bases de datos para clases y proyectos, incluyendo conjuntos asociados a salud, housing, turismo, ventas, banca y compensaciones.

**Evaluaciones:**  
El curso contempla tres evaluaciones principales con componente de proyecto y presentación. Entre los temas cubiertos se incluyen:

- análisis de salarios y compensaciones con regresión lineal
- modelamiento de churn bancario con clasificación
- actividades intermedias y entregas según el cronograma oficial del curso

## Recursos

- [Documentación del curso](https://fralfaro.github.io/ICS40125/)
- [Programa y cronograma](docs/programa.md)
- [Listado de clases](docs/clases/clases.md)
- [Datasets disponibles](docs/datasets/datasets.md)
- [Proyecto 1](docs/assessments/project1.md)
- [Proyecto 2](docs/assessments/project2.pdf)
- [Proyecto 3](docs/assessments/project3.md)

## Estructura del repositorio

```text
.
├── docs/
│   ├── clases/
│   ├── exercises/
│   ├── datasets/
│   ├── assessments/
│   ├── images/
│   ├── index.md
│   ├── perfil.md
│   └── programa.md
├── mkdocs.yml
├── pyproject.toml
└── uv.lock
```

## Documentación local

Para instalar el entorno y levantar el sitio localmente:

```bash
uv sync
uv run mkdocs serve
```

Para construir la documentación:

```bash
uv run mkdocs build
```
