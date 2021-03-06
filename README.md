tsp-tabusearch
==============

El problema del viajante (TSP), es comúnmente utilizado para mostrar la funcionalidad de la búsqueda tabú. 

El TSP requiere buscar un orden en el cual viajar entre ciudades, tal que la distancia recorrida sea minimizada. Por ejemplo, si las ciudades A y B están una al lado de la otra, mientras que la ciudad C está más lejos, la distancia total recorrida será más corta si las ciudades A y B son visitadas una después de la otra, antes de visitar C. Como encontrar un orden óptimo para visitar las ciudades en el TSP es un problema NP-difícil. los métodos de aproximación basados en heurísticas son útiles para lograr la optimalidad.

La búsqueda tabú puede utilizarse para encontrar una solución satisfactoria para el TSP. Primero, la búsqueda tabú comienza con una solución inicial, que puede ser generada con el algoritmo del vecino más cercano. Para crear nuevas soluciones, el orden en que dos ciudades son visitadas es intercambiado. La distancia total recorrida entre todas las ciudades es utilizada para juzgar cuanto mejor es una solución de otra. Para prevenir ciclos y para salir de los óptimos locales, una solución es agregada a la lista tabú si es que es aceptada en N*(x), el vecindario de soluciones. Se continuan creando nuevas soluciones hasta que algún criterio de parada, como por ejemplo un número arbirtrario de iteraciones, es encontrado. Una vez que la búsqueda tabú se detiene, la mejor solución es aquella que cuya distancia total a recorrer entre las ciudades es la menor.
