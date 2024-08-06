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
                                          Error=500-520 
                                            Error=-20
7.	El valor calculado se convierte de decimal a binario usando complemento a 2 suponiendo 10 bits, y se obtiene el siguiente valor: 1111101100 
8.	Para realizar control del valor del error se realiza el siguiente calculo, suponiendo una Kp de 2 
                                     Control= 1111101100 * 2
                                          Control=11111011000
9. Finalmente, se crea un mensaje con el sensor de velocidad, error, y valor de control en el formato adecuado para enviar a la unidad de control. 
                                           
