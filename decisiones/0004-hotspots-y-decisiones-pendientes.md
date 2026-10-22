# ADR 0004 — Gestión de hotspots y decisiones pendientes

**Estado:** Aceptada como criterio de trabajo; cuestiones pendientes de validación  
**Etapa:** Diseño estratégico — Sesión 3  
**Decisión relacionada:** DD-10

## Contexto

Al analizar la contratación, los beneficios y los impagos de las membresías de Nodo encontramos reglas conocidas, pero también preguntas que el caso y las entrevistas disponibles todavía no resuelven.

Estas dudas afectan decisiones importantes: cuándo se consumen las horas de sala, qué puede hacer un miembro durante un impago y cómo se aplican los cambios de plan a contratos vigentes. Resolverlas por suposición podría producir un modelo incorrecto o establecer fronteras de responsabilidad sin suficiente evidencia.

## Decisión

**Mantener explícitos los hotspots H-01 a H-12 y los riesgos R-01 a R-10**, sin presentar como confirmadas las respuestas que aún no ha dado el experto.

Distinguir en la documentación entre **reglas confirmadas**, **hipótesis del equipo** y **preguntas abiertas**. Posponer la elección de patrones de integración y el diseño táctico hasta las sesiones correspondientes.

## Justificación

Las incertidumbres identificadas pueden modificar el comportamiento del negocio y sus fronteras:

- **Impagos y acceso (H-01, H-08 a H-10):** el caso describe una suspensión del acceso tras cinco días de impago en una renovación mensual. No podemos asumir que el plazo o sus consecuencias sean iguales para todas las modalidades, ni que «membresía vigente», «pago al día» y «acceso habilitado» signifiquen lo mismo.
- **Consumo de beneficios (H-04, H-05 y H-12):** confirmar una reserva no aclara por sí solo cuándo se descuentan las horas, cuándo se restituyen ni qué ocurre si dos reservas utilizan simultáneamente las últimas horas disponibles.
- **Cambios comerciales (H-03):** falta precisar qué sucede con las membresías existentes cuando Nodo modifica las condiciones de un plan.
- **Casos particulares (H-02, H-06, H-07 y H-11):** siguen abiertas las reglas sobre cambios múltiples, caducidad de horas, planes de equipo y asignación de escritorios dedicados.

Los riesgos R-01 a R-10 describen **consecuencias posibles** de no resolver estas cuestiones; no son fallos observados del sistema.

## Alternativas no adoptadas

- **Completar las reglas mediante suposiciones:** daría una falsa sensación de certeza y podría contradecir al experto.
- **Decidir ahora mecanismos de integración o estructuras de código:** adelantaría decisiones propias de las Sesiones 4 a 6 sin contar con los acuerdos de negocio necesarios.

## Consecuencias

- Cada hotspot conservará su pregunta, prioridad y relación con el proceso afectado.
- Las hipótesis permanecerán identificadas como tales, y las reglas consideradas confirmadas deberán vincularse con su fuente.
- Cuando exista una respuesta validada, se actualizarán los artefactos afectados: glosario, EventStorming, Domain Storytelling, Context Map y reglas e invariantes.
- La selección de patrones entre contextos queda para la **Sesión 4**; el modelo táctico y su implementación, para las **Sesiones 5 y 6**.

## Revisión pendiente

La validación priorizará las cuestiones de **impago y acceso**, **consumo y restitución de horas** y **cambios de planes con contratos vigentes**. También debe aclararse si Membresías necesita una relación directa con Tarifas y si los beneficios de membresía se aplican a Eventos.

**Referencia de respaldo:** análisis estratégico de Nodo, apartados 5 a 9; [08-hotspots-riesgos.md](../docs/08-hotspots-riesgos.md).
