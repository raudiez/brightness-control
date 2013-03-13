          brightness-control, release 1.2
===================================================



EN:  A very simple executable code to control the brightness of your laptop.
This program implements a script that allows increase and lower the backlight (brightness) of your laptop.
Read this file to know how to install it on your system. All the file are in english and spanish.

ES: Código ejecutable muy simple que controla el brillo de tu portátil.
Este programa implementa un script que permite subir y bajar la retroiluminacion (brillo) de tu portatil.
Lea este fichero para saber cómo instalarlo en su sistema. Todo el archivo está en inglés y en español.

EN: 
          ON WHAT HARDWARE DOES IT RUN?

This program run in all hardware, because it use Linux's System commands and Bash sentences; and Linux is compatible with most PCs.

          INSTALLING

Once the "brillo" file is download, put it into /bin as root:

    sudo cp brillo /bin/

And then, give executable permisions to it:

    sudo chmod +x /bin/brillo

Finally, edit the file /etc/rc.local , and insert the following lines before of the "exit 0" line:

          setpci -s 00:02.0 f4.b=00
          /bin/brillo &

It's done! Reboot your system and your brightness would work properly.



ES: 
          ¿EN QUÉ HARDWARE FUNCIONA?

Este programa funciona en cualquier hardware, porque usa comandos del Sistema Linux y sentencias Bash; y Linux es compatible con la mayoría de PCs.

          INSTALLING

Una vez que el archivo "brillo" esté descargado, póngalo dentro del directorio /bin como root:

    sudo cp brillo /bin/

Y luego, proporciónele permisos de ejecución:

    sudo chmod +x /bin/brillo

Finalmente, edite el archivo /etc/rc.local , e inserte las siguientes líneas antes de la línea "exit 0":

          setpci -s 00:02.0 f4.b=00
          /bin/brillo &

Listo! Reinicie su sistema y la iluminación de su portátil debería funcionar correctamente.
