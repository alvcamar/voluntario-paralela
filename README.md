# voluntario-paralela

En este proyecto, vamos a encontrar 2 archivos python.

Uno de ellos es un broker al que varios clientes mediante el archivo client.py van a poder conectarse para intercambiar informacion.
En el broker.py, vamos a tener que introducirle la dirección IP de nuestro ordenador para que empieze a ejecutarse y escuchar clientes.
Cuando empieze a ejecutarse, va a esperar a que se conecten clientes, y cuando se conecten, imprimirá un mensaje por pantalla 
avisando de que un cliente se ha conectado y la dirección ip del cliente. Una vez conectados los clientes, van a poder 
comunicarse a intercambiar información. Si un mensaje de los que se vayan a mandar es "quit", se cerrará la conexión y se eliminará
al cliente que ha puesto este mensaje del broker.

En cuanto al client.py, se va a tener que proporcionar el puerto del cliente, la dirección ip del cliente y la direccion ip del servidor, en este orden.
Se van a guardar los datos en un diccionario y e cliente va a intentar conectarse al broker.py, que debe ejecutarse anteriormente.
Este cliente va a poder mandar informacion (mensajes) al broker y cualquier persona conectada podra leerlos, y si se escribe "quit", inmediatamante 
se cierra la conexion de este cliente con el broker, se terminan de ejecutar el proceso que hace que se conecte al broker (client_listener),
se sale del servidor y se cierra el programa.
