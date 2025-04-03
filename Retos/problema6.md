# Problema 6 
![problema1](../Imagenes/images.jpg)

Imagen [Sueldo](https://th.bing.com/th/id/R.dbb383279d5aa8a4a43a695cb6ea8f0d?rik=%2bgZGY8QNC2CAKA&riu=http%3a%2f%2fwww.on-school.com%2fblog%2fwp-content%2fuploads%2f2019%2f11%2f75154480-675-5000-ilustraci%c3%b3n-que-representa-el-mont%c3%b3n-de-dinero-billetes-y-monedas-ideal-para-materiales-instituci1.jpg&ehk=4V1YTPYuKCvJxXT%2bajTkInP1JgK0fk4NDRXnlmmHEaY%3d&risl=&pid=ImgRaw&r=0)

Se requiere un algoritmo para determinar, de N cantidades, cuántas son cero, cuántas son menores a cero, y cuántas son mayores a cero. Realice el pseudocódigo para representarlo, utilizando el ciclo apropiado.

## 📝 Pseudocódigo
```
Inicio 
Escribir "Ingrese las cantidades: "
Leer Cantidades
Saber tamaño de "Cantidades"            (len(Cantidades))
mayor = 0
menor = 0
igual = 0
Desde i=0 hasta tamaño de cantidades 
    Si Cantidad > 0                                             (cantidad = valor posicion i en cantidades)
        mayor = mayor + 1             La variable se vuelve a guardar con el valor de mayor + 1
    Sino Cantidad < 0 
        menor = menor +1
    Sino Cantidad == 0
        igual = igual + 1
    Finsi
Fin Desde
Imprimir "La cantidad de nuemeros mayores a 0 son:" mayor
Imprimir "La cantidad de nuemeros menores a 0 son:" menor
Imprimir "La cantidad de nuemeros iguales a 0 son:" igual

       