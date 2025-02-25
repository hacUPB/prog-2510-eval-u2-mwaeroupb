# Actividad 2

## Algoritmo para calcular el ingreso semestral y promedio mensual de un empleado  

### Descripción  
Este algoritmo recibe como datos el **ID del empleado** y los **seis primeros sueldos del año**, calcula el **ingreso total semestral** y el **promedio mensual**, y muestra los resultados.  

## Diagrama de flujo

 <p align="center">
  <img src="../Imagenes/mapa.jpeg" alt="Diagrama de flujo" width="300">
</p>

## Pseudocódigo 
```plaintext
Inicio
  1. Leer ID_Empleado
  2. Leer Sueldo1, Sueldo2, Sueldo3, Sueldo4, Sueldo5, Sueldo6
  3. Calcular Ingreso_Total = Sueldo1 + Sueldo2 + Sueldo3 + Sueldo4 + Sueldo5 + Sueldo6
  4. Calcular Promedio_Mensual = Ingreso_Total / 6
  5. Imprimir "ID del Empleado: ", ID_Empleado
  6. Imprimir "Ingreso Total Semestral: ", Ingreso_Total
  7. Imprimir "Promedio Mensual: ", Promedio_Mensual
Fin


