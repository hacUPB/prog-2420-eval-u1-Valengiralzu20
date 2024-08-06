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
