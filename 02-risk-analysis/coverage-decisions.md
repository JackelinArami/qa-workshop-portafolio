# Coverage Decisions

## Riesgos que se probarán primero
1. El sistema podría aprobar un pago pero no generar el pedido correspondiente
2. El inventario podría no sincronizarse correctamente entre la aplicación web y la API
3. El sistema podría permitir finalizar la compra sin autenticación del usuario

## ¿Por qué esos riesgos son prioridad?
Estos riesgos son prioritarios porque impactan directamente en:

- Ingresos del negocio (flujo de pago y generación de pedidos)
- Experiencia del usuario (compras fallidas o inconsistentes)
- Seguridad y trazabilidad de las operaciones

Además, corresponden a los flujos críticos del sistema, como el checkout, la gestión de pedidos y la consistencia del inventario.

## Qué se probará menos o quedará fuera por ahora
- Validaciones visuales de la interfaz (UI)
- Escenarios extremos de performance
- Funcionalidades de bajo uso dentro del sistema

## Justificación de exclusiones
Las áreas excluidas tienen menor impacto inmediato en el negocio y no afectan directamente los flujos principales de generación de ingresos.

Estas serán consideradas en fases posteriores, una vez que los flujos críticos estén validados y estabilizados.

El enfoque inicial se centra en asegurar que el sistema funcione correctamente en los procesos clave de compra y gestión de pedidos.