# Assignment-4-Single-Neuron-Network-with-and-without-PCA

Este repositorio contiene el trabajo realizado en conjunto con mis compañeros Sergio Alejandro Zamora Dávila y Perla Yazmín Antonio Pérez. En este trabajo se desarrollan dos modelos de clasificación basados en redes neuronales de una sola neurona, utilizando el mismo dataset.

El primer modelo fue entrenado utilizando las 30 características originales del dataset, mientras que el segundo modelo fue construido aplicando previamente Análisis de Componentes Principales (PCA) para reducir la dimensionalidad de los datos, conservando aproximadamente el 95% de la varianza explicada.

En el archivo [assignment_PCA.ipynb](assignment_PCA.ipynb) se encuentra el desarrollo de los modelos.
* HTML -> [assignment_PCA.html](assignment_PCA.html)

**Información del dataset**

[]()

El dataset seleccionado para este proyecto es *Breast Cancer Wisconsin (Diagnostic)* (Mangasarian, 1993), recuperado del [UC Irvine Machine Learning Repository](https://archive.ics.uci.edu/dataset/17/breast+cancer+wisconsin+diagnostic). Este conjunto de datos se enfoca en el área médica, en la investigación para el diagnóstico del cáncer de mama.

Su propósito principal es clasificar tumores como benignos o malignos a partir de características obtenidas de imágenes digitalizadas de aspiraciones con aguja fina (FNA) de masas mamarias.

El dataset tiene un total de 569 datos y 32 columnas. De estas, una corresponde al número de cada muestra (ID) y la otra es la variable objetivo (Diagnosis), donde M indica un tumor maligno y B uno benigno. Las 30 variables restantes corresponden a características numéricas calculadas a partir de las imágenes.

Para cada núcleo celular se calcularon 10 características principales, y de cada una se obtuvieron tres medidas diferentes: promedio, error estándar y valor máximo. Esto nos da, al final del día, 30 variables predictoras.


Las 10 características principales son:

- radius: media de las distancias desde el centro hasta los puntos del perímetro.

- texture: desviación estándar de los valores en escala de grises.

- perimeter: longitud del contorno del núcleo.

- area: área del núcleo.

- smoothness: variación local en las longitudes del radio.

- compactness: $$
\frac{\text{perimeter}^2}{\text{area}} - 1
$$
- concavity: severidad de las porciones cóncavas del contorno.

- concave points: número de porciones cóncavas del contorno.

- symmetry: simetría del núcleo.

- fractal dimension: $$\text{coastline approximation} - 1$$

