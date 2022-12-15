![HenryLogo](https://d31uz8lwfmyn8g.cloudfront.net/Assets/logo-henry-white-lg.png)

<p align="center">
<img src="https://406242.smushcdn.com/2456487/wp-content/uploads/2019/06/blog-6-24-19.jpg?lossy=1&strip=1&webp=1"   
>
</p>

<h1 align="center">Proyecto Individual #2</h1>
<h3 align="center">Daniel Muñoz López</h3>
<h3 align="center">DATAFT05</h3>
<hr>

## Objetivo

El presente proyecto tiene como pilar principal la aplicación de modelos de *Machine Learning* para realizar predicciones en enfoque de clasificación. Cabe recordar que los modelos de predicción se basan en la aplicación de herramientas estadísticas que permiten analizar los datos de manera que puedan ser interpretados como resultados de funciones matemáticas, que al tener forma funcional permiten ser extrapolados a más valores.

## Contexto del Proyecto.

En todos los centros de atención hospitalaria existe el problema de la limitación de camas y/o habitaciones para pacientes cuando hay gran cantidad de usuarios que lo requieran.

La toma de datos y análisis de los mismos podría ayudar a predecir cuando un paciente tendría una hospitalización más duradera de lo habitual y así optimizar mejor los recursos del hospital. Si bien, las condiciones individuales en la salud de los pacientes son particulares para cada uno de ellos, existen variables que el mismo hospital puede evaluar y determinar que tan influyentes pueden ser a la hora de asignar el tiempo de permanencia de un usuario.

## Desarrollo del Proyecto

Para la implementación del modelo de predicción se usó un dataset con la información de un hospital cuyas variables estaban enfocadas a determinar si un paciente estaría más de 8 días hospitalizado.

Se realiza una análisis exploratorio de datos (EDA), decidiendo que variables realmente tenían influencia en la cantida de días en las que estaría un paciente usando el *coeificiente de correación de Pearson*, con el dataset de entrenamiento, aplicado al modelo.

Posteriormente se evaluaron que tipo de modelos tenían una mejor precisión (accuracy) para ser implementados, llegando a la conclusión que los **árboles de decisión** daban mejores respuestas frente a la problemática.

## Resultados del Modelo.

Para la evaluación del modelo se usaron dos métricas: *accuracy* y *exhaustividad* obtenidos a partir de la matriz de confusión.

$$ Recall=\frac{TP}{TP+FN} = 0.9953751486092784$$

$$ Accuracy=\frac{TP+TN}{P+N} = 0.684219512195122$$


## Conclusiones

El modelo tiene una alta exhaustividad, es muy sensible a los datos que hayan, sin embargo esto lleva a que su precisión no sea 100% fiable, tiene un accuracy menor.

Estos resultados dan cuenta del caracter aleatorio que puede tener un paciente, no solo pode su edad, género, doctor a cargo o dependencia que lo atiende, sino a su condición individual por la que haya ingresado al hospital.

Es dificil predecir con exactitud la necesidad de atención en el estado de salud de una persona, sin embargo, el modelo permite ayudar en la evualuación de saber si un paciente requiere permanecer más de 8 días hospitalizado.