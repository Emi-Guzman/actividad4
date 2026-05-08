## COMMIT 1:
### Reposicion De los proyectiles
Los proyectiles vuelven al lado derecho de la pantalla en una altura aleatoria si salen de la ventana 


## COMMIT 2:

### Mejorando Velocidad de la Bola y los proyectiles.

#### Los Objetivos (Bolas Azules) 

Cambio: Se incrementó el valor de desplazamiento horizontal en la función move().

Línea modificada: target.x -= 0.5 $\rightarrow$ target.x -= 2.0 (o superior).

En cada ciclo del cronómetro (ontimer), el código resta una cantidad de píxeles a la posición X de cada objetivo para moverlos de derecha a izquierda. Al restar un número mayor, la distancia recorrida en el mismo tiempo es superior, lo que percibimos como una velocidad de traslación más alta.

 #### El Proyectil (Pelota Roja) 
 
 Cambio: Se redujo el denominador en la fórmula de impulso dentro de la función tap().

Línea modificada: speed.x = (x + 200) / 25 $\rightarrow$ speed.x = (x + 200) / 15.

La velocidad inicial del disparo se calcula dividiendo la distancia entre el clic y el origen. Al disminuir el divisor, el resultado de la operación matemática (el vector de velocidad) es más grande.


####  Autores:

Santiago Acosta Gaytan - a01827126

Jose Emiliano Guzman Arriega - a01826972

