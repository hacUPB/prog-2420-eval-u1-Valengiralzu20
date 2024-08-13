# Algoritmos 

### Problema 1: Determinar el promedio de calificaciones de un estudiante y si ha aprobado o no
 #### Ana quiere saber si ha aprobado sus exámenes finales. Tiene una lista de sus calificaciones y necesita calcular el promedio. Para aprobar, debe tener un promedio de al menos 3.0.

### Análisis del problema: 
1.	#### Inicialización de variables: 
-Cantidad_notas: esta variable se usa para determinar la cantidad de notas de Ana 
-Calificaciones_Ana: esta variable se usará para definir las notas de Ana 
-Promedio_notas: sumar las variables y dividir por el numero de notas 
-Notamin_aprobacion: se debe determinar cual es la nota mínima para aprobar el curso

2.	#### Entrada de Datos: 
-El usuario debe ingresar sus notas separada por comas (5.0, 4.5, 3.5, 2.0...)
-Decir la cantidad de notas ingresadas cantidad_notas
-Decir la notamin_aprobacion 

3.	#### Proceso: 
-Se debe calcular el promedio, para esto sumar Calificaciones_Ana y luego dividirlas entre Cantidad_notas y se obtiene el promedio_notas  

4.	#### Salida: 
-Imprimir el promedio de notas de Ana. 
-Poner condicional: Si el promedio es igual o mayor a 3.0 mostrar mensaje de texto que diga “aprobó con un promedio de:”
-Si el promedio es <3.0 mostrar mensaje de texto “no aprobó, su promedio es:”

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


### Problema 4: Determinar la distancia total recorrida por un vehículo con registros de velocidad y tiempo
#### María tiene un registro de las velocidades a las que ha conducido su vehículo y el tiempo que ha mantenido cada velocidad. Quiere calcular la distancia total recorrida.

### Análisis del problema: 
1.	#### Inicialización de variables: 
-Velocidad: esta variable se usa para determinar la velocidad a las que ha conducido su vehículo  
-Tiempo: esta variable se usará para definir el tiempo que ha mantenido cada velocidad  
-Distancia_total: velocidad * tiempo = distancia_total

2.	#### Entrada de Datos: 
-El usuario debe ingresar velocidad separadas por comas notas separadas por comas
-Debe ingresar tiempo separado por comas 

3.	#### Proceso: 
-Se debe calcular la distancia total, para esto multiplicar la velocidad por el tiempo 

4.	#### Salida: 
-Imprimir distancia_total y escribir “La distancia total recorrida es de:”

### Pseudocódigo 

#### Inicio 
Declaración de variables 
Definir velocidad 
Definir tiempo 
Definir distancia_total >0

#### Ingreso de datos 
Escribir “ingrese velocidad en (m/s) separadas por comas”
Leer velocidad
Escribir  “ingrese tiempo en segundos separados por coma”
Leer tiempo 

#### Cálculo de la distancia total
Para i desde [1] hasta tamaño (velocidad) hacer:
Distancia_tramo= velocidad [i]* tiempo[i]
Distancia_total = distancia_total + distancia_tramo 

#### Salida 
Escribir “la distancia total recorrida es:   distancia_total “metros””

FIN

### Problema 6: Calcular la edad de una persona a partir de su fecha de nacimiento y la fecha actual
#### Descripción del Problema: Se desea saber cuántos años, meses y días tiene actualmente una persona, basándose en su fecha de nacimiento. Además, le gustaría saber si ya ha cumplido años este año o aún no, y si hoy es su cumpleaños para celebrarlo. Cada una de las fechas está conformada por 3 variables: día, mes y año

### Análisis del problema: 
1.	#### Inicialización de variables: 
-Fecha_nacimiento: esta variable se usa para determinar fecha de nacimiento de la persona, se debe decir día, mes y año 
-Fecha_actual: esta variable se usará para determinar la fecha actual, se debe decir día, mes y año 

2. #### Entrada de Datos: 
-El usuario debe ingresar su fecha de nacimiento (día, mes, año)
-Debe ingresar la fecha actual (día, mes, año)

3.	#### Proceso: 
-Se debe obtener día_actual, mes_actual, año_actual 
-Calculo de años: año_actual-año_nacimiento
-Hacer ajuste de años: si no ha cumplido año_actual-1=ajuste_años
-Calculo de meses: meses= mes_actual-mes_nacimiento, si mes_actual>mes_nacimiento se debe hacer un ajuste 
-Calculo de días: diferencia de días, se asume 30 días del mes y se calcula días=30-día_nacimiento

4.	#### Salida: 
-Imprimir la edad calculada, en años, meses y días “Tienes  ” años , “” meses, “” días. 

5.	#### Verificación cumpleaños 
-Se verifica si la fecha actual coincide con la fecha de nacimiento, si coinciden, escribir mensaje “Feliz cumpleaños”

#### Pseudocódigo
Inicio 
Definir fecha_nacimiento
Definir fecha_actual

Ingreso de datos 
Escribir “ingrese fecha de nacimiento (día, mes, año) separadas por comas”
Leer fecha de nacimiento
Escribir “ingrese fecha actual en (día, mes, año), separadas por comas”
Leer fecha actual

Cálculo de la edad 
Si fecha_actual <fecha_nacimiento
     Entonces fecha_actua-fecha_nacimiento=edad
    Fin si 
Si fecha_actual > fecha_nacimiento
     Entonces fecha_actual -1 = edad 
     Fin si 
Si mes_actual<mes_nacimiento
     Entonces mes actual-mes nacimiento= mes edad

Salida 
Su edad es:   “años, meses, días””
