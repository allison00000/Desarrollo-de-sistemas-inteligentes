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