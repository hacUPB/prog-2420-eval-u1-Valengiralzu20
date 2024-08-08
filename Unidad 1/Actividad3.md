# Algoritmos 

## Problema 1: Determinar el promedio de calificaciones de un estudiante y si ha aprobado o no Ana quiere saber si ha aprobado sus exámenes finales. Tiene una lista de sus calificaciones y necesita calcular el promedio. Para aprobar, debe tener un promedio de al menos 3.0.

### Análisis del problema: 
1.	#### Inicialización de variables: 
Cantidad_notas: esta variable se usa para determinar la cantidad de notas de Ana 
Calificaciones_Ana: esta variable se usará para definir las notas de Ana 
Promedio_notas: sumar las variables y dividir por el numero de notas 
Notamin_aprobacion: se debe determinar cual es la nota mínima para aprobar el curso

2.	#### Entrada de Datos: 
o	El usuario debe ingresar sus notas separada por comas (5.0, 4.5, 3.5, 2.0...)
o	Decir la cantidad de notas ingresadas cantidad_notas
o	Decir la notamin_aprobacion 

3.	#### Proceso: 
o	Se debe calcular el promedio, para esto sumar Calificaciones_Ana y luego dividirlas entre Cantidad_notas y se obtiene el promedio_notas  

4.	#### Salida: 
o	Imprimir el promedio de notas de Ana. 
o	Poner condicional: Si el promedio es igual o mayor a 3.0 mostrar mensaje de texto que diga “aprobó con un promedio de:”
o	Si el promedio es <3.0 mostrar mensaje de texto “no aprobó, su promedio es:”

### Pseudocódigo 
#### Inicio 
Declaración de variables
Definir Calificaciones_Ana como list
Definir cantidad_notas como numero
Definir Promedio_notas como numero
Definir notamin_aprobacion como numero >3.0

#### Ingreso de datos
Escribir Calificaciones_Ana separadas por comas 
Leer Lista_calificaciones_Ana

#### Procesamiento 
Para cada calificación en Lista_calificaciones_Ana hacer Suma_calificaciones= Suma_calificaciones+ calificación  cantidad_calificaciones
 Fin para  Promedio_notas= suma_calificaciones / cantidad_calificaciones 

#### Salida
Si promedio_notas >= 3.0 
      Escribir “aprobó con un promedio de:” 
Sino 
      Escribir “no aprobó, su promedio es:”
#### FIN 
