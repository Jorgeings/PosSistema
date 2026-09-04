# Comprobaciones

## Inicio de sesion adecuado

1. se ingresa a la app web
2. nos vamos al modulo de inicio sesion
3. ingresamos las credenciales
 - usuario: jorgeramos
 - clave: pos123456.

[ inicio de sesion ](../evidencias/img/iniciosesion.mkv)

## control de visibilidad de contraseña

Mejorar - agregar control mostrar/ocultar contraseña debido a que no cuenta con el ícono

[ control mostrar/ocultar](../evidencias/img/Captura%20desde%202026-09-04%2012-50-42.png)

## Cambio de constraseña
El sistema permite cambiar la contraseña por medio de un link enviado al correo pero 
no tiene validaciones para la nueva contraseña:
 * validaciones alfanumerico
 * que no sea igual a la anterior
 * la cantidad minima de caracteres
 * mantiene la sesion abierta aunque se esta cambiando la clave
 * el correo que envia no tiene validacion o tiempo limite
 * Al crear la nueva contraseña no redirecciona al login
 * no llega confirmacion de cambio de clave

[ Video demostrativo ](../evidencias/img/cambioclave.mkv)

