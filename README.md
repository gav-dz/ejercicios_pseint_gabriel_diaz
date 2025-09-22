
---
### Ejercicio 1
Escribir un programa que pregunte al usuario su nombre, y luego lo salude.
```
Algoritmo ejercicio_1
	Definir nombre Como Caracter
	
	Escribir "Escriba su nombre: " Sin Saltar
	Leer nombre
	
	Escribir "Hola, ", nombre, "!"
FinAlgoritmo
```
---
### Ejercicio 2

Calcular el perímetro y área de un rectángulo dada su base y su altura.
```
Algoritmo ejercicio_2
	Definir b, h, perimetro, area Como Real
	
	Escribir "Ingrese el valor de base: " Sin Saltar
	Leer b
	Escribir "Ingrese el valor de altura: " Sin Saltar
	Leer h
	
	perimetro = 2 * (b + h)
	area = b * h
	
	Escribir "El perimetro es ", perimetro, " y el area es ", area
FinAlgoritmo
```
---
### Ejercicio 3

Dados los catetos de un triángulo rectángulo, calcular su hipotenusa.
```
Algoritmo ejercicio_3
	Definir catetoA, catetoB, hipotenusa Como Real
	
	Escribir "Ingrese cateto A: " Sin Saltar
	Leer catetoA
	Escribir "Ingrese cateto B: " Sin Saltar
	Leer catetoB
	
	hipotenusa = rc(catetoA^2 + catetoB^2)
	
	Escribir "La hipotenusa es ", hipotenusa
FinAlgoritmo
```
---
### Ejercicio 4
Dados dos números, mostrar la suma, resta, división y multiplicación de ambos.
```
Algoritmo ejercicio_4
	Definir n1, n2 Como Real
	
	Escribir "Ingrese número 1: " Sin Saltar
	Leer n1
	Escribir "Ingrese número 2: " Sin Saltar
	Leer n2
	
	Escribir "Suma de ambos números: ", n1 + n2
	Escribir "Resta de ambos números: ", n1 - n2
	Escribir "Multiplicación de ambos números: ", n1 * n2
	Escribir "División de ambos números: ", n1 / n2
FinAlgoritmo
```
---
### Ejercicio 5

Escribir un programa que convierta un valor dado en grados Fahrenheit a grados Celsius. Recordar que la fórmula para la conversión es:

```
C = (F-32)*5/9
```
```
Algoritmo ejercicio_5
	Definir C, F Como Entero
	
	Escribir "Ingrese los grados fahrenheit a convertir: " Sin Saltar
	Leer F
	
	C = (F - 32) * 5/9
	
	Escribir F, "°F son ", C, "°C"
	
FinAlgoritmo
```
---
### Ejercicio 6

Calcular la media de tres números pedidos por teclado.
```
Algoritmo ejercicio_6
	Definir n1, n2, n3, media Como Real
	
	Escribir "Ingresar primer número: " Sin Saltar
	Leer n1
	Escribir "Ingresar segundo número: " Sin Saltar
	Leer n2
	Escribir "Ingresar tercer número: " Sin Saltar
	Leer n3
	
	media = (n1 + n2 + n3) / 3
FinAlgoritmo
```
---
### Ejercicio 7

Realiza un programa que reciba una cantidad de minutos y muestre por pantalla a cuantas horas y minutos corresponde. Por ejemplo: 1000 minutos son 16 horas y 40 minutos.
```
Algoritmo ejercicio_7
	Definir totalMinutos, horas, minutos Como Real
	
	Escribir "Ingresar minutos: " Sin Saltar
	Leer totalMinutos
	
	horas = totalMinutos / 60
	minutos = totalMinutos % 60
	// totalMinutos - (horas * 60)
	
	Escribir totalMinutos, " minutos son ", TRUNC(horas), " horas y ", minutos, " minutos."
FinAlgoritmo
```
---
### Ejercicio 8

Un vendedor recibe un sueldo base mas un 10% extra por comisión de sus ventas, el vendedor desea saber cuanto dinero obtendrá por concepto de comisiones por las tres ventas que realiza en el mes y el total que recibirá en el mes tomando en cuenta su sueldo base y comisiones.
```
Algoritmo ejercicio_8
	Definir sueldoBase, v1, v2, v3, comisionTotal, sueldoTotal Como Real
	
	Escribir "Escribir sueldo base: " Sin Saltar
	Leer sueldoBase
	
	Escribir "Escribir valor de la primera venta: " Sin Saltar
	Leer v1
	Escribir "Escribir valor de la segunda venta: " Sin Saltar
	Leer v2
	Escribir "Escribir valor de la tercer venta: " Sin Saltar
	Leer v3
	
	comisionTotal = (v1 + v2 + v3) * 0.10
	
	sueldoTotal = sueldoBase + comisionTotal
	
	Escribir "Comision total de las ventas: $", comisionTotal
	Escribir "Total de ingresos: $", sueldoTotal
	
FinAlgoritmo
```
---
### Ejercicio 9

