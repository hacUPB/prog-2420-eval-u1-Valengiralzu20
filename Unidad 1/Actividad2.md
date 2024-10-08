# Sistemas númericos 
## [Diagrama de bloques](https://miro.com/welcomeonboard/bGhPSnlGVEFmV2VSMFFSS2lINWZRdHpTbHJ2aUNCZmFDTDZJTVhTYm94NkdUdUNxTlRodFhySmhJRWtyTnJCenwzMDc0NDU3MzYyMjYzMDQ3NTUyfDI=?share_link_id=369874603517URL)

### Aplicación 1: 
### Una aeronave se encuentra volando a una velocidad de 500 mph, se requiere saber el proceso de la computadora para interpretar los datos que llegan desde los sensores. 

### Procedimiento que se debe seguir:
1. Un sensor de velocidad ubicado en una aeronave detecta una velocidad crucero de 500 mph esto genera un dato binario de 10 bits. 
2. Luego, debe detectar de que sensor le está llegando la señal en 2 bits, en este caso la señal le esta llegando de 00 que es velocidad 
3. Ahora debe decodificar y verificar el bit de paridad para detectar errores y descartar datos si se detecta un error 
4. Enviar nuevamente el dato de velocidad con las decodificaciones 
5. Convertir los datos binarios a decimal para facilitar visualización 
6. Ahora con el dato velocidad calcular el error para esto usar error=valor medido-setpoint
7. El valor calculado del error convertirlo de decimal a binario 
8. El valor calculado de velocidad del error calculado en binario hacerlo control proporcional a los valores de error con control=error*kp 
9. Ese valor obtenido codificarlo en formato adecuado para ser enviada a la unidad de control de la aeronave

### Procedimiento numérico: 
1. Recibe el dato de velocidad de 500 mph y lo convierte a binario en 10 bits y se obtiene el siguiente valor: 111110100
2. En 2 bits, identificar que señal le esta llegando, en este caso 00-que hace referencia a la velocidad
3. Obtenemos este dato con la señal de que viene del sensor de velocidad y se agrega el bit de paridad 1. El valor obtenido es de: 00 0111110100 1
4. Se envía el dato de velocidad con las decodificaciones y se verifica que la paridad es correcta 
5. Se convierten los datos de binarios en decimal para facilitar la visualización y obtenemos nuevamente el valor 500 
6. Para calcular el error se utilizará un set point de 520, por lo tanto el calculo sería: 
                                          Error=500-520= -20
7.	El valor calculado se convierte de decimal a binario usando complemento a 2 suponiendo 10 bits, y se obtiene el siguiente valor: 1111101100 
8.	Para realizar control del valor del error se realiza el siguiente calculo, suponiendo una Kp de 2 
                                     Control= 1111101100 * 2= 11111011000
9. Finalmente, se crea un mensaje con el sensor de velocidad, error, y valor de control en el formato adecuado para enviar a la unidad de control. 
                                           
### Aplicación 2: 
### Una aeronave se encuentra volando a una altura de 1000 ft, se requiere saber el proceso de la computadora para interpretar los datos que llegan desde los sensores. 

### Procedimiento que se debe seguir:
1. Un sensor de altitud ubicado en una aeronave detecta una altura de 1000 ft, esto genera un dato binario de 10 bits. 
2. Luego, debe detectar de que sensor le está llegando la señal en 2 bits, en este caso la señal le está llegando de 01 que es altitud 
3. Ahora debe decodificar y verificar el bit de paridad para detectar errores y descartar datos si se detecta un error 
4. Enviar nuevamente el dato de velocidad con las decodificaciones 
5. Convertir los datos binarios a decimal para facilitar visualización 
6. Ahora con el dato velocidad calcular el error para esto usar error=valor medido-setpoint
7. El valor calculado del error convertirlo de decimal a binario 
8. El valor calculado de velocidad del error calculado en binario hacerlo control proporcional a los valores de error con control=error*kp 
9. Ese valor obtenido codificarlo en formato adecuado para ser enviada a la unidad de control de la aeronave

