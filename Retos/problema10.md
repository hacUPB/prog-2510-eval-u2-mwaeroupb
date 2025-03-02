# Problema 10
Realice un algoritmo para obtener el seno de un ángulo y represéntelo mediante pseudocódigo. Utilice la siguiente ecuación:
$Sen x = x - \frac{x^3}{3!} + \frac{x^5}{5!} - \frac{x^7}{7!} + ...$

## 📝 Pseudocódigo
```
Inicio
    Leer x  // Ángulo en radianes
    Leer n  // Número de términos de la serie
    seno_x ← x  // Primer término de la serie
    termino ← x  // Variable para calcular cada término
    signo ← -1   // Alterna los signos de la serie

    Desde i = 1 hasta n Hacer
        termino ← termino * (x * x) / ((2 * i) * (2 * i + 1))  // Se multiplica por x^2 y se divide por (2i)(2i+1)
        seno_x ← seno_x + (signo * termino)  // Se suma o resta el término a la aproximación
        signo ← signo * -1  // Alterna el signo
    Fin Desde

    Imprimir "Sen(", x, ") ≈ ", seno_x
Fin

