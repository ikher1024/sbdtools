AM I SPAMMER? es una herramienta pensada para comprobar por línea de comandos si una dirección IP aparece actualmente en alguna lista negra debido a denuncias/reputación de Spam.

El objetivo principal son administradores de sistemas o consultores de seguridad que deseen comprobar por línea de comandos la reputación de la(s) direccion(es) IP de las que son de su responsabilidad o que están auditando (respectivamente).

Para ello, AM I SPAMMER? comprobará en más de 90 listas populares de blacklisting, utilizadas por los diversos mecanismos antispam, para determinar la probabilidad de que un correo entrante sea deseado o no.

Como opción, permite enviar un email a un destinatario cuando termine de efectuar la comprobación enviando un mensaje con las diferentes listas en las que aparece la dirección IP como spammer. Esto es muy útil si se efectúa esta tarea de forma automatizada por ejemplo, todas las noches, o con mayor frecuencia incluso, en lugares donde el correo sea una actividad muy crítica. Sólo enviará un email en caso de que el resultado de la búsqueda sea positivo.

La herramienta está desarrollada íntegramente en Perl. Requiere el módulo Net::DNS. Si queremos que nos envíe un email con el resultado, entonces necesitaremos el módulo Mail::Sender

Se ha probado su funcionalidad sobre sistemas operativos UNIX (Linux y Mac OS X) y Windows (XP y 2003).

Changelog

Versión 11/01/2010     Descargar

  * Mensaje con confirmación de la razón de bloqueo basado en registros TXT DNS cuando la IP aparece en alguna lista negra
  * Detección automatica de dirección IP si no se introduce via línea de comandos con el flag -i
  * Opción -d para comprobar todos los registros MX DNS que pertenezcan al dominio indicado o si la IP es dinámica o no conocida.
  * Opción -h para mostrar la ayuda del programa.
  * Opción -T 0|1 (por defecto es 1). Usa hilos mientras hace el análsis de cada IP contra todas las listas negras a la vez (-T 0) o hazlos de forma iterativa (-T 1)

Versión 19/12/2009     Descargar

  * Lanzamiento inicial