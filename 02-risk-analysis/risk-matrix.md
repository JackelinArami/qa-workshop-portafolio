# Risk Matrix

| ID | Riesgo | Impacto | Probabilidad | Nivel | Justificación |
|----|--------|---------|--------------|-------|---------------|
| R1 | El sistema podría aprobar un pago pero no generar el pedido correspondiente | Alto | Alta | Crítico | Afecta directamente los ingresos y genera pérdida de confianza del cliente al no completar la compra |
| R2 | El inventario podría no sincronizarse correctamente entre la aplicación web y la API | Alto | Alta | Crítico | Puede provocar ventas de productos sin stock o inconsistencias operativas |
| R3 | El sistema podría permitir finalizar la compra sin autenticación del usuario | Alto | Media | Alto | Genera problemas de seguridad y dificulta la trazabilidad de pedidos |
| R4 | La API podría aceptar datos inválidos o incompletos en la creación de pedidos | Medio | Alta | Alto | Puede generar registros incorrectos y afectar la integridad de la información |
| R5 | El sistema podría calcular incorrectamente el total de la compra en el checkout | Alto | Media | Alto | Impacta directamente en ingresos y puede generar reclamos de clientes |
| R6 | El carrito de compras podría perder productos al actualizar la sesión o la página | Medio | Media | Medio | Afecta la experiencia del usuario y reduce la probabilidad de completar la compra |
| R7 | La API podría eliminar registros incorrectos al ejecutar operaciones de borrado | Medio | Baja | Medio | Puede causar pérdida de información crítica y afectar la consistencia del sistema |
| R8 | El sistema podría presentar tiempos de respuesta lentos en el proceso de compra | Medio | Media | Medio | Impacta la experiencia del usuario y puede reducir la conversión de ventas |