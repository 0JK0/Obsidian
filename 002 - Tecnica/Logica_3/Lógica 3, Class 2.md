#tecnica 
Jcardona904@gmail.com
3108232300

### Matriz

Un arreglo o matriz es una coleccion ordenada de datos, se emplean para almacenar multiplesa valores en una sola variable frente a las variables que solo pueden almacenar un valor por cada variable.

se divide en columnas y lineas Cada elemento del arreglo (matriz) tiene un número al que está asociado
llamado "índice numérico" (numeric index), que permite acceder a él. 

**Testing matriz**

| -   | C1  | C2  | C3  | C4  |
| --- | --- | --- | --- | --- |
| F1  | 4   | 5   | 6   | 7   |
| F2  | 8   | 9   | 5   | 3   |
| F3  | 2   | 1   | 4   | 6   |
| F4  | 9   | 8   | 7   | 1   |


### Practice_1

Crear un algoritmo con un vector de 5 posiciones, donde se ingresen las notas de un estudiante; Mostrar el vector resultante y el promedio de las notas.
 
Bastante sensillo solo se suman las notas en el acumulador suma y despues se dividen por 5.

```python
vector = [0]*5
suma = 0

for i in range(5):
	vector[i] = float(input("Ingrese una nota: "))
	suma += vector[i]

promedio = suma / 5
for i in range(5):
	print(vector[i])

print("El Promedio de las notas es: ",promedio)
#This is aquivalent to Ejercicio_1
```

### Practice_2

El profesor hizo un ejemplo de como se llena y se escribe en una matriz.

Despues se muestra solo la diagonal principal de la matriz osea la dioganal de : F1-C1 hasta C4-F4

```python
#This works by 1st defines the columns and then a loop for the rows
matriz = [[0] * 4 for i in range(4)]

#Filling the Matrix
for i in range(4):
	for j in range(4):
		matriz[i][j] = int(input("Ingrese el valor : "))

#Prints the matrix with a simple loop
for fila in matriz:
	print(fila)

#Prints only diagonal
for i in range(4):
	for j in range(4):
		if i == j:
			print(matriz[i][j])

#This is aquivalent to Ejercicio_3
```

