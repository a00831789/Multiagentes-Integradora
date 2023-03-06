# Multiagentes-Integradora

# **Simulador Robot de Limpieza - M1. Actividad (FJ2023)**

Esteban Martinez - A00831789

<center>
<img src=https://topesdegama.com/app/uploads-topesdegama.com/2022/02/robot-aspiradora-roomba.jpg?x=480&y=375&quality=40 />
</center>

## **Explicación**

### **a. Describe la situación y/o problema a simular**
Lo que busca esta simulación es como sería el funcionamiento de los de las limpiadoras Roomba, por medio de que las limpiadoras sean capaces de identificar las casillas sucias y limpiarlas. Así también se define al principio del programa el número de limpiadoras y su rango de distancias en el que pueden ver las casillas sucias
### **b. Describe los agentes involucrados así como sus acciones y percepciones**
Los agentes involucrados son las limpiadoras y la suciedad del piso (Cleaner y Dirt). 
Las limpiadoras tienen la capacidad de moverse en todo el grid predeterminado por medio de no chocar con otras limpiadoras, así también de poder identificar los spots en donde se encuentra sucio y poder desaparecer dicha suciedad.
El Dirt tiene la capacidad de aparecer en el grid de forma aleatoria conforme el piso lo defina.
### **c. Describe cómo interactúan y se comunican dos o más agentes del mismo** 
Las limpiadoras tienen la capacidad de moverse por todo el mapa sin afectar la simulación de las otras limpiadoras, por medio de respetar en el espacio que se ubican. Así también tienen la capacidad de analizar el grid en un rango determinado y así poder trabajar de una manera más inteligente por medio de dirigirse a todos los spots sucios sin perder mucho tiempo. Adicionalmente, están programados que cada limpiadora cuenta con un número de pasos para poder limpiar todo el grid, simulando en la vida real con el hecho que las limpiadoras cuentan con una batería.
La suciedad del piso aparece de forma aleatoria en el piso y no pueden aparecer suciedad encima de otra o fuera del grid.
### **d. Describe el entorno**
El modelo Floor tiene la capacidad de simular los agentes por medio de generar de forma aleatoria la suciedad que se va a encontrar en el piso como la posición de los robots predeterminados. Así también, cuenta con el data collector que se encarga el obtener la información de la simulación en cada paso por medio de poder mostrar como los robots van desapareciendo los spots sucios dentro del grid.
### **e. Identifica  las  variables  y  los  parámetros  que  determinan  el  funcionamiento  del sistema.**
Los inits del modelo Floor y los Agentes Cleaner y Dirt.
La función def random_list(inf, sup, n) para la clase Floor.

**Floor:**
* def populate(self, num_cleaners, num_dirt, cleaner_rad)
* def get_grid(self):
* def get_rem_dirt(self): 
* def step(self):

**Cleaner:**
* def choose_next_pos(self): 
* def find_dirt_pos(self):
* def closest_pos(self, positions): 
* def aproximate(self, dirt_pos): 
* def step(self):
* def advance(self):
### **f. Describe el proceso de simulación**
En esta simualción se declaran los colores en la matrícula tienen los siguientes significados:
* Blanco: espacio vacío.
* Negro: suciedad.
* Azul: robot de limpieza.

Por defecto aparecen 5 robots y conforme se haya indicado, estos contaran un rango de distancia para poder identificar los spots sucios.
En la simulación cada robots cuenta con 100 pasos para poder limpiar todo el grid y entre todos los robots se encargan de desaparecer todos los spots sucios (cuadros negros) hasta que no quede ninguno restante en el grid.
Así también que los robots no tienen la capacidad de salirse del grid como también de sobreponerse en el espacio que ya ocupe algúna otra limpiadora.
En caso de que no se limpie todo el grid, se mostrara el resultado que se pudo lograr entre todas las limpiadoras.
### **g. Discute clara y concisamente los resultados obtenidos**
Entre el número de robots dentro de la simulación como de su capacidad de inteligencia (rango de distancia para detectar espacios sucios), se determinó que un incremento en el número de robots de limpieza aumenta el número final de celdas limpias, pero dicho aumento es inferior al producido por un incremento en el radio de los 'sensores' de los robots, lo que indica que la 'inteligencia' de los robots es más determinante que el número de robots en la simulación.
### **h. Agrega el link al repositorio.**
[link text](https://github.com/a00831789/Multiagentes-Integradora.git)

