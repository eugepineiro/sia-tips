# Métodos de Búsqueda 

El objetivo del trabajo práctico es crear un generador de soluciones para distintos juegos como el [Sokoban](http://www.game-sokoban.com/index.php?mode=level&lid=200), [8 Puzzle]([psicoactiva.com/juegos-inteligencia/area-espacial/rascacielos](https://camo.githubusercontent.com/59b1fbe9a5574e01cb73240f565a1a7cacd63385c81ba0fb74552fb5229c5fae/68747470733a2f2f6d69726f2e6d656469756d2e636f6d2f6d61782f3932342f312a5978655a4a7a666857346b6e354f35774147626b49672e676966)), [Cubo Rubik](https://es.wikipedia.org/wiki/Cubo_de_Rubik), [Fill-Zone](http://www.mygamesworld.com/game/7682/Fill_Zone.html), entre otros.

## Tips

### Implementación 

#### 1. Estados Muertos 
Considerar que hay ciertas situaciones en las que ya no se puede llegar a la solución. Por Ejemplo, para el Sokoban:
- Una posición con esquina de paredes 
- Una pared inmoviliza un eje de movimiento de la caja 
- Una caja bloquea otra caja

#### 2. Estados Repetidos
- No regresar al estado padre 
- No crear rutas con ciclos
- No expandir estados que ya expandí
- Ojo: trade-off con costo computacional

#### 3. Diseño de tableros
- Probar los algoritmos con tableros sencillos para poder realizar el seguimiento 
- En esta [página](http://www.game-sokoban.com/index.php?mode=level&lid=200) pueden acceder a tableros en ASCII del Sokoban. 
- Si usan los mismos caracteres que otros grupos se pueden compartir tableros y comparar resultados (puede llegar a ser una buena métrica para saber si tiene algún error de implementación)

#### 4. Heurísticas 
Las heurísticas informan al agente en su búsqueda, le dan información sobre qué tan cerca está el estado actual del estado objetivo. Esto les permite explorar en primer lugar los caminos más prometedores.
A la hora de definir una heurística se pueden plantear preguntas como: 
- ¿De qué forma la heurística ayuda al agente? 
- ¿Qué caminos lo hacen favorecer y cuáles evitar?
Una forma de derivar heurísticas consiste en inspeccionar los caminos recorridos por los métodos no informados. Siempre vamos a notar caminos que sabemos que no llevan a la solución, o bien pasos que no tienen sentido. ¿Cómo lo “codificamos” en una heurística?
Tener en cuenta cómo es la heurística, si es admisible entonces no sobreestima el costo real. 
Evitar utilizar heurísticas triviales porque termina aportando más el costo de la solución que la misma heurística. Por ejemplo, para el Sokoban una heurística trivial sería la cantidad de cajas por ubicas o la cantidad de objetivos. 

### Presentación de Resultados 

- Es importante la comparación entre los distintos métodos de búsqueda. ¿Cuál es conveniente utilizar en cada caso? ¿Cuándo performa uno mejor que otro? ¿Los resultados son los mismos para todos los problemas? 

Recordatorio: A la hora de comparar tiempos ejecución se debe correr el algoritmos múltiples veces, realizar un promedio y calcular el desvío estándar.

## Links útiles 

#### Otros juegos similares
[Juego de los Edificios](psicoactiva.com/juegos-inteligencia/area-espacial/rascacielos)

[8 Puzzle]([psicoactiva.com/juegos-inteligencia/area-espacial/rascacielos](https://camo.githubusercontent.com/59b1fbe9a5574e01cb73240f565a1a7cacd63385c81ba0fb74552fb5229c5fae/68747470733a2f2f6d69726f2e6d656469756d2e636f6d2f6d61782f3932342f312a5978655a4a7a666857346b6e354f35774147626b49672e676966))

[Sokoban](https://en.wikipedia.org/wiki/Sokoban#/media/File:Sokoban_ani.gif)


