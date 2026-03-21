# Coverage Decisions

## Riesgos a probar primero (Alta prioridad)

1. El usuario no puede completar el registro correctamente
2. Registro de usuarios duplicados
3. Validación de datos obligatorios (campos vacíos o incorrectos)
4. Seguridad de contraseñas
5. Envío de correo de confirmación

---

## Justificación de prioridad

Estos riesgos impactan directamente en:

- La funcionalidad principal del sistema (registro de usuarios)
- La seguridad de la información
- La integridad de los datos
- La experiencia del usuario

Si alguno de estos falla, el sistema pierde valor para el negocio y puede afectar la confianza del usuario.

---

## Riesgos de menor prioridad

- Diseño visual de la pantalla
- Compatibilidad con navegadores poco utilizados
- Mensajes secundarios no críticos

---

## Justificación de exclusión

Se prioriza validar primero que el sistema funcione correctamente, sea seguro y permita registrar usuarios sin errores.

Los aspectos visuales o secundarios pueden ser evaluados en etapas posteriores sin afectar el funcionamiento principal del sistema.