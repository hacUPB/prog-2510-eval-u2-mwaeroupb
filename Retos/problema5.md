# Problema 5
![problema1](../Imagenes/sueldo.png)
Imagen [Sueldo](https://th.bing.com/th/id/R.dbb383279d5aa8a4a43a695cb6ea8f0d?rik=%2bgZGY8QNC2CAKA&riu=http%3a%2f%2fwww.on-school.com%2fblog%2fwp-content%2fuploads%2f2019%2f11%2f75154480-675-5000-ilustraci%c3%b3n-que-representa-el-mont%c3%b3n-de-dinero-billetes-y-monedas-ideal-para-materiales-instituci1.jpg&ehk=4V1YTPYuKCvJxXT%2bajTkInP1JgK0fk4NDRXnlmmHEaY%3d&risl=&pid=ImgRaw&r=0)

Realice un algoritmo que permita determinar el sueldo semanal de un trabajador con base en las horas trabajadas y el pago por hora, considerando que a partir de la hora número 41 y hasta la 45, cada hora se le paga el doble, de la hora 46 a la 50, el triple, y que trabajar
más de 50 horas no está permitido. Represente el algoritmo mediante pseudocódigo.

## 📝 Pseudocódigo
```
Inicio
    // Entrada: horas trabajadas y pago por hora
    Escribir "número de horas trabajadas en la semana:"
    Leer horas_trabajadas
    Escribir "pago por hora:"
    Leer pago_hora

    // Validar que las horas trabajadas no sean mayores a 50
    Si horas_trabajadas > 50 Entonces
        Escribir "Error: No se permite trabajar más de 50 horas."
    Sino
        // Caso 1: Hasta 40 horas, pago normal
        Si horas_trabajadas ≤ 40 Entonces
            sueldo ← horas_trabajadas * pago_hora
        // Caso 2: Entre 41 y 45 horas, las extras se pagan al doble
        Sino Si horas_trabajadas ≤ 45 Entonces
            sueldo ← (40 * pago_hora) + ((horas_trabajadas - 40) * (2 * pago_hora))
        // Caso 3: Entre 46 y 50 horas, las extras entre 41 y 45 se pagan al doble y las de 46 a 50 al triple
        Sino
            sueldo ← (40 * pago_hora) + (5 * (2 * pago_hora)) + ((horas_trabajadas - 45) * (3 * pago_hora))
        FinSi

        // Mostrar el sueldo calculado
        Escribir "El sueldo semanal es: ", sueldo
    FinSi
Fin
