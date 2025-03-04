# Actividad 4: De algoritmo a código fuente

## 1. Introducción
> ¿Por qué crees que el pseudocódigo es útil antes de escribir un programa en Python?

El pseudocódigo es útil antes de escribir un programa en Python porque permite estructurar y planificar la lógica del programa sin preocuparse por la sintaxis específica del lenguaje.


## 2. Estructura básica del pseudocódigo
> Actividad: 
- Toma un pseudocódigo de un ejercicio anterior o escribe tu propio pseudocódigo, similar al mostrado en el ejemplo de arriba 👆🏻.

```
INICIO
    Leer num1
    Leer num2
    suma = num1 + num2
    promedio = suma / 2
    Mostrar promedio
FIN
```

## 3. Traduciendo el pseudocódigo a Python
> Pregunta orientadora:
¿Cuál es la diferencia entre usar `int(input())` y `float(input())` en Python? Si no lo tienes claro, investiga y discute lo que encontraste con el profe.

| Función         | Tipo de Dato | Acepta Decimales | Ejemplo de Entrada Válida |
|---------------|-------------|----------------|-------------------|
| `int(input())` | Entero      | ❌ No         | `10`, `25`, `100` |
| `float(input())` | Decimal     | ✅ Sí        | `3.14`, `10.0`, `5` |


## 4. Ejemplos adicionales de pseudocódigo y su traducción
> Actividad:
- Escribe tu propio pseudocódigo para calcular el promedio de una lista de calificaciones y tradúcelo a Python.

Pseudocódigo:
```
INICIO
    Leer n  // Cantidad de calificaciones
    Definir lista_notas como una lista vacía
    Para i desde 1 hasta n hacer
        Leer nota
        Agregar nota a lista_notas
    Fin Para
    suma = sumar todos los valores en lista_notas
    promedio = suma / n
    Mostrar promedio
FIN

```
Código en Python:
```
# Solicitar la cantidad de calificaciones
n = int(input("Ingresa la cantidad de calificaciones: "))

# Lista para almacenar las calificaciones
lista_notas = []

# Leer las calificaciones y agregarlas a la lista
for i in range(n):
    nota = float(input(f"Ingrese la calificación {i+1}: "))
    lista_notas.append(nota)

# Calcular el promedio
suma = sum(lista_notas)
promedio = suma / n

# Mostrar el resultado
print("El promedio de las calificaciones es:", promedio)
```

## 5. Buenas prácticas
> Pregunta orientadora:
- ¿Por qué es importante comentar el código, aunque sea breve y conciso?

Aunque sean breves y concisos, los comentarios hacen que el código sea más legible y útil a largo plazo. 


## 6. Reto final
Reto: toma el pseudocódigo de los 5 primeros ejercicios del reto y realiza la traducción a Python:

### Eercicio 1 Distancia entre dos puntos en el plano cartesiano
```
import math  # Importamos la librería para usar la raíz cuadrada

# Pedir las coordenadas del primer punto
x1, y1 = map(float, input("Ingrese (x1, y1) separados por espacio: ").split())

# Pedir las coordenadas del segundo punto
x2, y2 = map(float, input("Ingrese (x2, y2) separados por espacio: ").split())

# Calcular la distancia euclidiana
d = math.sqrt((x2 - x1)**2 + (y2 - y1)**2)

# Mostrar el resultado
print("La distancia entre los puntos es:", d)
```
### Ejercicio 2 Pulgadas a Metros

```
# Pedir la medida en metros
T = float(input("Ingrese la medida en metros (T): "))

# Convertir a pulgadas (1 pulgada = 0.0254 metros)
pulgadas = T / 0.0254

# Mostrar el resultado
print("La medida en pulgadas es:", pulgadas)
```
### Ejercicio 3 Hipotenusa de un triángulo
```
import math  # Importamos la librería para usar la raíz cuadrada

# Pedir los valores de A y B
A, B = map(float, input("Ingrese A y B separados por espacio: ").split())

# Calcular C usando el teorema de Pitágoras
C = math.sqrt(A**2 + B**2)

# Mostrar el resultado
print("El valor de C es:", C)

```
### Ejercicio 4 Edad actual de una persona
```
# Pedir la fecha de nacimiento
dia_nac = int(input("Ingrese el día de nacimiento: "))
mes_nac = int(input("Ingrese el mes de nacimiento: "))
año_nac = int(input("Ingrese el año de nacimiento: "))

# Pedir la fecha actual
dia_actual = int(input("Ingrese el día actual: "))
mes_actual = int(input("Ingrese el mes actual: "))
año_actual = int(input("Ingrese el año actual: "))

# Calcular la edad inicial
edad = año_actual - año_nac

# Verificar si ya cumplió años este año
if mes_actual < mes_nac or (mes_actual == mes_nac and dia_actual < dia_nac):
    edad -= 1
    print("Aún no ha cumplido años este año.")
elif mes_actual == mes_nac and dia_actual == dia_nac:
    print("¡Feliz Cumpleaños! 🎉")
else:
    print("Ya cumplió años este año.")

# Mostrar la edad calculada
print("La edad de la persona es:", edad)

```
### Ejercicio 5 Sueldo semanal de un trabajador
```
# Entrada: horas trabajadas y pago por hora
horas_trabajadas = int(input("Ingrese el número de horas trabajadas en la semana: "))
pago_hora = float(input("Ingrese el pago por hora: "))

# Validar que las horas trabajadas no sean mayores a 50
if horas_trabajadas > 50:
    print("Error: No se permite trabajar más de 50 horas.")
else:
    # Caso 1: Hasta 40 horas, pago normal
    if horas_trabajadas <= 40:
        sueldo = horas_trabajadas * pago_hora
    # Caso 2: Entre 41 y 45 horas, las extras se pagan al doble
    elif horas_trabajadas <= 45:
        sueldo = (40 * pago_hora) + ((horas_trabajadas - 40) * (2 * pago_hora))
    # Caso 3: Entre 46 y 50 horas, las extras entre 41 y 45 se pagan al doble y las de 46 a 50 al triple
    else:
        sueldo = (40 * pago_hora) + (5 * (2 * pago_hora)) + ((horas_trabajadas - 45) * (3 * pago_hora))

    # Mostrar el sueldo calculado
    print("El sueldo semanal es:", sueldo)

```
> Pregunta final:
- Después de este tutorial, ¿qué puntos crees que deberías reforzar para sentirte más seguro al traducir pseudocódigo a Python?
Creo que para mejorar en la traduccion de pseudocodigo a Python me hace falta practica y un mejor dominio del ingles para no hacer la memorizacion tan mecanica.