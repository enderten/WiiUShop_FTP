Wii U Offline Shop - README.txt
===============================

Este proyecto te permite enviar juegos (formato WUP) desde tu Mac/PC a tu Wii U usando WiFi y FTPiiU Everywhere, con una interfaz web tipo eShop.

----------------------------------------------------------
INSTRUCCIONES DE USO

1) Requisitos previos:
----------------------
- Tener Python 3 instalado en tu Mac o PC.
- Instalar las dependencias necesarias:
    pip3 install flask python-dotenv

- Tu Wii U debe estar con el Homebrew Launcher y el homebrew FTPiiU Everywhere activo. 
  (Anotá la IP local que te muestra la Wii U al iniciar FTPiiU Everywhere.)

2) Cómo iniciar el servidor:
----------------------------
- Abre la terminal.
- Navega a la carpeta del proyecto, por ejemplo:
    cd /Users/tu_usuario/Downloads/WiiU_OfflineShop

- Inicia el servidor ejecutando:
    python3 app.py

3) Acceder a la tienda:
-----------------------
- Abrí tu navegador web y entra a:
    http://127.0.0.1:5000
  (o desde otra PC/telefono en la misma red, usa la IP local que aparece en la terminal, ej: http://192.168.100.185:5000 )

4) Enviar juegos:
-----------------
- Copia tus juegos en formato WUP dentro de la carpeta:
    static/games/
  (Cada juego debe estar en su propia carpeta, ejemplo: static/games/ZeldaBotW/[app, h3, tmd, ...])

- En la web, ingresa la IP de tu Wii U (la que aparece en FTPiiU Everywhere) y haz click en "Instalar" sobre el juego que quieras transferir.

- El juego será copiado automáticamente a la Wii U en la carpeta correcta.

5) Instalar el juego en Wii U:
------------------------------
- En tu Wii U, abre el homebrew WUP Installer GX2 y deberías ver el juego listo para instalar en la lista.

----------------------------------------------------------
Cualquier duda, contactá a tu programador favorito ;)

¡Disfrutá tu propia eShop offline!
