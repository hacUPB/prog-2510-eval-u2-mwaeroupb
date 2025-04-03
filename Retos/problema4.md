# Problema 4
 ![problema1](../Imagenes/feliz-cumpleanos.png)
 Imagen [Feliz cumpleaños](https://th.bing.com/th/id/OIP.0rXf0NpMcJeG8X5NRuimWgHaFz?rs=1&pid=ImgDetMain)

3. Se requiere determinar la edad actual de una persona basándose en su fecha de nacimiento. Además, es necesario establecer si la persona ya ha cumplido años en el año en curso, si aún no lo ha hecho, o si hoy es su cumpleaños, para celebrarlo. La fecha de nacimiento y la fecha actual estarán representadas mediante tres variables: día, mes y año.
    
## 📝 Pseudocódigo
```
 Inicio
    // Entrada: fecha de nacimiento
    Escribir "Ingrese el día de nacimiento:"
    Leer dia_nac
    Escribir "Ingrese el mes de nacimiento:"
    Leer mes_nac
    Escribir "Ingrese el año de nacimiento:"
    Leer año_nac

    // Entrada: fecha actual
    Escribir "Ingrese el día actual:"
    Leer dia_actual
    Escribir "Ingrese el mes actual:"
    Leer mes_actual
    Escribir "Ingrese el año actual:"
    Leer año_actual

    // Calcular la edad inicial
    edad= año_actual - año_nac

    // Verificar si ya cumplió años este año
    Si (mes_actual < mes_nac) o (mes_actual = mes_nac y dia_actual < dia_nac) Entonces
        edad = edad - 1
        Escribir "Aún no ha cumplido años este año."
    Sino Si (mes_actual = mes_nac y dia_actual = dia_nac) Entonces
        Escribir "Feliz Cumpleaños"
    Sino
        Escribir "Ya cumplió años este año."
    FinSi

    // Mostrar la edad calculada
    Escribir "La edad de la persona es: ", edad
Fin


