# A---HEURISTICA---Teoria-juego

**1. Algoritmo A***
¿Qué es A*?

El Algoritmo A* es un algoritmo de búsqueda informada utilizado para encontrar el camino más corto entre dos nodos en un grafo.

Se usa mucho en:

* Videojuegos
* Sistemas GPS
* Robótica
* Inteligencia artificial

A* combina dos cosas:

- Costo real recorrido
- Estimación del costo que falta

Su función principal es:

**𝑓(𝑛)=𝑔(𝑛)+ℎ(𝑛)**

Donde:

g(n) = costo desde el nodo inicial hasta n

h(n) = heurística (estimación hasta el objetivo)

¿Cómo funciona A*?

Empieza en el nodo inicial.
Calcula el costo de cada nodo vecino.
Escoge el nodo con menor valor de f(n).
Repite hasta llegar al objetivo.

En resumen:

A* busca siempre el camino más prometedor.

Ejemplo de uso

Un mapa tipo laberinto
------------------------
S . . X .
. X . X .
. X . . .
. . X X .
. . . . G

S = inicio
G = objetivo
X = obstáculo

A* buscará el camino más corto evitando obstáculos.

Si deseas probar el algoritmo directamente en línea:

👉 Ir a [astar_animado_py.ipynb](https://colab.research.google.com/drive/19FCcajeWRCiwZagbx92gF_AGYZHeX7Z9?usp=sharing)

-------------------------------------
-------------------------------------
**2. Heurística**
¿Qué es?

Una heurística es una regla o método que ayuda a tomar decisiones rápidas para encontrar soluciones.
En inteligencia artificial:
Es una estimación de qué tan cerca estamos de la solución.

¿Para qué sirve?

Sirve para:

acelerar algoritmos
reducir cálculos
encontrar soluciones más rápido

Por ejemplo:

GPS no prueba todas las rutas, usa estimaciones.

¿Cómo funciona?

La heurística calcula un valor aproximado:

EJEMPLO #1. El Viajante de Comercio (Heurística: Vecino más Cercano)
Este es un problema de optimización. La heurística aquí es: "Desde donde estoy, ve a la ciudad más cercana que no haya visitado". Es fascinante ver cómo se van trazando las líneas.
-----------------------------------------
👉 Ir a [viajantecomercio.ipynb](https://colab.research.google.com/drive/1vT7nWTumyqy8-mb9D5xgfQ69qWlT57kS?usp=sharing)
----------------------------------------

EJEMPLO #2. Manhattan vs. Euclídea (La "Forma" de la búsqueda)
podemos comparar cómo cambia la mancha de expansión de un algoritmo según la heurística.

Manhattan: Explora en forma de "diamante" (cuadrado rotado).
Euclídea: Explora en forma de "círculo".

Este código genera un mapa vacío y verás cómo la heurística "dirige" el crecimiento de forma orgánica.
----------------------------------------
👉 Ir a [Manhattan.ipynb](https://colab.research.google.com/drive/14Z9x28-ttsX3XL9zC9CtVWEz7YD5PGW3?usp=sharing)
----------------------------------------

-----------------------------------------
**3. Teoría de Juegos**

¿Qué es?

La teoría de juegos estudia cómo toman decisiones los jugadores cuando sus decisiones afectan a otros.

Se usa en:

economía
política
inteligencia artificial
negociación
videojuegos

**¿Para qué sirve?**

Permite:
predecir comportamientos
encontrar estrategias óptimas
analizar conflictos

**¿Cómo funciona?**

Cada juego tiene:

jugadores
estrategias
recompensas

Los jugadores buscan maximizar su ganancia.

