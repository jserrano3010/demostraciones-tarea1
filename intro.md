# Demostraciones – Tarea 1

**Estudiante:** Jairo Andrés Serrano Meléndez  
**Profesor:** PhD. Lihki Rubio  
**Curso:** Machine Learning · Maestría en Ingeniería Industrial

Este libro reúne las demostraciones de la Tarea 1, basadas en las notas del curso
([K-NN](https://lihkir.github.io/MachineLearning/knn_model.html),
[modelos lineales](https://lihkir.github.io/MachineLearning/linear_model.html),
[árboles de decisión](https://lihkir.github.io/MachineLearning/decisiontree_model.html)).
Cada capítulo muestra primero la captura del enunciado de las notas y después la demostración completa.

| Capítulo | Tema | Qué se demuestra |
|---|---|---|
| 1 | K-NN | Riesgo verdadero y empírico; insesgadez de $L_S(h)$; optimalidad del clasificador de Bayes |
| 2 | K-NN | Caso $\min\{\eta,1-\eta\}=1-\eta$ en la cota del 1-NN |
| 3 | Ridge | Esperanza, covarianza, sesgo y error cuadrático medio del estimador (3.12) |
| 4 | Ridge | $Z^T\mathbf 1=\mathbf 0$, ecuación (3.8) y derivada de formas cuadráticas |
| 5 | Ridge | Igualdades de estandarización (3.11) |
| 6 | Lasso | Condiciones KKT, umbral suave, descenso por coordenadas y LARS |
| 7 | Random Forest | Error en el árbol del Ejercicio 6 |
| 8 | AdaBoost | Deducción de $a_i$ y de la actualización de pesos |

:::{admonition} Errores encontrados en las notas
:class: warning
- **Cap. 2:** la cadena $2\eta(1-\eta)\le 2(1-\eta)^2\le 2\min\{\eta,1-\eta\}$ no es válida en general (falla con $\eta=0.1$).
- **Cap. 7:** en el umbral 36, $|D_1|$ debe ser 3 (no 2), y el Gini es $0.476$ (no $0.5$); en el umbral 39 la ponderación correcta es $\tfrac{4}{10}$ y $\tfrac{6}{10}$.
- **Cap. 8:** $a_i=\tfrac12\ln\!\big(\tfrac{1-P_i}{P_i}\big)$, el logaritmo del cociente completo.
:::

Los resultados de los capítulos 3 y 6 se verificaron numéricamente con Python (simulación y `scikit-learn`).
