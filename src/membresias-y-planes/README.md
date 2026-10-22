# Membresías y Planes — esqueleto conceptual

**Sin implementación: modelo táctico pendiente Sesiones 5–6.**

## Propósito y frontera

Representar la oferta de planes de Nodo, las condiciones de cada contratación y los derechos/beneficios que se derivan de ella. El alcance es una sola frontera conceptual, no tres BC.

## Capacidades internas

- **Catálogo de Planes:** modalidades ofrecidas y condiciones generales.
- **Gestión de Membresías:** contratación, condiciones contratadas, vigencia, renovación, cambio, cancelación y finalización.
- **Administración de Beneficios:** derechos, horas incluidas/utilizadas/acumuladas/caducadas y consumos adicionales.

## Lenguaje ubicuo

Plan ofertado, condiciones contratadas, membresía, miembro, vigencia, activa, al día, beneficio incluido, beneficio disponible, saldo, horas reservadas, horas utilizadas, consumo adicional. Sus distinciones y términos pendientes están en [glosario](../../docs/02-glosario.md).

## Reglas candidatas

Se conserva RN-01–RN-15 y se distinguen INV-01–INV-07 de POL-01–POL-09 en [reglas e invariantes](../../docs/06-reglas-invariantes.md). Activación, gracia, titularidad del plan de equipo, cambios de catálogo y momento de consumo/restauración siguen sujetos a H-01–H-12.

## Fuera de esta frontera

Disponibilidad/ocupación; facturas, cobros y pagos; cálculo del precio final; autorización e ingreso físico; administración de inventario de espacios; contratación de eventos; envío transversal de notificaciones. Los límites y relaciones están en [Context Map](../../docs/05-context-map.md).

No se crean entidades, agregados, value objects, repositorios, interfaces, casos de uso, APIs, eventos técnicos, bases de datos ni código de aplicación en esta etapa.
