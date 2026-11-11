# Elección de empresa: TrackFlow

## Por qué elegí TrackFlow

Elegí TrackFlow porque me atrae la logística y resolver problemas reales con datos e IA, donde cada sistema conecta con un paquete físico que viaja desde una estantería en Los Ángeles o Zaragoza hasta la puerta de alguien. Me interesa la complejidad de unificar dos países, dos idiomas y dos stacks técnicos: hoy los dos almacenes ni siquiera pueden ver el inventario del otro. Me llamó la atención que entre el 18% y el 25% del volumen sean devoluciones y que todas pasen por revisión humana, y que el 80% de las consultas de clientes se pueda automatizar mientras 15 agentes las responden a mano. Además, sus retos combinan ingeniería de datos, agentes y visión por computador, que es justo lo que quiero practicar.

## Departamentos que más me interesan

- **Logística Inversa (Sofía Ramos, equipo de 5 personas):** cada devolución implica decidir si se aprueba, si se recoge y si el producto se reacondiciona o se desecha, y hoy no hay criterios automáticos ni una inspección consistente. Me interesan la aprobación automática de devoluciones y la inspección asistida por IA.
- **Experiencia del Cliente (Valentina Cruz, 15 agentes):** atienden a marcas (B2B) y consumidores (B2C) por correo, WhatsApp y teléfono, sin sistema de tickets, sin base de conocimiento (las respuestas salen de un Word en Google Drive) y sin cobertura fuera de horario. Me interesan el agente de primera línea y la base de conocimiento con RAG.

## Reto de IA que más quiero construir

Sistema de inspección de devoluciones: el operario fotografía el producto devuelto y la IA clasifica su estado (reacondicionar, revender, desechar, etc.). Hoy esa inspección es subjetiva e inconsistente y no deja datos sobre qué productos se devuelven más ni por qué.

## Mi idea de Agente de IA

**Agente de Inspección de Devoluciones** para el equipo de Sofía Ramos.

**Qué haría:**
- Cuando llega un paquete devuelto al almacén, el operario hace 2 o 3 fotos del producto con el móvil o la tablet.
- El agente analiza las fotos y clasifica el estado del producto: *como nuevo*, *reacondicionar*, *dañado* o *desechar*, explicando en una frase por qué (por ejemplo: "caja abierta pero producto sin marcas de uso").
- Compara lo que ve con el motivo de devolución que indicó el cliente (por ejemplo, "llegó roto") y avisa si no coincide.
- Aplica las reglas de cada marca cliente para recomendar qué hacer (devolver al stock, enviar a reacondicionar, desechar, reembolso total o parcial).
- Si no está seguro, no decide solo: pasa el caso a una persona del equipo para que lo revise.

**Qué información necesitaría:**
- Las fotos del producto devuelto.
- Los datos del pedido original: SKU, marca cliente, almacén (Los Ángeles o Zaragoza) y fecha de entrega.
- El motivo de devolución que dio el consumidor.
- Las reglas de devolución configuradas por cada marca cliente.
- Ejemplos de inspecciones anteriores hechas por el equipo, para aprender qué cuenta como "reacondicionable" en cada tipo de producto.

**Qué produciría o desencadenaría:**
- Un registro de inspección con la clasificación, las fotos y la explicación, guardado para cada devolución.
- La acción siguiente según el resultado: actualizar el inventario si el producto vuelve a stock, crear la orden de reacondicionamiento o marcarlo para desecho.
- Un aviso a Experiencia del Cliente para que el consumidor sepa el estado de su reembolso.
- Datos para el dashboard de devoluciones: qué productos y qué marcas se devuelven más y por qué motivos, algo que hoy TrackFlow no puede ver.

Así las inspecciones serían rápidas y consistentes entre los dos almacenes, y el equipo de 5 personas dedicaría su tiempo solo a los casos dudosos.
