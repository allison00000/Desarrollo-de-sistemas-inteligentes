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