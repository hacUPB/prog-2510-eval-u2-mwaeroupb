# Problema 5
![problema1](../Imagenes/sueldo.png)
Imagen [Sueldo](https://th.bing.com/th/id/R.dbb383279d5aa8a4a43a695cb6ea8f0d?rik=%2bgZGY8QNC2CAKA&riu=http%3a%2f%2fwww.on-school.com%2fblog%2fwp-content%2fuploads%2f2019%2f11%2f75154480-675-5000-ilustraci%c3%b3n-que-representa-el-mont%c3%b3n-de-dinero-billetes-y-monedas-ideal-para-materiales-instituci1.jpg&ehk=4V1YTPYuKCvJxXT%2bajTkInP1JgK0fk4NDRXnlmmHEaY%3d&risl=&pid=ImgRaw&r=0)

Realice un algoritmo que permita determinar el sueldo semanal de un trabajador con base en las horas trabajadas y el pago por hora, considerando que a partir de la hora número 41 y hasta la 45, cada hora se le paga el doble, de la hora 46 a la 50, el triple, y que trabajar
más de 50 horas no está permitido. Represente el algoritmo mediante pseudocódigo.

## 📝 Pseudocódigo
```
Inicio
    Escribir "Ingresa el número de horas que trabajaste esta semana: "
    Leer h
    Escribir "Ingresa el pago por hora: "
    Leer ph

    Si h > 50 Entonces
        Escribir "Número de horas no permitido en la empresa"
    Sino
        Si h <= 40 Entonces
            sueldo <- h * ph
        Sino Si h >= 41 Y h <= 45 Entonces
            sueldo <- (40 * ph) + ((h - 40) * 2 * ph)
        Sino Si h >= 46 Y h <= 50 Entonces
            sueldo <- (40 * ph) + (5 * 2 * ph) + ((h - 45) * 3 * ph)
        FinSi

        Escribir "Su sueldo es: ", sueldo
    FinSi
Fin

```






