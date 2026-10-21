Algoritmos de busqueda (son metodos que permiten encontar una solucion a un problema explorando diferentes posibilidades)

1. Problema de búsqueda
Es una situación en la que se busca encontrar una solución entre varias posibilidades.
Ejemplo: encontrar la ruta más corta de tu casa a la universidad.
2. Espacio de estados
Es el conjunto de todos los estados o situaciones posibles por las que puede pasar el problema.
Ejemplo: en un laberinto, cada posición donde puedes estar representa un estado.
3. Estado inicial
Es el punto donde comienza la búsqueda.
Ejemplo: la entrada del laberinto.
4. Acciones
Son los movimientos o decisiones que permiten pasar de un estado a otro.
Ejemplo: avanzar, retroceder, girar a la izquierda o a la derecha.
5. Modelo de transición
Describe cómo cambia el estado cuando se realiza una acción.
Ejemplo: si estás en una casilla y avanzas una posición, llegas a la siguiente casilla disponible.
6. Prueba de meta
Es la condición que permite comprobar si se ha alcanzado el objetivo.
Ejemplo: verificar si llegaste a la salida del laberinto.
7. Costo del camino
Es el costo total de las acciones realizadas para llegar a la meta. Puede representar distancia, tiempo, dinero o cantidad de movimientos.
Ejemplo: una ruta de 5 km cuesta menos distancia que una de 8 km.
8. Solución
Es la secuencia de acciones que permite llegar desde el estado inicial hasta el objetivo.
Ejemplo: la lista de movimientos que te lleva a la salida.
9. Frontera
Es el conjunto de estados descubiertos que todavía están pendientes de explorar.
Ejemplo: las casillas posibles a las que puedes avanzar, pero que aún no has revisado.
10. Nodo
Es una representación de un estado dentro del árbol o estructura de búsqueda. Puede almacenar el estado, el nodo anterior, la acción realizada y el costo acumulado.
Ejemplo: una casilla del laberinto representada dentro del algoritmo.
11. Agente de resolución de problemas
Es el sistema que analiza el problema, busca alternativas y selecciona acciones para alcanzar una meta.
Ejemplo: un programa que calcula una ruta para un robot.
12. Sistemas y estrategias de búsqueda
Los sistemas de búsqueda utilizan diferentes estrategias para decidir qué estado explorar primero.
Búsqueda no informada (ciega)
Explora los estados sin utilizar información adicional que indique qué tan cerca está de la meta. Sigue las reglas del algoritmo.
Ejemplo: revisar las rutas disponibles sin saber cuál parece más cercana al destino.
Búsqueda en amplitud (BFS)
Explora primero todos los estados de un nivel y después pasa al siguiente. Utiliza una cola (FIFO): el primero en entrar es el primero en salir.
Ejemplo: revisar primero todas las casillas que están a un movimiento de distancia, después las que están a dos movimientos, etc.
Búsqueda en profundidad (DFS)
Explora un camino lo más profundo posible antes de regresar y probar otra alternativa. Utiliza una pila (LIFO): el último en entrar es el primero en salir.
Ejemplo: seguir un camino del laberinto hasta que ya no se pueda avanzar y regresar si es necesario.
Búsqueda de costo uniforme
Explora primero el camino que tiene el menor costo acumulado, sin importar cuántos pasos tenga.
Ejemplo: elegir una ruta de 10 km que cuesta menos que otra de 6 km, si la ruta de 10 km tiene un costo total menor según los valores asignados.
Cola (FIFO)
El primero en entrar es el primero en salir. Se utiliza en búsqueda en amplitud.
Ejemplo: una fila de personas esperando turno.
Pila (LIFO)
El último en entrar es el primero en salir. Se utiliza en búsqueda en profundidad.
Ejemplo: una pila de platos: retiras primero el que está arriba.
Propiedades de los algoritmos
Completitud
Indica si el algoritmo garantiza encontrar una solución cuando existe, bajo las condiciones correspondientes.
Optimalidad
Indica si el algoritmo garantiza encontrar la mejor solución, normalmente la de menor costo.
Complejidad en tiempo
Es la cantidad de operaciones o el tiempo de ejecución que puede necesitar el algoritmo conforme aumenta el tamaño del problema.
Complejidad en espacio
Es la cantidad de memoria que necesita para almacenar los estados y la información de búsqueda.
actividad3.1.2
![[WhatsApp Image 2026-10-08 at 6.25.22 PM.jpeg|385]]![[WhatsApp Image 2026-10-08 at 6.26.16 PM.jpeg|388]]![[WhatsApp Image 2026-10-08 at 6.27.19 PM.jpeg|366]]![[WhatsApp Image 2026-10-08 at 6.28.02 PM.jpeg|364]]BFS prioriza explorar por niveles, mientras que Dijkstra prioriza el costo acumulado de cada ruta. En un mapa donde todos los movimientos tienen el mismo costo, ambos pueden encontrar caminos óptimos, si existen costos diferentes, Dijkstra puede encontrar la ruta de menor costo.

