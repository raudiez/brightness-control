##          brightness-control, release 1.3

Copyright (C) 2012/2013 Raúl Díez Sánchez.
Mail: rauldiez20@gmail.com

EN:  A very simple executable code to control the brightness of your laptop.
This program implements a script that allows increase and lower the backlight (brightness) of your laptop.
Read this file to know how to install it on your system. All the file are in english and spanish.

 This program is free software; you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation; either version 3 of the License, or
 (at your option) any later version.
 You can find the GNU GPL on http://www.gnu.org/licenses/gpl.html

ES: Código ejecutable muy simple que controla el brillo de tu portátil.
Este programa implementa un script que permite subir y bajar la retroiluminacion (brillo) de tu portatil.
Lea este fichero para saber cómo instalarlo en su sistema. Todo el archivo está en inglés y en español.

 Este programa es software libre; puedes redistribuirlo y/o modificarlo
 bajo los términos de la GNU General Public License tal y como se publicó por
 la Free Software Foundation; sea la version 3 de la Licencia, o cualquier versión posterior.
 Puedes encontrar la GNU GPL en http://www.gnu.org/licenses/gpl.html (en inglés).

EN: 
## ON WHAT HARDWARE DOES IT RUN?

This program run in all hardware, because it use Linux's System commands and Bash sentences; and Linux is compatible with most PCs.

## INSTALLING

Once the "brillo" file is download, put it into /bin as root:

    sudo cp brillo /bin/

And then, give executable permisions to it:

    sudo chmod +x /bin/brillo

Finally, edit the file /etc/rc.local , and insert the following lines before of the "exit 0" line:

          setpci -s 00:02.0 f4.b=00
          /bin/brillo &

It's done! Reboot your system and your brightness would work properly.


ES: 
## ¿EN QUÉ HARDWARE FUNCIONA?

Este programa funciona en cualquier hardware, porque usa comandos del Sistema Linux y sentencias Bash; y Linux es compatible con la mayoría de PCs.

## INSTALACIÓN

Una vez que el archivo "brillo" esté descargado, póngalo dentro del directorio /bin como root:

    sudo cp brillo /bin/

Y luego, proporciónele permisos de ejecución:

    sudo chmod +x /bin/brillo

Finalmente, edite el archivo * /etc/rc.local *, e inserte las siguientes líneas antes de la línea "exit 0":

          setpci -s 00:02.0 f4.b=00
          /bin/brillo &

Listo! Reinicie su sistema y la iluminación de su portátil debería funcionar correctamente.
