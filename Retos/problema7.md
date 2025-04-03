# Problema 7
![problema1](../Imagenes/sueldo.png)

Imagen [Sueldo](https://th.bing.com/th/id/R.dbb383279d5aa8a4a43a695cb6ea8f0d?rik=%2bgZGY8QNC2CAKA&riu=http%3a%2f%2fwww.on-school.com%2fblog%2fwp-content%2fuploads%2f2019%2f11%2f75154480-675-5000-ilustraci%c3%b3n-que-representa-el-mont%c3%b3n-de-dinero-billetes-y-monedas-ideal-para-materiales-instituci1.jpg&ehk=4V1YTPYuKCvJxXT%2bajTkInP1JgK0fk4NDRXnlmmHEaY%3d&risl=&pid=ImgRaw&r=0)

Se requiere un algoritmo para determinar cuánto ahorrará en pesos una persona en un año, si ahorra 3¢ el primero de enero, 9¢ el dos de enero, 27¢ el 3 de enero y así sucesivamente todo el año. Represente la solución mediante pseudocódigo.

## 📝 Pseudocódigo
```
Inicio
ahorro = 0
Desde i=1 hasta 30                 (todos los meses tienen 30 dias)
    ahorro = ahorro + (3)**i
Fin Desde

ahorro = ahorro *12

imprimir "El ahorro de una persona en un año si tododos los meses tienen 30 dias es : " ahorro


