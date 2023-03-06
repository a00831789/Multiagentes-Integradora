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

### **g. Discute clara y concisamente los resultados obtenidos**

### **h. Agrega el link al repositorio.**