### Procedimiento numérico: 
1. Recibe el dato de altitud de 1000 ft y lo convierte a binario en 10 bits y da un valor de: 1111101000
2. En 2 bits, identificar que señal le esta llegando, en este caso 01-que hace referencia a la altitud
3. Obtenemos este dato con la señal de que viene del sensor de velocidad y se agrega el bit de paridad 0. El valor obtenido es de 01 1111101000 0
4. Se envía el dato de velocidad con las decodificaciones y se verifica que la paridad es correcta 
5. Se convierten los datos de binarios en decimal para facilitar la visualización y obtenemos nuevamente el valor de 1000
6. Para calcular el error se utilizará un set point de 1500, por lo tanto el calculo sería: 
Error=1000-1500= -500
7. El valor calculado se convierte de decimal a binario usando complemento a 2 suponiendo 12 bits, y se obtiene el siguiente valor: 11000001100
8. Para realizar control del valor del error se realiza el siguiente calculo, suponiendo una Kp de 2 
Control=11000001100*2 =11000011000
9. Finalmente, se crea un mensaje con el sensor de altitud, error, y valor de control en el formato adecuado para enviar a la unidad de control. 

### Aplicación 3: 
### Una aeronave se encuentra volando a una temperatura de -15 °C, se requiere saber el proceso de la computadora para interpretar los datos que llegan desde los sensores. 

### Procedimiento que se debe seguir:
1. Un sensor de altitud ubicado en una aeronave detecta una temperatura de -15 °C, esto genera un dato binario de 12 bits. 
2. Luego, debe detectar de que sensor le está llegando la señal en 2 bits, en este caso la señal le esta llegando de 10 que es la temperatura.  
3. Ahora debe decodificar y verificar el bit de paridad para detectar errores y descartar datos si se detecta un error 
4. Enviar nuevamente el dato de velocidad con las decodificaciones 
5. Convertir los datos binarios a decimal para facilitar visualización 
6. Ahora con el dato velocidad calcular el error para esto usar error=valor medido-setpoint
7. El valor calculado del error convertirlo de decimal a binario 
8. El valor calculado de velocidad del error calculado en binario hacerlo control proporcional a los valores de error con control=error*kp 
9. Ese valor obtenido codificarlo en formato adecuado para ser enviada a la unidad de control de la aeronave

### Procedimiento numérico: 
1. Recibe el dato de temperatura de -15°C y lo convierte a binario en 12 bits y da un valor de: 11111110001
2. En 2 bits, identificar que señal le esta llegando, en este caso 10-que hace referencia a la temperatura
3. Obtenemos este dato con la señal de que viene del sensor de velocidad y se agrega el bit de paridad 1. El valor obtenido es de 11111110001101
4. Se envía el dato de velocidad con las decodificaciones y se verifica que la paridad es correcta 
5. Se convierten los datos de binarios en decimal para facilitar la visualización y obtenemos nuevamente el valor de -15
6. Para calcular el error se utilizará un set point de -20, por lo tanto el calculo sería: 
Error=-15-(-20) = 5
7. El valor calculado se convierte de decimal a binario y se obtiene el siguiente valor: 101
8. Para realizar control del valor del error se realiza el siguiente calculo, suponiendo una Kp de 2 
Control= 101*2= 1010
9.	Finalmente, se crea un mensaje con el sensor de temperatura, error, y valor de control en el formato adecuado para enviar a la unidad de control. 

### Conclusión: 
La transmisión de datos en formato binario desde sensores de una aeronave hacia su unidad de control es primordial por su eficiencia, precisión y fiabilidad. Al eliminar la necesidad de conversiones, se agiliza el procesamiento de la información y se reduce la latencia. La representación binaria permite una mayor resolución en las mediciones y facilita la implementación de sistemas de detección de errores. Además, la flexibilidad de los protocolos digitales y la posibilidad de aplicar técnicas de cifrado y autenticación hacen que esta forma de transmisión sea altamente segura. En resumen, el uso de datos binarios en la aviónica garantiza un control más preciso y confiable de la aeronave, mejorando la seguridad y eficiencia del vuelo.