Una tienda ofrece un descuento del 15% sobre el total de la compra y un cliente desea saber cuanto deberá pagar finalmente por su compra.
```
Algoritmo ejercicio_9
	Definir totalCompra, descuento, total Como Real
	
	Escribir "Ingrese total de la compra: " Sin Saltar
	Leer totalCompra
	
	descuento = totalCompra * 0.15
	total = totalCompra - descuento
	
	Escribir "El total de la compra con descuento de 15% aplicado es ", total
FinAlgoritmo
```
---
### Ejercicio 10

Un alumno desea saber cual será su calificación final en la materia de Algoritmos. Dicha calificación se compone de los siguientes porcentajes:

- 55% del promedio de sus tres calificaciones parciales.
- 30% de la calificación del examen final.
- 15% de la calificación de un trabajo final.
```
Algoritmo ejercicio_10
	Definir notaParcial_1, notaParcial_2, notaParcial_3, promedioParcial Como Real 
	Definir notaExamen, notaTrabajo, notaFinal Como Real
	
	Escribir "Ingrese la primera nota parcial: " Sin Saltar
	Leer notaParcial_1
	Escribir "Ingrese la segunda nota parcial: " Sin Saltar
	Leer notaParcial_2
	Escribir "Ingrese la tercer nota parcial: " Sin Saltar
	Leer notaParcial_3
	Escribir "Ingrese nota del examen final: " Sin Saltar
	Leer notaExamen
	Escribir "Ingrese nota del trabajo final: " Sin Saltar
	Leer notaTrabajo
	
	promedioParcial = (notaParcial_1 + notaParcial_2 + notaParcial_3) / 3
	
	notaFinal = (promedioParcial * 0.55) + (notaExamen * 0.30) + (notaTrabajo * 0.15)
	
	Escribir "Tu calificación final es: ", notaFinal
	
	
FinAlgoritmo
```
---
### Ejercicio 11

Pide al usuario dos números y muestra la “distancia” entre ellos (el valor absoluto de su diferencia, de modo que el resultado sea siempre positivo).
```
Algoritmo ejercicio_11
	Definir x1, x2, distancia Como Real
	
	Escribir "Ingrese el primer numero: " Sin Saltar
	Leer x1
	Escribir "Ingrese el segundo numero: " Sin Saltar
	Leer x2
	
	distancia = abs(x1 - x2)
	
	Escribir "La distancia entre el primer y el segundo numero es ", distancia
FinAlgoritmo
```
---
### Ejercicio 12

Pide al usuario dos pares de números x1,y2 y x2,y2, que representen dos puntos en el plano. Calcula y muestra la distancia entre ellos.
```
Algoritmo ejercicio_12
	Definir x1, y1, x2, y2, distancia Como Real
	
	Escribir "Ingrese el valor del punto (x1): " Sin Saltar
	Leer x1
	Escribir "Ingrese el valor del punto (y1): " Sin Saltar
	Leer y1
	Escribir "Ingrese el valor del punto (x1): " Sin Saltar
	Leer x2
	Escribir "Ingrese el valor del punto (y2): " Sin Saltar
	Leer y2
	
	distancia = rc((x2 - x1)^2 + (y2 - y1)^2)
	
	Escribir "La distancia entre los dos puntos es ", distancia
	
FinAlgoritmo
```
---
### Ejercicio 13

Realizar un algoritmos que lea un número y que muestre su raíz cuadrada y su raíz cúbica. PSeInt no tiene ninguna función predefinida que permita calcular la raíz cúbica, ¿Cómo se puede calcular?
```
Algoritmo ejercicio_13
	Definir n, raizCuadrada, raizCubica Como Real
	Definir i Como Real
	
	Escribir "Ingrese un numero: " Sin Saltar
	Leer n
	
	raizCuadrada = rc(n)
	
	raizCubica = n^(1/3)
	
	Escribir "La raiz cuadrada de ", n, " es ", raizCuadrada
	Escribir "La raiz cubica de ", n, " es ", raizCubica
	
FinAlgoritmo
```
---
### Ejercicio 14

Dado un número de dos cifras, diseñe un algoritmo que permita obtener el número invertido. Ejemplo, si se introduce 23 que muestre 32.
```
Algoritmo ejercicio_14
	Definir n, x, z Como Entero
	
	Escribir "Ingrese un numero de dos cifras: " Sin Saltar
	Leer n
	
	x = trunc(n/10)
	z = n % 10
	
	Escribir z, x
	
FinAlgoritmo
```
---
### Ejercicio 15

Dadas dos variables numéricas A y B, que el usuario debe teclear, se pide realizar un algoritmo que intercambie los valores de ambas variables y muestre cuanto valen al final las dos variables.
```
Algoritmo ejercicio_15
	Definir A, B, C Como Entero
	
	Escribir "Ingrese el valor de A: " Sin Saltar
	Leer A
	Escribir "Ingrese el valor de B: " Sin Saltar
	Leer B
	
	C = A
	A = B
	B = C
	
	Escribir "Se han intercambiado las variables"
	Escribir "Valor de la variable A: ", A, ". Valor de la variable B: ", B, "."
FinAlgoritmo
```
---
### Ejercicio 16

