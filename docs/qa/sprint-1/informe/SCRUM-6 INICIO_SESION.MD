# Comprobaciones de autenticación

## Inicio de sesión correcto

### Pasos realizados

1. Se ingresa a la aplicación web.
2. Se accede al módulo de inicio de sesión.
3. Se ingresan las credenciales:

- Usuario: `jorgeramos`
- Contraseña: `********`

### Resultado esperado

El sistema debe permitir el acceso con credenciales válidas y redireccionar al usuario a la vista correspondiente.

### Resultado obtenido

El inicio de sesión se realiza correctamente.

### Estado

PASS

### Evidencia

![Ver video de inicio de sesión](../evidencias/img/iniciosesion.mp4)

---

## Control de visibilidad de contraseña

### Hallazgo

El campo de contraseña no cuenta con un control para mostrar u ocultar temporalmente los caracteres ingresados.

### Clasificación

Mejora de usabilidad / UX.

### Recomendación

Agregar un control de mostrar/ocultar contraseña mediante un ícono de ojo.

### Evidencia

![Ver captura del campo de contraseña](../evidencias/img/Captura%20desde%202026-09-04%2012-50-42.png)

---

## Cambio de contraseña

### Funcionalidad evaluada

El sistema permite solicitar el cambio de contraseña mediante un enlace enviado al correo electrónico del usuario.

### Hallazgos encontrados

Durante la prueba se identificaron las siguientes situaciones:

- El sistema permite utilizar contraseñas débiles.
- No se evidencian validaciones de complejidad alfanumérica.
- No se valida una longitud mínima de contraseña.
- No se valida si la nueva contraseña es igual a la contraseña anterior.
- La sesión permanece activa después del cambio de contraseña.
- El enlace enviado al correo no evidencia un tiempo límite de expiración.
- Después de crear la nueva contraseña, el sistema no redirecciona al inicio de sesión.
- No se recibe una confirmación posterior indicando que la contraseña fue modificada.

### Resultado esperado

El sistema debería aplicar las políticas de seguridad definidas para las contraseñas, controlar la validez del enlace de recuperación y proporcionar una confirmación clara al usuario después del cambio.

### Resultado obtenido

La contraseña puede ser modificada sin varias de las validaciones de seguridad esperadas.

### Estado

FAIL / Hallazgos de seguridad y usabilidad.

### Evidencia

![Ver video del cambio de contraseña](../evidencias/img/cambioclave.mp4)
