# Problema 8
![problema1](../Imagenes/hardware.gif)

Realice el algoritmo para determinar cuánto pagará una persona que adquiere N artículos, los cuales están de promoción. Considere que si su precio es mayor o igual a $200 se le aplica un descuento de 15%, y si su precio es mayor a $100, pero menor a $200, el descuento es de
12%; de lo contrario, solo se le aplica 10%. Se debe saber cuál es el costo y el descuento que tendrá cada uno de los artículos y finalmente cuánto se pagará por todos los artículos obtenidos. Represente la solución mediante pseudocódigo.

## 📝 Pseudocódigo
```

Inicio 
Escribir "Ingrese el nombre de los articulos que compro: "
Leer nombres 
Escribir "Ingresa del valor de cada uno de los articulos en el mismo orden que los nombres: "
Leer valor 
descuentos= []
precios = []                                                    precio como una lista vacia 
precio total = 0
Desde i=0 hasta  n                                              len(valor)  tamaño empieza el ciclo
    precio=0
    descuento=0                                                 cambia con cada iteracion
    Si valor[i] >= 200                                          valor en la posicion i
        precio= (valor[i]- valor[i]*0.15)
        descuento = "15%"
    Sino valor[i]<200 y valor [i]>100
        precio= (valor[i]- valor[i]*0.12)
        descuento= "12%"
    Else 
        precio= (valor[i]-valor[i]*0.10)
        descuento= "10%"
    Fin condicion 
    precio total = precio total + precio
    precio sin descuento = precio sin descuento + valor[i] 
    precios.append(precio)                                         precio se añade a precios 
    descuentos.append(descuento)                                   se añade descuento a la lista 
Fin desde
imprimir "El articulo: "nombre + "tiene un valor de: " valor + "con un descuento de: " descuento
imprimir "el precio total a pagar es: " precio total + "el precio total sin descuento de cada articulo es:  " precio sin descuento
                
no cambia el orden de las listas 




 
