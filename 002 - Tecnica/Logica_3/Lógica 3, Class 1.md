#tecnica 
Jcardona904@gmail.com
3108232300

### Vectores
Son estructuras de datos similares a los arreglos, pero mas desarrollados que entre otras cosas, crecen y decrecen dinamicamente, según se necesite. En algunos lenguajes. En algunos lenguajes el tamaño de arreglo queda fijo en tiempo de compilación.

A vector is like a box that holds information, numbers or text.


### fixed-size vector (Estructura Fija)

This is just a way to user input into a vector. Apparently to print them complintly it needs a loop all the time, since it works like a list or tuple.

Example in Pseint:

```python
Algoritmo sin_titulo
	
	Dimension vector[5] #Crear Vector vacio
	
	para i = 1 Hasta 5 Hacer # LLenar el vector ex: 1 5 8 3 6
		Escribir "Ingresa el valor en la posicion", i
		Leer  vector[i]
	FinPara
	
	#Para Mostrar el vector lleno
	para i = 1 hasta 5 Hacer
		Escribir vector[i]
	FinPara
	
FinAlgoritmo
```

Example in python:
```python
def llenar_Vector():
    vector = [0]*5 #Definir o iniciar el vector
    for i in range(5): #llenar vector
        vector[i]=int(input(f"Ingrese el valor en la posicion:")) #1 5 8 3 6
    print(vector) #Imprimir Vector

llenar_Vector()
```

Final Resul of both:

| 1   | 2   | 3   | 4   | 5   |
| --- | --- | --- | --- | --- |
| 1   | 5   | 8   | 3   | 6   |


### Practice_1

We practiced the loop and understood how it worked, we had to:

Crear un vector de 20 posiciones con los numeros ingresados por el usuario y solo Mostrar los 10 primeros numeros del vector

```python
vector = [0]*20
#enter the numbers
for i in range(20):
	vector[i] = int(input("Ingresa un numero para el vector: "))

#Print only up to the 10th index
for i in range(10):
	print(vector[i])
#This is aquivalent to Ejercicio_2
```

### Practice_2

Crear un vector de 20 posiciones, con numeros aleatorios, buscar entre todo el vector el numero solicitado por el usuario, imprimir el vector resultante lleno y mostrar cuantas veces esta el numero buscado dentro del vector.

para saber si el numero buscado esta dentro del vector usamos "If" para que si "for loop" en el debido momento esta pasando por el numero buscado sume 1 al contador.

```python
import random
vector = [0]*20

# makes random numbers and puts them in vector
for i in range(20):
	vector[i]=random.randrange(1,20)

#Prints vector
for i in range(20):
	print(vector[i])

search = int(input("What number do you want to search for?: "))
count = 0

#Sums 1 to the counter if the number is found
for i in range(20):
	if vector[i] == search:
		count += 1

print ("The number was found ",count," Times in the vector")
#This is aquivalent to Ejercicio_3
```



### Practice_3

crear un vector de 5 posiciones con numeros ingresados por el usuario de forma desordenada, mostrar el vector ingresado y Mostrar el vector ordenado

la explicacion de la forma que se organizan es muy fastidiosa de explicar necesito obtener un mejor entendimiento, aun asi lo intentare: 

##### Explicacion Logica de organizacion,Tipo burbuja.

"i" es el index que va por atras y "j" va por delante por ejemplo si "i" esta en el index 2(8) y "j" esta en el index 3,(5) 

| 1   | 2   | 3   | 4   | 5   |
| --- | --- | --- | --- | --- |
| 3   | 8   | 5   | 2   | 4    |


si el index 2(8) es mayor al index 3(5), el index "i" se manda a un auxiliar para guardar la informacion:

	AUX = vector[i] or AUX = 8

y despues el index 2(8 -> 5) se convierte en el index "j"(8):

	vector[i] = vector[j]


por ultimo el index "j" se convierte en el auxiliar:

	vector[j] = aux


un intento de representacion ilustrada se veria como:


paso 1:

| -   | i   | j   | -   | -   | aux = 0    |
| --- | --- | --- | --- | --- | --- |
| i1  | i2  | i3  | i4  | i5  |     |
| 3   | 8   | 5   | 2   | 4   |     |

paso 2: es i mayor a j? SI

| -     | i     | j     | -     | -     | aux =  8 |
| ----- | ----- | ----- | ----- | ----- | -------- |
| 1     | 2     | 3     | 4     | 5     |          |
| **3** | **8** | **5** | **2** | **4** |          |

paso 3: index[i] = index[j]

| -     | i     | j     | -     | -     | aux = 8 |
| ----- | ----- | ----- | ----- | ----- | ------- |
| 1     | 2     | 3     | 4     | 5     |         |
| **3** | **5** | **5** | **2** | **4** |         |

paso 4: ultimamente index j se convierte en el auxiliar:

| -     | i     | j     | -     | -     | aux = 8 |
| ----- | ----- | ----- | ----- | ----- | ------- |
| 1     | 2     | 3     | 4     | 5     |         |
| **3** | **5** | **8** | **2** | **4** |         |

Todo esto va en dos For loops uno para j y otro para i estos For Loops se llevaran acabo tantas veces como el vector mism el vector "j" sera el que controle el if statement.

Codigo en python:

```python
for i in range(5):
	vector[i]= int(input("Enter the number:")) #Well inputs the vector

for i in range(5):
	print(vector[i]) # Prints unorganized vector

for i in range(5):
	for j in range(5):
		if vector[i] > vector[j]: #Organization logic
			aux = vector[i]
			vector[i] = vector[j]
			vector[j] = aux

print(" ")#Forgot how to do backslash
print("Organized") 

for i in range (5):  # Prints now organized vector
	print (vector[i])

#This is aquivalent to Ejercicio_5
```








