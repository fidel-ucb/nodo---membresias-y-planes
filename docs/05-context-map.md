# 05 · Context Map

Propuesta hasta Sesión 3: el BC propio `Membresías y Planes` ocupa el centro y contiene Catálogo de Planes, Gestión de Membresías y Administración de Beneficios. Las seis cajas vecinas son **candidatos de delimitación**, no BC resueltos por este equipo.

![Figura 9. Context Map de Nodo](figuras/figura-09-context-map.png)

## Leyenda y límites

- **Línea continua:** relación identificada en los procesos con Reservas y Disponibilidad, Facturación y Cobros o Control de Acceso.
- **Línea discontinua:** relación directa que aún se debe validar, en particular con Tarifas y Precios, Agenda de Eventos y Espacios y Recursos.
- **Sin flechas, dirección, dependencia ni patrón nombrado.** Las líneas solo expresan relación o hipótesis.
- Notificaciones se representa fuera de los contextos como capacidad transversal; no decide si una membresía está vigente, una factura pagada o una reserva confirmada.
- La figura conservada es el Context Map disponible para este análisis; no se generó un diagrama sustituto.

## Contextos candidatos vecinos

| Candidato | Subdominio / clasificación | Responsabilidad que conserva |
|---|---|---|
| Reservas y Disponibilidad | Core | Franjas, ocupación, disponibilidad, confirmación y restricciones de reserva. |
| Facturación y Cobros | Generic | Facturas, cargos, obligaciones, pagos, vencimientos y regularizaciones. |
| Control de Acceso | Generic | Credenciales, autorización operativa e ingreso físico. |
| Tarifas y Precios | Supporting | Tarifas, condiciones comerciales y determinación de importes. |
| Agenda de Eventos | Supporting | Solicitud, aprobación, contratación y confirmación de eventos. |
| Espacios y Recursos | Supporting | Identidad, características y capacidad de recursos físicos. |

## Qué pido / qué entrego / qué decisión conserva cada BC

| Relación candidata | Qué pide Membresías y Planes | Qué entrega Membresías y Planes | Decisión que conserva cada BC / estado |
|---|---|---|---|
| Reservas y Disponibilidad — continua | Reservas confirmadas, modificadas o canceladas, recurso y período. | Condiciones de utilización, derechos, beneficios y saldo aplicable. | Reservas decide ocupación/confirmación; Membresías decide derechos y cómo reconoce su consumo. H-04, H-05, H-12. |
| Facturación y Cobros — continua | Obligaciones vencidas, pagos y regularizaciones pertinentes. | Condiciones contratadas, cuota aplicable, cambios y consumos adicionales reconocidos. | Facturación reconoce obligaciones/pagos; Membresías interpreta consecuencias contractuales. H-01, H-08–H-10. |
| Control de Acceso — continua | Resultado pertinente de habilitación, restricción o recuperación. | Derecho contractual, horarios y restricciones que se derivan de la membresía. | Control de Acceso autoriza/ejecuta ingreso físico; Membresías conserva derechos contractuales. H-08–H-10. |
| Tarifas y Precios — discontinua | Importe aplicable si un proceso de Membresías lo requiere; necesidad directa no probada. | Modalidad, descuento y condiciones comerciales. | Tarifas decide importe; Membresías concede beneficio. Validar si el intercambio es directo o mediado por otros procesos. |
| Agenda de Eventos — discontinua | No hay necesidad directa establecida. | Eventualmente, condiciones/beneficios aplicables a eventos. | Eventos decide su contratación y aprobación; relación directa por validar. |
| Espacios y Recursos — discontinua | Eventualmente, identidad/características de puesto dedicado. | Condición contractual que justifica un derecho a puesto. | Espacios administra recursos; asignación/liberación del escritorio por resolver (**H-11**). La relación vía Reservas está identificada. |

La necesidad de intercambiar datos no significa compartir modelos ni transferir decisiones. Acontecimientos candidatos: `Reserva confirmada/modificada/cancelada`; `Membresía contratada/renovada/finalizada`; `Cambio de plan aplicado`; `Horas descontadas/restituidas` (estos dos últimos sujetos a H-04/H-05); `Factura vencida impaga`, `Pago regularizado`; `Acceso suspendido/restablecido`; e importe determinado sujeto a validación. `Reserva confirmada` no equivale a horas consumidas; factura impaga no equivale a membresía finalizada.

## Notificaciones y servicios externos

Notificaciones puede comunicar acontecimientos de contratación, cambio, cancelación, vencimiento, pago o reserva, según acuerde cada responsable. No define el significado, condición ni estado que comunica. Pasarelas de pago, proveedores de mensajería y dispositivos físicos serían servicios externos, no BC de Nodo por defecto; no se eligen mecanismos ahora.

## Escenarios y preguntas de coordinación

1. **Reserva con horas incluidas:** ¿en qué momento reserva compromete/consume saldo y cuándo se restituye tras cambiar/cancelar? **H-04, H-05, H-12**.
2. **Renovación impaga:** ¿qué derechos existen durante gracia, a qué modalidades aplica el plazo de cinco días y qué permite recuperar acceso? **H-01, H-08–H-10**.
3. **Horas extra:** Membresías reconoce el exceso; Tarifas determina importe; Facturación registra cargo. ¿Hace falta relación directa con Tarifas? Mantener separado consumo, precio final y cargo.
4. **Escritorio dedicado:** ¿quién asigna, evita duplicidad y libera el puesto? **H-11**.
5. **Cambio de catálogo:** ¿qué condiciones permanecen en contratos existentes y qué reglas recibe renovación? **H-03**; permite volver a evaluar límites internos.

Son preguntas para Sesión 4, no patrones ni contratos de integración asignados. El riesgo y el intercambio detallado están en [08-hotspots-riesgos.md](08-hotspots-riesgos.md).
