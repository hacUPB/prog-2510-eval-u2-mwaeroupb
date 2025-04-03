# Problema 9 
![problema1](../Imagenes/e.png)
Imagen [E](https://media.istockphoto.com/id/649112040/es/foto/funci%C3%B3n-exponencial-natural-matem%C3%A1ticas-symbol-ilustraci%C3%B3n-de-render-3d.jpg?s=1024x1024&w=is&k=20&c=bZ56kbVL6_QybFCRfGIu2N2CDkSttAfTICBxv230k3k=)

8. Realice un algoritmo y represéntelo mediante pseudocódigo para obtener una función exponencial, la cual está dada por:
    
    $𝑒^𝑥 = 1+\frac x {1!} + \frac {x^2}{2!}+ \frac {x^3}{3!}+ …$
    
## 📝 Pseudocódigo
```
Inicio
Escribir "que precicion quieres: "
Leer n
Escribir "A que numero quieres elevar e: "
Leer x
resultado = 0
Desde i=0 hasta n
    resultado = resultado + x**i / i!                 factorial en codigo es con otro ciclo
Fin desde 
imprimir "e^x segun los datos suministrados es : " resultado 

