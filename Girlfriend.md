![http://i35.tinypic.com/16i8u8y.jpg](http://i35.tinypic.com/16i8u8y.jpg)

# Introducción #

Girlfriend es un programa que permite bloquear un PC cuando no detecta la presencia vía Bluetooth de un dispositivo 'maestro' (típicamente un móvil)


adicionalmente, actua a modo de 'sonar' registrando toda la actividad bluetooth que vea el dispositivo, creando un fichero de log con los in / out detectados


## Manual de uso ##

Una vez descargado el programa, debes identificar la dirección física del dispositivo que hará de maestro. Una vez obtenida la dirección física debes incluirla dentro del fichero config.txt que debe estar en el mismo directorio que el ejecutable.

Para obtener la dirección fisica del dispositívo puedes emplear el ejecutable inquiry.exe que, basicamente, lista los dispositivos visibles

Hecho esto, simplemente ejecuta Girlfriend.exe

Puedes visualizar los logs de los dispositivos detectados en el fichero bluelog.txt