Dos vehículos viajan a diferentes velocidades (v1 y v2) y están distanciados por una distancia d. El que está detrás viaja a una velocidad mayor. Se pide hacer un algoritmo para ingresar la distancia entre los dos vehículos (km) y sus respectivas velocidades (km/h) y con esto determinar y mostrar en que tiempo (minutos) alcanzará el vehículo más rápido al otro.
```
Algoritmo ejercicio_16
	Definir v1, v2, distancia, tiempo Como Real
	
	Escribir "Ingrese la velocidad, en km/h, del vehiculo 1: " Sin Saltar
	Leer v1
	Escribir "Ingrese la velocidad, en km/h, del vehiculo 2: " Sin Saltar
	Leer v2
	Escribir "Ingrese la distancia, en km, que hay entre los dos vehiculos" Sin Saltar
	Leer distancia
	
	tiempo = distancia / (v1 - v2)
	
	tiempo = tiempo * 60
	
	Escribir "El vehiculo alcanzara al otro en ", tiempo, " minutos."
FinAlgoritmo
```
---
### Ejercicio 17

Un ciclista parte de una ciudad A a las HH horas, MM minutos y SS segundos. El tiempo de viaje hasta llegar a otra ciudad B es de T segundos. Escribir un algoritmo que determine la hora de llegada a la ciudad B.
```
Algoritmo ejercicio_17
	Definir horaA, minA, segA, puntoA Como Entero
	Definir horaB, minB, segB, puntoB Como Entero
	Definir tiempoViaje Como Entero
	
	Escribir "Hora de salida:" Sin Saltar
	leer horaA
	Escribir "Minutos de salida: " Sin Saltar
	leer minA
	Escribir "Segundos de salida: " Sin Saltar
	Leer segA
	Escribir "Duracion del viaje (s): " Sin Saltar
	Leer tiempoViaje
	
	puntoA = (horaA * 3600) + (minA * 60) + segA
	
	puntoB = puntoA + tiempoViaje
	
	horaB = trunc(puntoB / 3600)
	minB = trunc(puntoB % 3600) / 60
	segB = (puntoB % 3600) % 60
	
	Escribir "Hora de llegada al punto B: ", horaB, " horas, ", minB, " minutos y ", segB, " segundos."
	
FinAlgoritmo
```
---
### Ejercicio 18

Pedir el nombre y los dos apellidos de una persona y mostrar las iniciales.
```
Algoritmo ejercicio_18
	Definir nombre, apellido, inicialN, incialA Como Caracter
	
	Escribir "Escribe tu nombre: " Sin Saltar
	Leer nombre
	Escribir "Escribe tu apellido: " Sin Saltar
	Leer apellido
	
	inicialN = Subcadena(nombre, 0, 1)
	inicialA = Subcadena(apellido, 0, 1)
	
	Escribir "Iniciales: ", inicialN, ", ", inicialA
FinAlgoritmo
```
---
### Ejercicio 19

Escribir un algoritmo para calcular la nota final de un estudiante, considerando que: por cada respuesta correcta 5 puntos, por una incorrecta -1 y por respuestas en blanco 0. Imprime el resultado obtenido por el estudiante.
```
Algoritmo ejercicio_19
	Definir totalPuntos, respuestaCorrecta, respuestaIncorrecta Como Real
	
	Escribir "Cantidad de respuestas correctas: " Sin Saltar
	Leer respuestaCorrecta
	Escribir "Cantidad de respuestas incorrectas. " Sin Saltar
	Leer respuestaIncorrecta
	
	totalPuntos = (respuestaCorrecta * 5) + (respuestaIncorrecta * (-1))
	
	Escribir "Total de puntos: ", totalPuntos
	
FinAlgoritmo
```
---
### Ejercicio 20

Diseñar un algoritmo que nos diga el dinero que tenemos (en euros y céntimos) después de pedirnos cuantas monedas tenemos (de 2€, 1€, 50 céntimos, 20 céntimos o 10 céntimos).
```
Algoritmo ejercicio_20
	Definir dosEuro, unEuro, centimos50, centimos20, centimos10, centimos, dineroTotal Como Entero
	Escribir "Cuantos monedas de $2 tienes: " Sin Saltar
	Leer dosEuro
	Escribir "Cuantas monedas de $1 tienes: " Sin Saltar
	Leer unEuro
	
	Escribir "Cuantas monedas de 50 centimos tienes: " Sin Saltar
	Leer centimos50
	Escribir "Cuantas monedas de 20 centimos tienes: " Sin Saltar
	Leer centimos20
	Escribir "Cuantas monedas de 10 centimos tienes: " Sin Saltar
	Leer centimos10
	
	euros = (dosEuro * 2) + unEuro
	centimos = (centimos50 * 50) + (centimos20 * 20) + (centimos10 * 10)
	
	euros = euros + trunc(centimos / 100)
	centimos = centimos % 100
	
	
	Escribir "Tienes ", euros, " euros y ", centimos, " centimos."
FinAlgoritmo
```
---
