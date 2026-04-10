# Sesión 1
## Charter
Explorar el flujo completo de compra y comportamiento del carrito, utilizando diferentes combinaciones de productos y acciones (agregar, eliminar, repetir ítems), para identificar inconsistencias en el cálculo de totales, actualización del carrito y continuidad del flujo de pago.
## ÁREAS
Catálogo de productos, carrito de compras y proceso de checkout en la aplicación JPetStore.
## INICIO
10/04/2026 - 12:30 (Duración aproximada: 35 minutos)
## TESTER
Jackelin Arami Peña Cabrera
## DESGLOSE DE TAREAS
10 min: Exploración del catálogo y selección de productos
15 min: Pruebas sobre el carrito (agregar, eliminar, repetir productos)
10 min: Validación del flujo de compra y comportamiento ante mensajes del sistema
## ARCHIVOS DE DATOS
Datos propios generados durante la navegación (productos disponibles en el sistema, sin uso de datos externos).
## NOTAS DE PRUEBA
Se agregaron múltiples productos al carrito desde distintas categorías.
Se probaron productos repetidos para observar si el sistema los consolida o los muestra por separado.
Se eliminaron productos hasta dejar el carrito vacío.
Se validó el comportamiento del sistema al mostrar mensajes de advertencia.
Se intentó continuar el flujo de compra luego de recibir mensajes inconsistentes.
Se observó lentitud en la carga de algunas páginas durante la navegación.
## LISTA DE RIESGOS
El sistema podría calcular incorrectamente el total y subtotal del carrito.
El usuario podría continuar el proceso de compra con información inconsistente.
El carrito podría no reflejar correctamente el estado real de los productos.
Problemas de rendimiento podrían afectar la experiencia del usuario.
Posible confusión del usuario al no entender cómo se gestionan productos repetidos.
## DEFECTOS (BUGS)
Al cambiar el idioma a español, la descripción de los animales se muestra de forma incorrecta, concentrándose en un solo elemento en la parte superior en lugar de distribuirse correctamente en cada producto.
Al modificar la cantidad de un producto en el carrito, el costo total no se actualiza automáticamente. El costo total solo se actualiza al presionar la tecla Enter, sin indicación visible para el usuario.
El ícono del carrito no muestra la cantidad de productos cuando existen ítems agregados.
## INCIDENTES (ISSUES)
No está definido si los productos repetidos deben consolidarse o mostrarse individualmente.
No está claro el comportamiento esperado cuando el carrito queda vacío.
No hay definición sobre la persistencia del carrito al recargar la página.
Lentitud en la carga de páginas: no está claro si es comportamiento esperado o un problema de performance.