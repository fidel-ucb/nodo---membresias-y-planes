# 06 · Reglas, invariantes y políticas

Las RN describen reglas del negocio; las INV son condiciones que el modelo debería conservar; las POL son reacciones ante acontecimientos. “Candidata” no significa confirmada. Los detalles abiertos remiten a hotspots, no se elevan a reglas por conveniencia.

## RN-01–RN-15 · Reglas de negocio

| Código | Regla preservada | Estado / límite |
|---|---|---|
| RN-01 | Nodo ofrece pase diario, mensual flexible, escritorio dedicado y plan de equipo. | Modalidades documentadas. |
| RN-02 | Cada modalidad determina condiciones y derechos, incluidos horarios, horas de sala y descuentos. | Diferencias concretas por modalidad. |
| RN-03 | Un miembro no puede mantener dos membresías activas simultáneamente. | Titularidad de equipo por precisar (**H-07**). |
| RN-04 | Contratación mensual contempla compromiso mínimo de 30 días; no se extiende al pase diario. | Procedencia primaria debe verificarse. |
| RN-05 | Cambios de plan solicitados se aplican desde el ciclo de facturación siguiente. | Múltiples cambios antes del ciclo: **H-02**. |
| RN-06 | Cancelar una membresía renovable evita su continuidad en el ciclo siguiente, según condiciones contratadas, sin reembolso anticipado. | No implica necesariamente finalización inmediata. |
| RN-07 | Solicitar cancelación no implica necesariamente finalización inmediata de la membresía. | Distinguir solicitud y fin efectivo. |
| RN-08 | Derechos de utilización corresponden a las condiciones de la modalidad contratada. | Diferenciar oferta de contrato. |
| RN-09 | Horas de sala no utilizadas pueden acumularse por un máximo de un año. | Cálculo temporal/orden de uso por validar (**H-06**). |
| RN-10 | Horas utilizadas por encima de las incluidas se reconocen como consumo adicional sujeto a condiciones comerciales. | No equivale automáticamente a precio o cargo. |
| RN-11 | Reconocer consumo y eventual restitución debe coordinarse con acontecimientos de Reservas y Disponibilidad. | Momento exacto pendiente (**H-04, H-05**). |
| RN-12 | Utilización de determinados derechos está condicionada a vigencia contractual y cumplimiento de condiciones económicas. | No fusionar vigencia y estado de pago. |
| RN-13 | En el escenario de renovación mensual del caso, impago durante cinco días conduce a suspensión del acceso. | Extensión a otras modalidades por validar (**H-09**). |
| RN-14 | Factura pendiente no demuestra por sí sola que la membresía haya finalizado. | Obligación y vigencia distintas. |
| RN-15 | Regularización económica puede permitir recuperar acceso. | Condiciones exactas pendientes (**H-10**). |

La ocupación es responsabilidad de Reservas; importes, de Tarifas; cobros/pagos, de Facturación; ingreso operativo, de Control de Acceso. No se importan sus reglas al BC de membresías.

## INV-01–INV-07 · Invariantes candidatas

| Código | Condición candidata | Grado de respaldo / enlace |
|---|---|---|
| INV-01 | Un miembro no mantiene simultáneamente dos membresías activas. | Deriva de RN-03; tratamiento de equipos pendiente, H-07. |
| INV-02 | La membresía conserva condiciones contractuales identificables para el período al que corresponden sus derechos. | Coherencia candidata, no regla confirmada; H-03. |
| INV-03 | Cambio de plan no altera las condiciones efectivas antes del ciclo en que corresponde aplicarlo. | Deriva de RN-05; H-02. |
| INV-04 | Finalización de membresía mensual respeta compromiso mínimo y condiciones de cancelación aplicables. | Deriva de RN-04, RN-06 y RN-07; detalles por validar. |
| INV-05 | Horas acumuladas no se mantienen utilizables tras superar su período máximo de conservación. | Deriva de RN-09; cálculo temporal por validar, H-06. |
| INV-06 | El mismo consumo no se reconoce más de una vez sobre el saldo de una membresía. | Candidata por riesgo de duplicación/coordinación; H-04, H-05, H-12. |
| INV-07 | Horas que exceden los beneficios aplicables no se confunden con horas cubiertas por la membresía. | Candidata; cómo se reconoce el consumo adicional está abierto, H-04, H-12. |

El documento considera RN/INV-01, 03, 04 y 05 derivadas de reglas documentadas, aunque los detalles necesitan validación. INV-02, 06 y 07 requieren contraste. **No** se afirma que el saldo nunca sea negativo: el tratamiento de consumo adicional no está decidido. Tampoco son invariantes de este BC que toda factura esté pagada o que todo ingreso esté autorizado.

## POL-01–POL-09 · Políticas

| Código | Acontecimiento / condición | Reacción | Estado |
|---|---|---|---|
| POL-01 | Se solicita cambio de plan. | Registrar el cambio para aplicación en el ciclo correspondiente. | Regla documentada; múltiples solicitudes por resolver, H-02. |
| POL-02 | Se solicita cancelar membresía renovable. | Evitar continuidad del siguiente ciclo según condiciones contratadas. | Regla documentada. |
| POL-03 | Membresía alcanza fin de ciclo. | Evaluar renovación, cambio o finalización aplicables. | Política de ciclo; precisar condiciones por modalidad. |
| POL-04 | Se reconoce acontecimiento de reserva que utiliza beneficios. | Evaluar actualización del saldo correspondiente. | Candidata, H-04, H-05. |
| POL-05 | Se alcanza caducidad de horas acumuladas. | Dejar de considerar esas horas entre derechos disponibles. | Derivada de acumulación; precisión temporal, H-06. |
| POL-06 | Se cumplen condiciones de suspensión por impago. | Aplicar consecuencias sobre derechos y coordinar restricción de ingreso físico. | Regla del escenario de renovación mensual; alcance pendiente, H-08, H-09. |
| POL-07 | Se regulariza obligación económica. | Evaluar recuperación de derechos y autorizaciones correspondientes. | Candidata, H-10. |
| POL-08 | Se reconoce consumo superior a beneficios incluidos. | Identificar consumo adicional para valoración y facturación posteriores. | Regla de negocio; coordinación externa por precisar. |
| POL-09 | Se modifican condiciones de plan ofertado. | Determinar qué condiciones aplican a nuevas y existentes contrataciones. | Candidata, H-03. |

## Casos límite enlazados

| Caso | Códigos y hotspot |
|---|---|
| Segunda membresía activa / equipo compartido | RN-03, INV-01, H-07 |
| Cancelación antes de cumplir 30 días o retiro de solicitud | RN-04, RN-06, RN-07, INV-04 |
| Cambios repetidos antes de renovar | RN-05, INV-03, POL-01, H-02 |
| Cambio de oferta con contratos vigentes | INV-02, POL-09, H-03 |
| Reserva cancelada tarde / uso próximo a caducar / concurrencia | RN-09, RN-11, INV-05–INV-07, POL-04–POL-05, H-04–H-06, H-12 |
| Impago dentro de gracia y recuperación | RN-12–RN-15, POL-06–POL-07, H-01, H-08–H-10 |

La procedencia de las reglas cuya evidencia primaria no está disponible debe verificarse con el equipo. Los hotspots y los riesgos están en [08-hotspots-riesgos.md](08-hotspots-riesgos.md).
