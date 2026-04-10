# Sesión 1

## Charter
Explorar el flujo completo de compra y comportamiento del carrito, utilizando diferentes combinaciones de productos y acciones (agregar, eliminar, repetir ítems), para identificar inconsistencias en el cálculo de totales, actualización del carrito y continuidad del flujo de pago.

## ÁREAS
Catálogo de productos, carrito de compras y proceso de checkout en la aplicación JPetStore.

## INICIO
10/04/2026 - 12:30 (Duración aproximada: 40 minutos)

## TESTER
Jackelin Arami Peña Cabrera

## DESGLOSE DE TAREAS
10 min: Exploración del catálogo y selección de productos

20 min: Pruebas sobre el carrito (agregar, eliminar, repetir productos)

10 min: Validación del flujo de compra y comportamiento ante mensajes del sistema

## ARCHIVOS DE DATOS
Datos propios generados durante la navegación (productos disponibles en el sistema, sin uso de datos externos).

## NOTAS DE PRUEBA
Se agregaron múltiples productos al carrito desde distintas categorías, observando que el sistema permite agregar productos repetidos sin una regla clara de consolidación.

Se probaron productos duplicados para evaluar si el sistema los agrupa o los muestra de forma individual, detectando falta de consistencia en su representación.

Se eliminaron productos de forma progresiva hasta dejar el carrito vacío, evaluando el comportamiento del sistema en este estado.

Se validó el comportamiento ante mensajes de advertencia, observando que estos no siempre bloquean el flujo de compra.

Se intentó continuar el proceso de compra luego de recibir mensajes inconsistentes, verificando que el sistema permite avanzar sin validar correctamente el estado del carrito.

Se percibió lentitud en la carga de algunas páginas durante la navegación, lo que podría afectar la experiencia del usuario.

## LISTA DE RIESGOS
El sistema podría calcular incorrectamente el total y subtotal del carrito.

El usuario podría continuar el proceso de compra con información inconsistente.

El carrito podría no reflejar correctamente el estado real de los productos.

Problemas de rendimiento podrían afectar la experiencia del usuario y la finalización de compras.

La falta de claridad en la gestión de productos repetidos podría generar confusión en el usuario.

## DEFECTOS (BUGS)
Bug 1: Al modificar la cantidad de un producto en el carrito, el costo total no se actualiza automáticamente.

Resultado esperado:
El costo total debería actualizarse automáticamente al cambiar la cantidad o al salir del campo.

Resultado actual:
El costo total solo se actualiza al presionar la tecla Enter, sin indicación visible para el usuario.

Impacto:
Medio – puede generar confusión en el usuario y errores en la percepción del total a pagar.

Bug 2: El ícono del carrito no muestra la cantidad de productos cuando existen ítems agregados.

Resultado esperado:
El ícono del carrito debería mostrar un contador visible con la cantidad de productos agregados.

Resultado actual:
Aunque existen productos en el carrito, no se muestra ningún número en el ícono.

Impacto:
Medio – genera confusión en el usuario y afecta la percepción de que la acción fue realizada correctamente.

## INCIDENTES (ISSUES)
1. No está definido si los productos repetidos deben consolidarse o mostrarse individualmente.
2. No está claro el comportamiento esperado cuando el carrito queda vacío.
3. No hay definición sobre la persistencia del carrito al recargar la página.
4. Lentitud en la carga de páginas: no está claro si es comportamiento esperado o un problema de performance.