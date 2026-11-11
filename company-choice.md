# Elección de empresa: TrackFlow

Elegí TrackFlow porque me atrae la logística y resolver problemas reales con datos e IA, donde cada sistema conecta con un paquete físico. Me interesa la complejidad de unificar dos países, dos idiomas y dos stacks técnicos. Además, sus retos combinan ingeniería de datos, agentes y visión por computador, que es justo lo que quiero practicar.

## Departamentos que más me interesan
- Logística Inversa (Sofía Ramos): aprobación automática de devoluciones e inspección asistida por IA.
- Experiencia del Cliente (Valentina Cruz): agente de primera línea y base de conocimiento con RAG.

## Reto de IA que más quiero construir
Sistema de inspección de devoluciones: el operario fotografía el producto y la IA clasifica su estado (reacondicionar, desechar, etc.).

## Mi idea de Agente de IA

Agente de Inspección de Devoluciones para el equipo de Sofía Ramos.

**Qué haría:**
- Cuando llega un paquete devuelto al almacén, el operario hace 2 o 3 fotos del producto con el móvil o la tablet.
- El agente analiza las fotos y clasifica el estado del producto: como nuevo, reacondicionar, dañado o desechar, explicando en una frase por qué (por ejemplo: "caja abierta pero producto sin marcas de uso").
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
