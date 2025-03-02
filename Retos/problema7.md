# Problema 7
![problema1](../Imagenes/sueldo.png)

Imagen [Sueldo](https://th.bing.com/th/id/R.dbb383279d5aa8a4a43a695cb6ea8f0d?rik=%2bgZGY8QNC2CAKA&riu=http%3a%2f%2fwww.on-school.com%2fblog%2fwp-content%2fuploads%2f2019%2f11%2f75154480-675-5000-ilustraci%c3%b3n-que-representa-el-mont%c3%b3n-de-dinero-billetes-y-monedas-ideal-para-materiales-instituci1.jpg&ehk=4V1YTPYuKCvJxXT%2bajTkInP1JgK0fk4NDRXnlmmHEaY%3d&risl=&pid=ImgRaw&r=0)

Se requiere un algoritmo para determinar cuánto ahorrará en pesos una persona diariamente, y en un año, si ahorra 3¢ el primero de enero, 9¢ el dos de enero, 27¢ el 3 de enero y así sucesivamente todo el año. Represente la solución mediante pseudocódigo.

## 📝 Pseudocódigo
```
Inicio
    // Inicializar variables
    ahorro_dia ← 3   // Comienza ahorrando 3 centavos
    ahorro_total ← 0 // Acumulador del ahorro anual

    // Recorrer los 365 días del año
    Desde dia ← 1 hasta 365 Hacer
        Imprimir "Día ", dia, ": ahorró ", ahorro_dia, " centavos"
        ahorro_total ← ahorro_total + ahorro_dia
        ahorro_dia ← ahorro_dia * 3 // Multiplica por 3 cada día
    Fin Desde

    // Convertir a pesos (1 peso = 100 centavos)
    ahorro_pesos ← ahorro_total / 100

    // Mostrar el ahorro total en pesos
    Imprimir "El ahorro total en el año es: ", ahorro_pesos, " pesos"
Fin