Heuristica
La **heurística** es el conjunto de técnicas, estrategias o atajos mentales de carácter práctico que permiten resolver problemas, tomar decisiones o hacer descubrimientos de forma rápida, aunque no garanticen una solución perfecta o 100% óptima.

**En inteligencia artificial y computación:** Son algoritmos o métodos prácticos que exploran grandes volúmenes de datos para dar con una solución "suficientemente buena" en poco tiempo, evitando revisar cada combinación posible.

***actividad 3.2***
Compara een la pagina dos algoritmos (A*) y uno ciego. Contestar las siguientes preguntas:

**qué longitud tiene cada algoritmo?**
A*(Manhattan)=22
A*(Manhattan(Allow diagonal))=16.73
Breadth-First-Search=22
Breadth-First-Search(Allow diagonal16.73
**cuanto tiempo se tardo cada algoritmo?**
A*(Manhattan1.0000ms
A*(Manhattan(Allow diagonal))=0.0000ms
Breadth-First-Search=2.0000ms
Breadth-First-Search(Allow diagonal)=1.0000ms
que diferencia observas?
solo cambia si contiene "Allow diagonal" de lo contrario los tiempos y la longitud son lo mismo en los dos algoritmos 


![[Captura de pantalla 2026-10-14 a la(s) 3.59.02 p.m..png]]
![[Captura de pantalla 2026-10-14 a la(s) 4.00.58 p.m..png]]![[Captura de pantalla 2026-10-14 a la(s) 4.03.56 p.m..png]]![[Captura de pantalla 2026-10-14 a la(s) 4.05.01 p.m..png]]### Preguntas

**1. Sección “How does machine learning work?”** El artículo menciona tres tipos de aprendizaje. Anótalos y escribe con tus palabras en qué se diferencian.
aprendizaje supervisado:cuando el algoritmo aprende usando datos que ya vienen clasificados de manera correcta o incorrecta, el objetivo es clasificar los nuevos datos teniendo como referencia los anteriores
Aprendizaje sin supervisión: El modelo analiza datos que no tienen etiquetas ni respuestas previas. Su propósito es explorar la información, agruparla y descubrir patrones o relaciones ocultas por sí mismo.
**2. Sección “What is machine learning used for?”** Elige una aplicación (reconocimiento de imágenes, diagnóstico médico, conducción automática, texto y voz) y describe con las ideas de la clase de qué se trata: ¿cuál sería la tarea (T) y qué datos serían la experiencia (E)?
Tarea (T): Procesar la información del entorno para tomar decisiones de navegación seguras en tiempo real (acelerar, frenar, girar, evitar obstáculos).
Experiencia (E): Todos los datos en tiempo real e históricos captados por los sensores del vehículo mientras circula y reacciona al tráfico.
3.⁠ ⁠Sección “When to use machine learning?”
¿Cuándo usarlo? Conviene usar ML cuando los métodos tradicionales no pueden procesar enormes volúmenes de datos estadísticos o cuando no es posible resolver el problema con reglas fijas o cálculos simples debido a la complejidad de los patrones.
Ejemplo donde NO convendría: El cálculo del IVA o de impuestos fijos sobre una compra. Al ser una regla matemática exacta y sin variación, se resuelve mejor con programación tradicional basada en reglas lógicas.
4.⁠ ⁠Sección de aplicaciones, “Fraud detection” y “Anomaly detection”
Por qué tiene sentido el enfoque no supervisado: Como los fraudes raros o complejos no suelen tener un patrón conocido previa ni datos explícitamente categorizados, los modelos no supervisados pueden aprender lo que es "normal" y detectar cualquier irregularidad nueva que un humano no vería.
Problema del modelo supervisado: Necesita datos previamente etiquetados como "fraude" para aprender. Si surge un tipo de fraude nuevo que nunca antes fue etiquetado, el modelo supervisado no sabrá reconocerlo y no lo detectará.
5.⁠ ⁠Sección de aplicaciones, “Healthcare”
Elegí el sector de Salud (Cuidado de la salud):
El peor error: El falso negativo (decirle a un paciente que está sano cuando en realidad tiene una enfermedad o insuficiencia cardíaca).
Por qué: Si el modelo falla dando un falso negativo, el paciente no recibirá el tratamiento médico necesario a tiempo, lo que pone en riesgo directo su vida. Un falso positivo, en cambio, solo llevaría a realizar pruebas adicionales para desmentir la falsa alarma.
6.⁠ ⁠Sección “Machine learning examples by company”
Elegí el caso de Amazon:
Datos que usa el sistema: El historial de compras, las búsquedas realizadas y la navegación que hace el usuario en la plataforma.
Quién se beneficia: Tanto Amazon (porque aumenta sus ventas) como el comprador (porque recibe recomendaciones de productos útiles e interesantes para él).
Quién sale perjudicado: El usuario en el ámbito de su privacidad, ya que toda su actividad es rastreada continuamente para influir en sus decisiones de compra.
7.⁠ ⁠Lectura crítica
Lo que me hace dudar de la información del artículo:
Promesa del título incumplida: El título dice que habrá "12 aplicaciones y ejemplos", pero al revisar el texto solo se enumeran 11 áreas/aplicaciones principales antes de pasar a promocionar sus propios servicios.
Conflicto de interés y métricas infladas: El artículo lo escribe Helpware Tech (una empresa que vende servicios de consultoría de ML) y dan cifras como "6X CTR", "3X CVR" u "80% de precisión" sin explicar la metodología de medición ni dar pruebas objetivas.

Actividad 3.4
Como se benefician las GPU's de las redes neuronales y viceversa?
1. ¿Cómo se benefician las Redes Neuronales de las GPUs?

Las redes neuronales, especialmente el _Deep Learning_ (aprendizaje profundo), requieren realizar miles de millones de operaciones matemáticas simples de forma simultánea. Las GPUs están diseñadas exactamente para eso.

- **Procesamiento masivo en paralelo:** A diferencia de una CPU (que tiene pocos núcleos pero muy rápidos para tareas secuenciales), una GPU tiene **miles de núcleos más pequeños** diseñados para manejar múltiples tareas a la vez. Esto permite calcular los pesos y sesgos de millones de neuronas simultáneamente.

- **Aceleración de operaciones de álgebra lineal:** El entrenamiento de una red neuronal consiste casi en su totalidad en **multiplicaciones de matrices y sumas de vectores**. Las GPUs destacan en este tipo de matemáticas, reduciendo el tiempo de entrenamiento de meses a solo horas o días.

- **Hardware especializado (Tensor Cores):** Las GPUs modernas (como las arquitecturas Tensor de NVIDIA) incluyen núcleos dedicados exclusivamente a acelerar las operaciones de matriz utilizadas en IA, lo que multiplica la eficiencia energética y la velocidad de cómputo.

- **Ancho de banda de memoria masivo:** Mover los gigantescos conjuntos de datos (datasets) a través del procesador requiere conexiones ultrarrápidas. Las GPUs utilizan memorias de alta velocidad (como HBM o GDDR) que evitan los cuellos de botella al alimentar la red neuronal con datos.
2. ¿Cómo se benefician las GPUs de las Redes Neuronales?

El éxito de las redes neuronales transformó por completo la industria de los gráficos por computadora y redefinió el propósito de las GPUs.

- **Evolución arquitectónica y nuevos mercados:** Originalmente creadas solo para videojuegos, el éxito de la IA obligó a empresas como NVIDIA, AMD e Intel a rediseñar sus chips. Esto creó un mercado multimillonario en centros de datos e IA que hoy supera los ingresos del sector de los videojuegos.

- **Mejora de gráficos mediante IA (DLSS y FSR):** Las GPUs utilizan redes neuronales integradas para **renderizar imágenes a menor resolución y reescalarlas inteligentemente en tiempo real** (técnicas como NVIDIA DLSS o AMD FSR). Esto permite que los videojuegos corran al doble de fotogramas por segundo con un consumo de energía menor.

- **Generación de fotogramas y Ray Tracing:** Las redes neuronales dentro de la GPU ayudan a predecir e interpolar fotogramas completos (Frame Generation) y a "limpiar" el ruido visual que genera el cálculo de iluminación realista (_Ray Tracing_) mediante algoritmos de _denoising_ basados en IA.

- **Optimización del propio silicio:** Los ingenieros ahora utilizan redes neuronales para **diseñar la próxima generación de GPUs**, optimizando el acomodo de los transistores en el chip para que consuman menos energía y disipen mejor el calor.
- 