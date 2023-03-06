# Multiagentes-Integradora

# **Simulador Robot de Limpieza - M1. Actividad (FJ2023)**

Esteban Martinez - A00831789

<center>
<img src=https://topesdegama.com/app/uploads-topesdegama.com/2022/02/robot-aspiradora-roomba.jpg?x=480&y=375&quality=40 />
</center>

## **Explicación**


### **a. Describe la situación y/o problema a simular**
b. Describe los agentes involucrados así como sus acciones y percepciones
c. Describe cómo interactúan y se comunican dos o más agentes del mismo 
d. Describe el entorno
e. Identifica  las  variables  y  los  parámetros  que  determinan  el  funcionamiento  del 
sistema.
f. Describe el proceso de simulación
g. Discute clara y concisamente los resultados obtenidos
h. Agrega el link al repositorio.


El programa implementado hace una visualización de lo que serían los robots tipo Roomba, los cuales limpian una cuadrícula con base a la suciedad que se encuentre. Primero, se tendría que definir el tamaño de la cuadrícula y la posición inicial de cada uno de los robots.

Luego, se implementaría un ciclo que ejecutara los movimientos de los robots en cada paso, siempre y cuando no se cumplan ciertas condiciones de detención (como por ejemplo, que hayan limpiado toda la cuadrícula o que se hayan agotado la batería de los robots (pasos)).

En cada paso, se verificaría si el robot puede moverse a la siguiente posición en la cuadrícula sin chocar con otros robots o salirse de la cuadrícula. Si el movimiento es válido, el robot se movería a la nueva posición y limpiaría la casilla en la que se encuentra, o si no vuelve a buscar una casilla a limpiar. Si el movimiento no es válido, el robot no se mueve y simplemente limpia la casilla en la que se encuentra.

Una vez que se hayan ejecutado todos los pasos para cada robot, el programa mostrará el estado final de la animación por medio que se pueda observar si se limpió por completo la cuadricula.
