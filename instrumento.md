# Instrumento de recolección - Pasteleria Dulce Tentacion

Proyecto: Sistema de gestión de pedidos Pasteleria Dulce Tentacion
Fecha de aplicación: 18 de noviembre de 2026

---

<!-- ── Qué técnica se usa, y por qué ──────────────────────────────────── -->
## Técnicas seleccionadas

| Técnica | A quién | Qué se busca | Por qué esta técnica |
|---|---|---|---|
| Entrevista semiestructurada | propietaria | el proceso completo y sus excepciones | requiere profundidad, y es una sola persona |
| Observación directa | mostrador, 2 horas | cómo se registra un pedido **de verdad** | lo que se hace no siempre es lo que se dice |
| Revisión documental | cuaderno de pedidos | volumen real y tipos de error | el dato ya existe, solo hay que contarlo |

No se aplica encuesta: el universo son dos personas, y una encuesta a dos
personas es una entrevista con menos información.

---

## Guía de entrevista

<!-- ── Cómo se escribe una pregunta ───────────────────────────────────── -->
**Apertura**

1. Cuénteme cómo es un día normal en la panadería, desde que abren.
2. ¿En qué momento del día aparecen los pedidos por encargo?

**El proceso actual**

3. Muéstreme cómo anota un pedido. *(observar, no interrumpir)*
4. ¿Qué datos anota siempre? ¿Cuáles a veces?
5. ¿Cómo sabe, en la mañana, qué tiene que preparar ese día?
6. ¿Qué pasa cuando la persona que anotó no está?

**Los problemas**

7. ¿Cuándo fue la última vez que un pedido salió mal? ¿Qué pasó?
8. ¿Con qué frecuencia le parece que ocurre algo así?
9. ¿Qué hace cuando eso pasa?

**El contexto de uso**

10. ¿Con qué tiene las manos ocupadas cuando llega un pedido?
11. ¿Quién más tendría que poder registrar o consultar?
12. ¿Usa el celular durante el trabajo? ¿Para qué?

**Cierre**

13. Si pudiera cambiar una sola cosa del proceso actual, ¿cuál sería?
14. ¿Hay algo que no le pregunté y que debería saber?

---
## Registro de la entrevista 

## Registro de la observación

| Momento | Qué se observó | Qué contradice o confirma |
|---|---|---|
| 09:15 | pedido tomado por teléfono, anotado en un papel suelto y pasado al cuaderno 20 min después | contradice "siempre se anota en el cuaderno" |
| 10:40 | consulta de lo que hay que preparar: se revisan 3 hojas hacia atrás | confirma los 15-20 minutos declarados |
| 11:05 | un pedido se anota sin el teléfono del cliente | el dato "siempre se anota el teléfono" no se cumple |

---

## Resultados que alimentan el documento

| Hallazgo | Dónde se usa |
|---|---|
| los pedidos telefónicos pasan por un papel intermedio | formulación del problema (causa) |
| se consulta hacia atrás por hojas, no por fecha | requerimiento funcional de consulta |
| el teléfono del cliente no siempre se registra | validación de campos obligatorios |
| se trabaja con las manos ocupadas | requerimiento **no funcional**: pocos campos, botones grandes |
