# SVM Credit Risk

El objetivo del proyecto es estudiar las **Máquinas de Soporte Vectorial (SVM)** desde su formulación matemática como problema de optimización convexa y aplicarlas a un problema de clasificación de riesgo de crédito.

---

## Integrantes

- Andrés Padrón
- Othoniel Camacho
- Manuel De la Tejera

---

## Objetivos

- Comprender la formulación matemática de SVM
- Analizar el problema primal y dual
- Estudiar el concepto de margen máximo
- Implementar SVM lineal y no lineal
- Aplicar el modelo a un problema de riesgo de crédito
- Comparar resultados utilizando distintos kernels

---

## Problema de aplicación

El proyecto se enfoca en un problema de clasificación binaria relacionado con riesgo de crédito.

El objetivo será clasificar solicitantes en:

- Aprobado
- Rechazado

utilizando variables financieras y demográficas.

Cada solicitante será representado como un punto en un espacio de múltiples dimensiones, donde SVM buscará encontrar el hiperplano óptimo que maximice la separación entre clases.

---

## Temas principales

- Optimización convexa
- Programación cuadrática
- Máquinas de Soporte Vectorial (SVM)
- Margen máximo
- Support Vectors
- Kernels
- Clasificación binaria
- Riesgo de crédito

---

## Estructura del proyecto

```text
SVM-credit-risk/
│
├── data
│   ├── processed
│   └── raw
│
├── docs
│   ├── images
│   ├── Avance_Proyecto Final_CHEQUE.docx
│   └── Avance_Proyecto Final_CHEQUE.pdf
│
├── extra
│   ├── SVM_teoria
│   ├── Kernel Trick.ipynb
│   ├── Maquinas de Soporte Vectorial.ipynb
│   └── imágenes y material teórico auxiliar
│
├── notebooks
│
├── src
│
├── LICENSE
└── README.md
```

---

## Metodología

El proyecto se dividirá en dos componentes principales:

### Parte teórica

- Fundamentos geométricos de SVM
- Hiperplano de separación
- Margen máximo
- Formulación primal y dual
- Multiplicadores de Lagrange
- Parámetro de regularización \(C\)
- Kernel Trick

### Parte práctica

- Limpieza y preparación de datos
- Entrenamiento de modelos SVM
- Comparación entre kernels
- Evaluación del desempeño
- Visualización de fronteras de decisión

---

---

## Resultados finales

Se desarrolló un modelo de clasificación de riesgo de crédito utilizando Máquinas de Soporte Vectorial (SVM), analizando tanto su formulación matemática como su implementación computacional.

Se compararon distintos kernels y estrategias de regularización, obteniendo los siguientes resultados:

| Modelo | Kernel | Accuracy |
|---|---|---|
| SVM lineal | Linear | 0.53 |
| SVM no lineal | RBF | 0.80 |
| SVM optimizado | RBF + Grid Search | 0.94 |

El modelo final optimizado fue un SVM con kernel RBF utilizando:

$$
C = 100
\qquad
\gamma = 0.1
$$

obteniendo un desempeño cercano al:

$$
94\%
$$

de exactitud sobre el conjunto de prueba.

---

## Visualizaciones desarrolladas

El proyecto incorpora visualizaciones geométricas y matemáticas avanzadas para interpretar el comportamiento del modelo:

- Matrices de confusión
- Fronteras de decisión
- Comparación entre kernels
- Regiones de clasificación
- Mapas topográficos de optimización
- Visualización de support vectors
- Proyecciones PCA en 2D y 3D
- Superficies geométricas del kernel RBF
- Interpretación del hiperespacio de decisión

Estas visualizaciones permiten conectar directamente la teoría de optimización convexa con la geometría de clasificación de SVM.

---

## Conceptos matemáticos implementados

Durante el proyecto se desarrollaron e interpretaron:

- Problema primal y dual de SVM
- Condiciones KKT
- Multiplicadores de Lagrange
- Soft Margin SVM
- Kernel Trick
- Espacios de Hilbert
- Maximización del margen
- Fronteras de decisión no lineales
- Regularización mediante \(C\)
- Función de decisión:

$$
f(x)=\sum_{i=1}^{n}\alpha_i y_i K(x_i,x)+b
$$

---

## Principales conclusiones

- El kernel lineal presenta limitaciones cuando las clases no son linealmente separables.
- El kernel RBF mostró el mejor desempeño al capturar relaciones no lineales complejas presentes en los datos financieros.
- El parámetro \(C\) controla el balance entre margen amplio y penalización de errores.
- Los support vectors representan las observaciones críticas que determinan la frontera óptima de clasificación.
- La validación cruzada y el tuning de hiperparámetros fueron fundamentales para mejorar la capacidad de generalización del modelo.
- Las proyecciones PCA permitieron interpretar geométricamente regiones de decisión en espacios de alta dimensión.

---

## Tecnologías utilizadas

- Python
- scikit-learn
- NumPy
- pandas
- matplotlib
- seaborn
- SciPy
- Jupyter Notebook

---

## Aplicación

El proyecto demuestra cómo los métodos de optimización convexa y aprendizaje estadístico pueden utilizarse para resolver problemas reales de clasificación de riesgo de crédito, integrando teoría matemática, geometría computacional y machine learning.