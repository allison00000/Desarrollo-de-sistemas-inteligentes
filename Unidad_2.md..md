2 Ejemplos machine learning

### Predicción de tráfico

**T:** Predecir el nivel de tráfico en una carretera o avenida.  
**P:** % de predicciones correctas sobre el nivel de tráfico real.  
**E:** Datos históricos de tráfico, horarios, días de la semana y condiciones climáticas.

### Predicción del precio de una casa

**T:** Predecir el precio de una vivienda según sus características.  
**P:** Diferencia promedio entre el precio predicho y el precio real.  
**E:** Datos históricos de viviendas: ubicación, tamaño, número de habitaciones, antigüedad y precio de venta.

supervisado:
se le proporciona datos al algoritmo, lo que facilita su entrenamiento y con ello aumenta el porcentaje de acierto
No supervisado:
no se le proporcionan datos para entrenar, en cambio se le pone una meta u objetivo al que tiene que llegar
Por esfuerzo:
se utiliza en casos específicos segun el sistema que se desarrolle  

Actividad 2.3
Glosario (Todo con base en Machine Learning)
-Pandas: Libreria de python orientada al analisis y manipulación de datos. Utiliza estructuras como los DataFrames (similares a tablas) para limpiar, filtrar y transformar conjuntos de datos.
-Matplotlib: Libreria estandar de python para la creación de gráficos e imagenes estadísticas de dos dimensiones (como histogramas, diagramas de dispersion, gráficos de lineas)
-Scikit-learn: Una de las librerias mas importantes de python para machine Learning. incluye algoritmos para clasificación, regresión agrupación(clustering), asi como herramientas para preprocesamiento y evaluación de modelos.
(iris, boston,wine, digits)a los que se pueden acceder mediante sklearn.datasets.
-Google colab: Entorno de cuadernos de jupyter ejecutable en la nube por parte de google. Permite escribir y ejecutar código Python en el navegador web con acceso gratuito a recursos como GPUs/TPUs.

Conceptos de modelado y evaluación 
Arbol de decision: algoritmo de aprendizaje supervisado que organiza las decisiones en una estructura en forma de árbol. evalua condiciones sucesivas en los atributos de los datos para llegar a una predicción final.
Matriz de confusion: Tabla utilizada en problemas de clasificación para medir el rendimiento de un modelo. compara los valores  reales contra las predicciones hechas por el modelo para identificar aciertos y errores.

sobreajuste(overfitting): Problema que ocurre cuando un modelo de machine learning memoriza en exceso lo datos de entrenamiento (incluyento el ruido o detalles insignificantes). como consecuencia, obtiene un excelente desempeño en los datos de entrenamiento pero falla al integrar generalizar sobre datos nuevos.

-Falso Positivo: Ocurre cuando un sistema, prueba o evaluación indica que algo si esta presente o ha sucedido, cuando en realidad no es asi 
-Falso Negativo: Ocurre cuando un sistema indica que algo no esta presente o ha sucedido, cuando en realidad si esta presente 

Actividad 2.4

|                        | Definición                                                                                                                                                                       | Cómo funciona                                                                                                                                                                                                                                                                                                     | Un caso de uso                                                                          |
| ---------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- |
| Arbol de decisión      | Es un modelo de aprendizaje supervisado en forma de diagrama de flujo que divide los datos en ramas según ciertas condiciones para tomar una decisión o clasificar un resultado. | Evalúa una característica a la vez mediante preguntas condicionales en cada nodo. Comienza en la raíz, divide los datos en subconjuntos cada vez más homogéneos y avanza hasta llegar a las hojas, las cuales representan la predicción final.                                                                    | Sistemas de diagnostico medico preliminar basados en sintomas                           |
| Regresión logistica    | Es un algoritmo de clasificación estadística utilizado para predecir la probabilidad de que una observación pertenezca a una categoría específica (binaria).                     | Calcula una combinación lineal de las variables de entrada y aplica una función sigmoide para transformar el resultado en un rango de probabilidades entre 0 y 1. Si la probabilidad supera un umbral determinado (por ejemplo, 0.5), se asigna a la clase positiva.                                              | <br>deteccion de correo no deseado                                                      |
| K vecinos mas cercanos | Es un algoritmo de clasificación y regresión basado en instancias que no requiere un entrenamiento explícito previa integración de datos (lazy learner).                         | Calcula la distancia (como la distancia euclidiana) entre la nueva muestra y todos los puntos del conjunto de entrenamiento. Selecciona los k puntos más cercanos e identifica la clase más frecuente entre ellos (votación por mayoría) para asignarla al nuevo dato.                                            | Busqueda de documentos o textos similares dentro de una base de datos                   |
| Naive Bayes            | Es un clasificador probabilístico basado en el teorema de Bayes, el cual asume que las características de entrada son independientes entre sí dada la clase.                     | Calcula las probabilidades previas y la verosimilitud de las variables para cada categoría. Aplica la fórmula del teorema de Bayes para determinar la probabilidad a posteriori de cada clase y selecciona la clase con la probabilidad más alta.                                                                 | Analisis de sentimientos en redes sociales (comentarios positivos, neutros o negativos) |
| SVM                    | Algoritmo que busca encontrar el hiperplano óptimo para clasificar datos separándolos en distintas categorías dentro de un espacio multidimensional.                             | Encuentra la frontera de decisión (hiperplano) que maximiza el margen o distancia entre las clases más cercanas (vectores de soporte). Para datos no separables linealmente, emplea funciones kernel que proyectan los datos a un espacio de mayor dimensión donde sí puedan separarse.                           | clasificacion de imagenes y reconocimiento facial                                       |
| Bosque aleatorio       | Método de aprendizaje en conjunto (ensemble learning) que combina múltiples árboles de decisión para lograr una predicción más precisa y estable.                                | Genera múltiples árboles entrenados con subconjuntos aleatorios de datos y características (técnica de bagging). Al momento de predecir, combina los resultados individuales mediante votación por mayoría (clasificación) o promedio (regresión).                                                                | Deteccion de fraudes en transacciones financieras con tarjetas de credito               |
| Red neuronal           | Modelo computacional inspirado en la estructura y funcionamiento del cerebro humano, diseñado para identificar patrones complejos en los datos.                                  | Está compuesta por capas de nodos (capa de entrada, capas ocultas y capa de salida) interconectadas mediante pesos. Ajusta estos pesos durante el proceso de entrenamiento utilizando el algoritmo de propagación hacia atrás (backpropagation) y descenso de gradiente para minimizar el error de la predicción. | Reconocimiento y sintesis de voz en asistentes virtuales                                |
Referencias   
Bishop, C. M. (2006). Pattern Recognition and Machine Learning. Springer.   
Hastie, T., Tibshirani, R., & Friedman, J. (2009). The Elements of Statistical Learning: Data Mining, Inference, and Prediction (2nd ed.). Springer.   
James, G., Witten, D., Hastie, T., & Tibshirani, R. (2013). An Introduction to Statistical Learning: with Applications in R. Springer.
Russell, S., & Norvig, P. (2020). Artificial Intelligence: A Modern Approach (4th ed.). Pearson.