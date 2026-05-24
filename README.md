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

## Kernels a explorar

- Kernel lineal
- Kernel RBF (Gaussiano)
- Kernel polinomial

---

## Herramientas

- Python
- scikit-learn
- NumPy
- pandas
- matplotlib
- seaborn
- Jupyter Notebook

---

## Aplicación esperada

Se espera analizar cómo distintos kernels y parámetros de regularización afectan:

- la separación entre clases,
- la capacidad de generalización,
- y el desempeño predictivo del modelo en un contexto de riesgo de crédito.

---

## Referencias iniciales

- Hastie, Tibshirani & Friedman — *The Elements of Statistical Learning*
- Bishop — *Pattern Recognition and Machine Learning*
- scikit-learn documentation