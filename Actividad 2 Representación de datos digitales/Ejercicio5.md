# Actividad 5 
## Cálculo del Espacio en Memoria para Almacenar Datos  

Para almacenar la información cada 10 segundos durante 24 horas, primero analizamos los tamaños de los tipos de datos en un lenguaje como **C o Java** 

### Tamaño de los Datos  

| Dato | Tipo de Dato | Tamaño Aproximado |
|------|------------|------------------|
| Identificador numérico | `int` | 4 bytes |
| Temperatura | `float` | 4 bytes |
| Valor lógico | `bool` (`boolean`) | 1 byte |
| Texto (10 caracteres) | `char[10]` o `String` | 10 bytes |

### Cálculo por Registro  
Cada conjunto de datos ocupa:  

\[4 + 4 + 1 + 10 = 19 \text{ bytes}\]

### Registros por Día  
Los datos se almacenan **cada 10 segundos durante 24 horas**.  

\[\frac{60 \text{ seg} \times 60 \text{ min} \times 24 \text{ h}}{10 \text{ seg}} = 8640 \text{ registros}\]

### Espacio Total Requerido  

\[8640 \text{ registros} \times 19 \text{ bytes/reg} = 164,160 \text{ bytes}\]

Convertimos a **Kilobytes (KB)** y **Megabytes (MB)**:  

\[\frac{164,160}{1024} \approx 160.31 \text{ KB}\]

\[\frac{160.31}{1024} \approx 0.16 \text{ MB}\]

### Resultado Final  

Para almacenar estos datos durante 24 horas, se requieren aproximadamente **160.31 KB (≈0.16 MB) de memoria**. 
