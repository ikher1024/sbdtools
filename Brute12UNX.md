BRUTE12UNX es una herramienta pensada para crackear certificados digitales con formato PKCS12 mediante ataques de diccionario.

Tiene la misma funcionalidad que Brute12 de www.security-projects.com aunque destinada a funcionar sobre entornos UNIX y Mac OS X

Como opción permite enviar un email a un destinatario cuando termine de efectuar el ataque de diccionario contra el certificado digital, enviando la contraseña del mismo o un mensaje de error si no se encontraba en la lista proporcionada

La herramienta está desarrollada íntegramente en Perl y tiene como dependencias el módulo Crypt::OpenSSL::PKCS12
Si además queremos que nos envíe un email con el resultado, entonces necesitaremos el módulo Mail::Sender