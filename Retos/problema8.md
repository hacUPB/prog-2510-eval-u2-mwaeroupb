# Problema 8
![problema1](../Imagenes/hardware.gif)

Realice el algoritmo para determinar cuánto pagará una persona que adquiere N artículos, los cuales están de promoción. Considere que si su precio es mayor o igual a $200 se le aplica un descuento de 15%, y si su precio es mayor a $100, pero menor a $200, el descuento es de
12%; de lo contrario, solo se le aplica 10%. Se debe saber cuál es el costo y el descuento que tendrá cada uno de los artículos y finalmente cuánto se pagará por todos los artículos obtenidos. Represente la solución mediante pseudocódigo.

## 📝 Pseudocódigo
```
Inicio
    Leer N
    Total ← 0

    Desde i = 1 hasta N Hacer
        Leer Precio
        Si Precio ≥ 200 Entonces
            Descuento ← Precio * 0.15
        Si no Si Precio > 100 Entonces
            Descuento ← Precio * 0.12
        Si no
            Descuento ← Precio * 0.10
        Fin Si
        PrecioFinal ← Precio - Descuento
        Total ← Total + PrecioFinal
        Imprimir "Artículo ", i, ": Precio =", Precio, ", Descuento =", Descuento, ", Precio final =", PrecioFinal
    Fin Desde

    Imprimir "Total a pagar:", Total
Fin
