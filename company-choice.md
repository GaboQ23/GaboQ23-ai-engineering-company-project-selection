# Elección de empresa: TrackFlow

## Por qué elegí TrackFlow

Elegí TrackFlow porque me atrae la logística y resolver problemas reales con datos e IA, donde cada sistema conecta con un paquete físico que viaja desde una estantería hasta la puerta de alguien. Me interesa la complejidad de unificar dos países, dos idiomas y dos stacks técnicos: los almacenes de Los Ángeles y Zaragoza usan sistemas distintos y no ven el inventario del otro. Me llamó la atención que para seguir un paquete haya que consultar uno por uno los portales de 8 transportistas (UPS, FedEx, DHL, MRW, SEUR...) y que no existan datos históricos de su rendimiento. Es un problema de datos muy concreto, medible y con mucho impacto, que es justo lo que quiero practicar.

## Departamentos que más me interesan

- **Operaciones de Almacén (Ana Whitfield, ~70 operarios):** los dos almacenes funcionan con sistemas distintos, no hay inventario en tiempo real a nivel global y las discrepancias se detectan tarde. Me interesan la API de inventario unificada y las alertas de stock.
- **Última Milla y Gestión de Transportistas (Carlos Vega):** la asignación de transportista es manual y el seguimiento obliga a consultar cada portal por separado. Me interesan el seguimiento unificado y la selección inteligente de transportista.
- **Logística Inversa (Sofía Ramos, equipo de 5 personas):** las devoluciones son entre el 18% y el 25% del volumen y todas pasan por revisión manual, sin criterios automáticos. Me interesan la aprobación automática y la inspección asistida por IA, porque una devolución es un paquete que vuelve y también hay que seguirlo.

## Reto de IA que más quiero construir

Seguimiento unificado de productos y paquetes: saber en tiempo real dónde está cada producto (en qué almacén) y cada paquete (en qué transportista y en qué estado) desde un solo lugar, y recomendar el mejor transportista para cada envío según destino, peso y urgencia.

## Mi idea de Agente de IA

**Agente de Seguimiento y Recomendación de Transportista** para el equipo de Carlos Vega.

**Qué haría:**
- Cuando entra un pedido, mira en qué almacén hay stock y recomienda qué transportista conviene según destino, peso y urgencia, explicando por qué en una frase.
- Después de enviar, vigila el estado del paquete en todos los transportistas y lo muestra en un único lugar, sin tener que entrar a cada portal.
- Detecta problemas antes de que escalen (paquete detenido, entrega fallida, dirección incorrecta, retraso) y propone qué hacer.
- Aprende con el tiempo qué transportistas fallan más en cada ruta, por ejemplo por retrasos o paquetes dañados, y lo tiene en cuenta en sus recomendaciones.
- Si el caso es dudoso, lo pasa a un coordinador logístico en lugar de decidir solo.

**Qué información necesitaría:**
- El stock por SKU en los almacenes de Los Ángeles y Zaragoza.
- Los datos del pedido: destino, peso, urgencia y cliente.
- Los estados de envío que reportan los 8 transportistas.
- El histórico de entregas: entregas a tiempo, incidencias por ruta y coste por kilo.

**Qué produciría o desencadenaría:**
- Una recomendación de transportista para cada envío, con su explicación.
- Un estado unificado de cada paquete, que sirve para el portal público de seguimiento y para Experiencia del Cliente.
- Alertas al coordinador cuando hay una incidencia, y alertas de stock bajo al equipo de compras.
- Datos para el dashboard de rendimiento de transportistas, algo que hoy TrackFlow no tiene.
- Sigue también los paquetes que vuelven: cuando un cliente inicia una devolución, muestra su estado en el mismo lugar que los envíos y avisa al equipo de Logística Inversa cuando llega al almacén.

Así el equipo de 6 coordinadores dejaría de buscar paquetes a mano y dedicaría su tiempo a resolver las incidencias reales.
