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


- **Tamaño por registro:** `19 bytes`  

- **Registros en 24 horas:** `8640 registros`

- **Espacio total en bytes:** `164,160 bytes`

- **Espacio total en KB:** `160.31 KB`  

- **Espacio total en MB:** `0.16 MB`  

### Resultado Final  

Para almacenar estos datos durante 24 horas, se requieren aproximadamente **160.31 KB (≈0.16 MB) de memoria**. 
