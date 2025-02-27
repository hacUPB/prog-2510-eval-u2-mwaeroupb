# Problema 4
 ![problema1](../Imagenes/feliz-cumpleanos.png)
 Imagen [Feliz cumpleaños](https://th.bing.com/th/id/OIP.0rXf0NpMcJeG8X5NRuimWgHaFz?rs=1&pid=ImgDetMain)

3. Se requiere determinar la edad actual de una persona basándose en su fecha de nacimiento. Además, es necesario establecer si la persona ya ha cumplido años en el año en curso, si aún no lo ha hecho, o si hoy es su cumpleaños, para celebrarlo. La fecha de nacimiento y la fecha actual estarán representadas mediante tres variables: día, mes y año.
    
## 📝 Pseudocódigo
```
Inicio
    Escribir "DIA"
    Leer DIA
    Escribir "MES"
    Leer MES
    Escribir "AÑO"
    Leer AÑO

    Escribir "dia hoy"
    Leer dia hoy
    Escribir "mes actual"
    Leer mes actual
    Escribir "año actual"
    Leer año actual

    edad ← año_act - año_nac

    Si (mes_act < mes_nac) O (mes_act = mes_nac Y dia_act < dia_nac) Entonces
        edad ← edad - 1
        Escribir "Aún no has cumplido años este año."
    Sino Si (mes_act = mes_nac Y dia_act = dia_nac) Entonces
        Escribir "Feliz Cumpleaños!"
    Sino
        Escribir "Ya has cumplido años este año."
    FinSi

    Escribir "Tu edad actual es: ", edad
Fin

