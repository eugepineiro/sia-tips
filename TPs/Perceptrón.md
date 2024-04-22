# Perceptrón Simple y Multicapa 

El objetivo del Trabajo es dar una introducción a Redes Neuronales implementando perceptrón simple y multicapa

## Tips 

### Train / Test

Dividir el conjunto de datos en training set y testing set. Para ello, tener en claro la diferencias entre: 


- Ttraining set : conjunto de datos usados para calcular los pesos
- Testing set: conjunto de datos que NO fueron usados para calcular los pesos

- Aprender bien en el training set = converger
- Aprender bien en el test set = generalizar
- Aprender bien = dada una entrada obtener la salida esperada

### Tipo de problema 

Poner el foco de los resultados en qué tipo de proble resuelve cada perceptron. Por ejemplo, el perceptron lineal se ajusta bien para problemas lineales pero no lo hará para problemas donde el conjunto de datos es no lineal.

### Hiperparámetros 

El ajuste de hiperparámetros es un problema complejo en Redes Neuronales. Para evaluar los hiperparámetros de su red, variar solo uno y fijar todo el resto. 

### Análisis 

A la hora de presentar los resultados es importante hacer un análisis previos de los hiperparámetros de la red. Por ejemplo, evaluar:
- ¿Cómo varía el error en función de la tasa de aprendizaje?
- ¿Cómo varía el error en función de las épocas?
- ¿Cómo influye la arquitectura de red? ¿Qué ocurre si agrego más capas o más neuronas?
- ¿Hay sobreajuste/overfitting?

### Optimizadores
Los optimizadores influyen notablemente en los resultados, evaluarlo tanto del punto de vista de las métricas de performance del modelo como desde el costo computacional.

### Presentación 

En la presentación se deben aclarar todos los parámetros y cuestiones de implementación que consideren necesarios: 
- Arquitectura de red (capas y neuronas por capa)
- Hiperparámetros como por ejemplo la tasa de aprendizaje, la cantidad de épocas, entre otros.
- Optimizadores utlizados. 
- Función de pérdida
- Cálculo del error 



