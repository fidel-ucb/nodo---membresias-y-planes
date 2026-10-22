# 08 · Hotspots y riesgos

Los hotspots son preguntas abiertas, no reglas. La prioridad se reproduce cuando la fuente la indica en su tabla final; las filas sin prioridad explícita quedan como “no indicada”. Los riesgos son escenarios potenciales, no incidentes confirmados.

## H-01–H-12 · Preguntas de validación

| Código | Proceso / pregunta | Impacto sobre frontera o regla | Prioridad |
|---|---|---|---|
| H-01 | Contratación — ¿En qué momento se considera activa una membresía y qué requisitos deben cumplirse? | Definición de estados y relación con Facturación/Acceso; RN-12, INV-01; activa no es sinónimo confirmado de vigente/al día. | Alta |
| H-02 | Ciclo de vida — ¿Qué pasa con varios cambios solicitados antes del siguiente ciclo? | Transiciones y condiciones efectivas; RN-05, INV-03, POL-01. | Media |
| H-03 | Catálogo/contratación — ¿Cambios comerciales del plan afectan membresías vigentes o solo nuevas contrataciones/renovaciones? | Cohesión interna Catálogo–Gestión; INV-02, POL-09. | Alta |
| H-04 | Beneficios — ¿Horas se descuentan al confirmar, comenzar o completar reserva? | Frontera con Reservas y reconocimiento de consumo; RN-11, INV-06/07, POL-04. | Alta |
| H-05 | Beneficios — ¿Cuándo se restituyen horas tras modificar o cancelar una reserva? | Frontera con Reservas y saldo; RN-11, INV-06, POL-04. | Alta |
| H-06 | Beneficios — ¿Se usan primero horas acumuladas más antiguas? ¿Desde cuándo se calcula caducidad? | Complejidad del saldo y política temporal; RN-09, INV-05, POL-05. | Media |
| H-07 | Plan de equipo — ¿Quién es titular y cómo se distribuyen derechos entre integrantes? | Titularidad y aplicación de unicidad; RN-03, INV-01 y posible responsabilidad interna. | Media |
| H-08 | Impago — ¿Qué derechos conserva el miembro durante el período de gracia? | Estados contractuales y coordinación Facturación/Acceso; RN-12/13, POL-06. | Alta |
| H-09 | Impago — ¿Los cinco días descritos en renovación mensual aplican a todas las modalidades y obligaciones? | Alcance de RN-13 y política de suspensión. | Alta |
| H-10 | Impago — ¿Regularizar restablece acceso automáticamente o requiere otra condición? | Frontera Facturación–Membresías–Acceso; RN-15, POL-07. | Alta |
| H-11 | Escritorio dedicado — ¿Quién asigna/libera el puesto y qué responsabilidad corresponde a Membresías y a Espacios y Recursos? | Frontera de recurso físico, R-09. | Media |
| H-12 | Beneficios/reservas — ¿Qué ocurre si dos reservas usan simultáneamente las últimas horas? ¿Se admite consumo adicional? | Coordinación/concurrencia y saldo; RN-11, INV-06/07, R-10. | Alta (agrupado con H-04/H-05 en la tabla de riesgos prioritarios). |

### Preguntas complementarias sin código H nuevo

El documento también plantea si una solicitud de cancelación puede retirarse antes de hacerse efectiva; cómo se confirma si horas se usan primero por antigüedad y qué ocurre con reservas futuras; cómo se distribuye una bolsa de equipo; y si beneficios aplican a eventos. No se crean identificadores nuevos. Relación directa con Tarifas y Precios y Agenda de Eventos sigue sin evidencia suficiente.

## R-01–R-10 · Riesgos potenciales

| Código | Riesgo | Consecuencia posible | Validación relacionada |
|---|---|---|---|
| R-01 | Interpretar de forma diferente activa, vigente y al día. | Autorizar reserva/ingreso bajo una condición distinta a la prevista. | Precisar operaciones por condición; H-01, H-08. |
| R-02 | Coordinación incompleta entre reservas y beneficios. | Descuento a destiempo, consumo duplicado u omisión de restitución. | Momento de consumo y restitución; H-04, H-05. |
| R-03 | Administración incorrecta de horas acumuladas. | Uso de horas caducadas o saldo incorrecto. | Orden de uso y cálculo de caducidad; H-06. |
| R-04 | Confundir plan ofertado y condiciones contratadas. | Aplicar cambios a contratos existentes sin corresponder. | Efecto de cambios del catálogo; H-03. |
| R-05 | Descoordinación entre obligación económica y acceso. | Mantener habilitación cuando corresponde restringirla o impedir ingreso tras regularizar. | Gracia, suspensión y recuperación; H-08–H-10. |
| R-06 | Confundir consumo adicional, precio y cargo. | Consumos omitidos, importes incorrectos o cargos duplicados. | Responsabilidades de Membresías, Tarifas y Facturación. |
| R-07 | Distribuir incorrectamente derechos en plan de equipo. | Consumo/asignación incompatible con contrato. | Titularidad y uso compartido; H-07. |
| R-08 | Depender de comunicaciones transversales sin significado definido. | Omitir avisos o comunicar un estado aún no reconocido por su modelo responsable. | Acontecimientos, destinatarios y responsable semántico. |
| R-09 | Asignar escritorio dedicado sin responsabilidad definida. | Asignaciones incompatibles o puesto no liberado. | Quién asigna/controla/libera; H-11. |
| R-10 | Consumos concurrentes sobre un saldo. | Beneficios duplicados o cálculo incorrecto de horas disponibles. | Reservas simultáneas/exceso; H-12. |

## Insumos para Sesión 4

Por cada vecino, acordar qué hecho/dato se intercambia, qué significa, quién toma la decisión y qué casos de error/temporalidad se aceptan. Preguntas: (1) ¿qué evento compromete o consume horas y cómo se revierten cambios? (2) ¿qué estado económico afecta derechos y con qué plazos? (3) ¿qué condiciones habilitan/restringen/restablecen el ingreso? (4) ¿requieren Tarifas y Precios y Membresías relación directa? (5) ¿hay beneficio de membresía aplicable a eventos? (6) ¿quién asigna/libera escritorios? (7) ¿qué comunicaciones se emiten, a quién y quién define su verdad?

Resolver con ejemplos, actores responsables, condiciones, lenguaje y modelo dueño; volver a valorar DD-02/03 si aparece independencia interna. No elegir todavía ACL, Customer/Supplier, OHS ni otro patrón. Ver [Context Map](05-context-map.md), [reglas](06-reglas-invariantes.md) y [ADR](../decisiones/0004-hotspots-y-decisiones-pendientes.md).
