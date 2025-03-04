# Problema 9 
![problema1](../Imagenes/e.png)
Imagen [E](https://media.istockphoto.com/id/649112040/es/foto/funci%C3%B3n-exponencial-natural-matem%C3%A1ticas-symbol-ilustraci%C3%B3n-de-render-3d.jpg?s=1024x1024&w=is&k=20&c=bZ56kbVL6_QybFCRfGIu2N2CDkSttAfTICBxv230k3k=)

8. Realice un algoritmo y represéntelo mediante pseudocódigo para obtener una función exponencial, la cual está dada por:
    
    $𝑒^𝑥 = 1+\frac x {1!} + \frac {x^2}{2!}+ \frac {x^3}{3!}+ …$
    
## 📝 Pseudocódigo
```
Inicio
    Leer x
    Leer n  // Número de términos de la serie
    e_x ← 1  // Primer término de la serie
    termino ← 1  // Variable para calcular cada término

    Desde i = 1 hasta n Hacer
        termino ← termino * (x / i)  // Se multiplica por x y se divide por i (equivale a x^i / i!)
        e_x ← e_x + termino  // Se suma el término a la aproximación
    Fin Desde

    Imprimir "e^", x, " ≈ ", e_x
Fin
