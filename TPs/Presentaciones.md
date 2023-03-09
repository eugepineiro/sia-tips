# Presentaciones

Algunas recomendaciones para la presentación de los TPs son:

## Modalidad

La presentación de los Trabajos Prácticos de la materia consiste en una serie de filminas donde al comienzo deben presentarse todos los integrantes del equipo, luego se describen los parámetros utilizados y los detalles de implementación que se crean pertinentes. 

Al final de cada ejercicio se muestran los resultados y se deben sacar conclusiones a partir de esos resultados. 

Todos los integrantes del grupo tienen que hablar, se recomienda ir turnandose cada 1 o 2 filminas (no dividirse por ejercicio ya que todos deben tener conocimiento sobre todos los temas) 

## No Dejar la Presentación para Último Momento

Siempre, a la hora de hacer los TPs, se debe tener en cuenta que un tiempo debe serle dedicado al armado de la Presentación.

El desarrollo del TP suele consistir en una implementación básica de los problemas propuestos en una primera instancia, luego se comienza a experimentar y, finalmente, se hace la presentación. No obstante, se debe tener en cuenta que durante el armado de la presentación suelen surgir nuevas ideas o correcciones o necesidad de implementar más cosas o recolectar más datos.

Por todo lo mencionado, es recomendable que no se realice la Presentación a último momento.

## Pensar: ¿Qué Quiero Presentar?

La idea principal de estos trabajos prácticos es apelar a su curiosidad. Prueben, experimenten, generen hipótesis sobre lo que debería suceder y comprueben o refuten.

En muchas ocasiones pensamos "Si pasa esto, seguro pasa esto otro", ¿seguro? Ese es un muy buen momento de poner manos a la obra y observar si es así. Todo es solo cuestión de cuestionar preguntandose "¿Por qué es así? ¿Es así? ¿Por qué no es asá?"

## Evitar Mostrar Código y Recaer en Detalles Técnicos de Implementación

El lenguaje en el que se desarrolló el TP, el Diagrama de Clases, versiones de librerías entre otras cosas ocupan tiempo de presentación y no suman por lo que es preferible no incluirlo pero sí tenerlo en mente en caso de que se haga un pregunta sobre eso.

Antes de incluir algún detalle de implementación esta bueno pensar si el mismo es relevante para el problema o el resultado obtenido. Esto no significa descartar todo detalle de implementación ya que cuestiones interesantes pueden surgir de la misma y puede ser fructífero explorarlas.

## Evaluación de Parámetros

Es importante para todos los trabajos prácticos definir los parámetros a utilizar y plasmar en la filmina qué parámetros se utilizaron para obtener los resultados que están mostrando. (Por Ej: tasa de aprendizaje, arquitectura de red, etc.). Esto se debe a que muchos resultados se ven afectados por el cambio de parámetros. Para comparar cómo afectan los parámetros a los resultados se debe variar un parámetro y fijar todos los demás. Es muy importante a la hora de evaluar resultados variar los parámetros, experimenten! 

## Practicar la Presentación Anteriormente

A la hora de exponer un tema, es una buena práctica repasar lo que se va a exponer y más si es un grupo. Practicando se facilita lo que les recomendamos más abajo, evita olvidarse de algo que se quería mencionar, evita que nos trabemos y evita el no saber quien va o que hable una sola persona mucho tiempo.

## Los Miembros del Grupo Hablen de Manera Intercalada

Se debería buscar que la división sea equitativa y no del estilo "Yo presento el problema 1 y vos el problema 2".

Tener en cuenta que es requisito para la aprobación de los TPs que todos los miembros conozcan como resolvieron todo lo concierne a cada TP. Esta estrategía es una buena manera de afianzar todo y no únicamente focalizarse en un tema particular de los abordados por el TP.

Tener presente que en el caso de que sólo un miembro del equipo presente un ejercicio o tema particular sus compañeros sean interpelados.

## Incluir Gráficos Representativos para los Datos que se Muestren

Los datos se pueden mostrar de muchas formas como sueltos, con tablas o con gráficos.

En cada caso esta bueno evaluar cuál es la mejor manera de mostrarlos por varios motivos: nos ayuda a mostrar mejor alguna cuestión y, ¡podemos encontrar algo de interés observandolo! 

Puede ser que algo que con los datos crudos jamás ibamos a encontrar, aparezca tan claro como el agua (y a veces no tanto) en un gráfico. 

Los gráficos tienen que tener los nombres de los ejes y la escala especificada. Cada gráfico tiene que tener una razón por la cual estar, para representar un resultado particular que quieren mostrar.


## Conclusiones 

Las conclusiones son muy importantes a la hora de mostrar los resultados. Si se muestra un gráfico se debe interpretar qué nos está diciendo ese gráfico, que información aporta al caso de uso. Las conclusiones deben surgir a partir de los resultados que ustedes presenten (no de las filminas de la teoría).

## Algoritmos Estocásticos 

Los algoritmos que vemos en la materia son estocásticos. Por lo tanto, trabajan con semillas de números aleatorios que tienen que manejar con cuidado.  Por ejemplo, pueden fijar una semilla particular para reproducir resultados. La idea entonces es que vean la evolución de los algoritmos en muchas ejecuciones, y mostrar los resultados en relación a promedios de corridas.  Pueden usar barras de errores en los gráficos para mostrar este tipo de información.

**Al momento de presentar mediciones de cantidades estocásticas nunca presentar mediciones únicas.** Ejemplos de cantidades estocásticas incluyen el tiempo de ejecucion de los programas o el mejor fitness encontrado por el motor de algoritmos geneticos. Para reportar mediciones de estas cantidades **lo que se busca es dar a entender las distribuciones que se observaron durante los experimentos**. 

Una manera de lograr esto ultimo es realizando varias mediciones (ejecutar múltiples veces el programa), promediándolas entre sí y calculando su desvío estándar. 

Por ejemplo, en vez de presentar
| Algoritmo | Tiempo de ejecución |
|--|--|
| DFS | 43ms |
| BFS | 103ms |

presentar algo de este estilo:

| Algoritmo | Tiempo de ejecución |
|--|--|
| DFS | 40ms +- 2ms |
| BFS | 100ms +- 1ms |

donde 40ms y 100ms son los promedios de los tiempos de ejecución para cada método, y 2ms y 1ms los respectivos desvíos estándar.

## Archivo de Configuración 

Todos los trabajos prácticos cuentan con múltiples parámetros para evaluar. Se aconseja tener un archivo de configuración .json o .yml (o lo que les parezca más cómodo) para que les resulte más sencillo variarlos. 

## Archivo README.md

El repositorio deberá contar con un archivo README.md con la documentación correspondiente de cada uno de los parámetros mencionados en el archivo de configuración y cómo se ejecuta el programa.

