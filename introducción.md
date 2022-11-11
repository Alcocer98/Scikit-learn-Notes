# ¿Qué es machine learning?

En pocas palabras Machine learning es acerca de crear modelos predictivos. Lo importante del machine learnig es saber por qué y cuando deben de ser usados.
En términos concretos machine learning crea las reglas de predicción a parir de los datos.

Los datos que uno maneja pueden contar con **ruído**, es decir, aspectos que no pueden ser explicados en ambitos provenientes de los datos.

## Memorización

Una posibilidad para modelo de predicción es la memorización de todos los datos disponibles.

- Almacenar todo el conocimiento de los individuos (un censo)
- Al recibir un nuevo individuo, se podría predecir de manera cercana a lo que se tiene en la base de datos

A este método se le conoce en machine learning como predicción de vecinos cercanos (nearest neighbor predictor). La ventaja de este método es que el error esperado es de 0, esto debido a que el caso al que se le hace predicción ya es conocido (está en la base de datos) la relación es en sí misma la conocida por lo que en consecuencia se tendrá un error de predicción de 0. Por ende **no se tendrán errores en nuevos datos**.

Las desventajas de este modelo es que si dentro de los datos que se tienen y los datos entrantes son ajenos se comenzarán a tener errores de predicción. Esto debido a que **generalizar es disinto que memorizar**. Y este este es el fundamento retador en machine learning.

Por ende los datos de entrenamiento son distintos a los datos de prueba.

- Los datos a los que se les aplica el modelo predictivo (conocidos como test data) son diferentes a los que se usan para crear el modelo predictivo (train data).
- Son diferentes los grupos de datos empleados porque podrían tener diferente ruído.
- Principalmente se usan diferentes datos para observar diferentes características que no se hayan observado, diferentes combincaciones de ocupación, edad, etc.

El modelo típico en el que se hace el flujo de trabajo en machine learning es:

1. Usar data set para aprender un modelo predictivo (data set)
2. Aplicar nuevos datos (test set) para poner a predecir al modelo o evaluar su viabilidad

## Conceptos de machine learning

**data matrix:** Todos los datos usados tendrán forma de tabla donde las **filas** se referirán a las diferentes observaciones (**samples**) y las **columnas** serán los diferentes características (**features**). Puede ser visto como una trabla 2D.

**Supervised machine learning:** Los datos recibidos son anotados, es decir, son asociados a una categoría o target class. En términos matemáticos es la acción de proporcionar datos (matrices) denotada como **X** con n observaciones. Y el objetivo (**target**) denotado como **y** al cual se le dan características resultado de la observación. ***El propósito es predecir Y a partir de X*** 

**Unsupervised machine learning:** Se proporcionan datos en formato de matriz 2D denotado por X, con lo cual no existe un objetivo disponible, el objetico es entonces extraer algun tipo de estructura a partir de X que generalice los nuevos datos. Este tipo de machine learning cubre otro tipo de problemas

Otro modelo supervisado es:

**Regression and classification:** En ambos caso al ser un aprendizaje supervisado (se predice como objetivo Y).
- **Classification:** Y es discreto, hecho de diferentes clases
- **Regresión:** Y es contínuo, es decir una cantidad numérica 

## Datos importantes

Machine learning trata acerca de la extracción proveniente de reglas de datos que generalizan nuevas observaciones.
