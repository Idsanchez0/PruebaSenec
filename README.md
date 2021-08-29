# PruebaSenec
 Prueba de programación

#Antes de proceder a ejecutar los comandos de instalación por favor tomar en cuenta lo siguiente:
- Configurar el archivo .env para la base de datos.
- Configurar el archivo .env con la siguiente información para recibir los correos electrónicos:
-- Configuracion de correos:
    	MAIL_DRIVER=smtp
	MAIL_HOST=smtp.gmail.com	
	MAIL_PORT=465
	MAIL_USERNAME=pruebaseneca
	MAIL_PASSWORD=12345678PruebaSeneca
	MAIL_ENCRYPTION=ssl
	MAIL_FROM_ADDRESS=pruebaseneca@gmail.com
	MAIL_FROM_NAME="PruebaSeneca"

#Para el ingreso al sistema hay que ejecutar los siguientes comandos:
- composer install
- php artisan migrate
- php artisan db:seed --class=DataUser (Este comando permite insertar un usuario por defecto)
- php artisan serve

#Usuario por defecto:
- Email: prueba@gmail.com
- Password: 12345678

#Notas
- Para poder recibir el correo de confirmación al registrar un usuario utilizar la opción de registrar de la pantalla principal el cual fue pensado para el registro de usuarios administradores pero no se encuentra bloqueado con Middlewares

- El registro de usuarios creado dentro del crud fue realizado para usuarios que no tengan el rol de administradores

- En caso no acordarse de la contraseña también se creo un modulo de recuperación de contraseñas mediante correo electrónico.

- El ultimo inicio de sesión se puede observar al dar clic en la foto de la derecha, junto al botón de cerrar sesión, donde se despliega fecha, hora y Ip del equipo conectado

- El ultimo inicio de sesión se muestra al iniciar sesión por segunda ocasión.
