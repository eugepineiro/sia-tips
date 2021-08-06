# Métodos de Búsqueda 

El objetivo del trabajo práctico es crear un generador de soluciones para el juego [Sokoban](http://www.game-sokoban.com/index.php?mode=level&lid=200)

## Tips

#### 1. Estados Muertos 
Considerar que hay ciertas situaciones en las que ya no se puede llegar a la solución: 
- Una posición con esquina de paredes 
- Una pared inmoviliza un eje de movimiento de la caja 
- Una caja bloquea otra caja

#### 2. Estados Repetidos
- No regresar al estado padre 
- No crear rutas con ciclos
- No expandir estados que ya extendí
- Ojo: trade-off con costo computacional

#### 3. Diseño de tableros
- Probar los algoritmos con tableros sencillos para poder realizar el seguimiento 
- En esta [página](http://www.game-sokoban.com/index.php?mode=level&lid=200) pueden acceder a tableros en ASCII. 
- Si usan los mismos caracteres que otros grupos se pueden compartir tableros y comparar resultados (puede llegar a ser una buena métrica para saber si tiene algún error de implementación)

#### 4. Heurísticas 
Las heurísticas informan al agente en su búsqueda y lo ayudan a evitar caminos inútiles
- ¿De qué forma la heurística ayuda al agente? 
- ¿Qué caminos lo hacen favorecer y cuáles evitar?
Una forma de derivar heurísticas consiste en inspeccionar los caminos recorridos por los métodos no informados. Siempre vamos a notar caminos que sabemos que no llevan a la solución, o bien pasos que no tienen sentido. ¿Cómo lo “codificamos” en una heurística?

## Links útiles 
[Juego de los Edificios](psicoactiva.com/juegos-inteligencia/area-espacial/rascacielos)


