#tecnica 
Jcardona904@gmail.com
3108232300
## What did we learn?

He didn't teach anything "new" we just did some exercises about filling a matrix with a vector

### Practice_1

Crear un vector de 4 posiciones con números primos menores que 10 y mostrar el vector

```python
primes = [2,3,5,7]

for i in primes:
	print(i)
	
#This is equivalent to Ejercicio_1
```

### Practice_2

Crear una matriz de 20 x 20 con los números primos (2,3,5,7) aleatorios, contar cuantas veces esta el numero 7 en la matriz antes de esto mostrar la matriz llena. Como se vio en el pseudocodigo de pseint hacer que se llene de forma aleatoria es mucho mas simple que de forma ordenada

```python
import random

matrix = [[0] * 20 for i in range(20)]
primes = [2,3,5,7]

amount = 0

for rows in range(20):
	for columns in range(20):
		random_primes = random.choice(primes) #Random.Choice randomizes the next choice lol
		matrix[rows][columns] = random_primes

for row in matrix: #por cada linea an la matrix
	for element in row: # Y por cada elemento en esta linea
		if element == 7: # si este elemento es 7
			amount += 1 # cantidad mas 1


print("Filled Matrix")
for row in matrix:
	print(row)

print("\n Amount of times the number 7 is found: ",amount,"\n")

#This is equivalent to Ejercicio_2
```

### Practice_3

crear una matriz 3 x 3 mostrar la matriz llena y mostrar el valor de la mitad de la matriz

```python
import random

matrix = [[0]*3 for i in range(3)]

for row in range(3):
	for column in range(3):
		matrix[row][column] = random.randrange(1,10)

for row in matrix:
	print(row)

print("\nThe Value in the middle is: ",matrix[1][1],"\n")

#This is equivalent to Ejercicio_3
```

### Practice_4

Crear una matriz 20 x 20 llenarla con las vocales,mostrar la matriz llena, contar cuantas veces esta la vocal "o". 

Fun fact: Hice todo el código sin poblarlo ni una vez, lo hice todo de corrido sin ver código pasado no lo probe hasta que pensé que estaba terminado y no tuvo ningún error.

```python
import random

matrix = [[0] * 20 for i in range(20)]
vocales = ["a","e","i","o","u"]

for row in range(20):
	for column in range(20):
		matrix[row][column] = vocales[random.randrange(0,5)]

for row in matrix:
	print(row)

amount = 0
for row in matrix:
	for element in row:
		if element == "o":
			amount += 1

print("\nThe amount of letters 'O' inside the matrix are: ",amount)

#This is equivalent to Ejercicio_4
```

### Practice_5

Crear una matrix 4 x 4 y llenarla con los signos zodiacales obviamente también se debe mostrar

```python
import random

matrix = [[0] * 4 for i in range(4)]
signos_zodiaco = ["Aries","Tauro","Geminis","Cancer","Leo","Virgo","Libra","Escorpio","Sagitario","Capricornio","Acuario","Picsis"]

for row in range(4):
	for column in range(4):
		matrix[row][column] = signos_zodiaco[(random.randrange(0,11))]

for row in matrix:
	print(row)

#This is equivalent to Ejercicio_5
```