# 09 · Trazabilidad

Esta matriz enlaza conceptos y reglas con las secciones y páginas internas de la documentación estratégica consultada, los procesos de EventStorming y Domain Stories, los hotspots/invariantes y las decisiones. Los materiales documentales originales no se incluyen ni se enlazan en este repositorio. Las referencias de sección y página permiten localizar la evidencia en la documentación de trabajo que conserva el equipo.

## Etiquetas de procedencia

- **Caso inicial:** el análisis atribuye la afirmación al caso; la evidencia primaria no está disponible aquí.
- **Entrevista general:** el análisis presenta la afirmación como entrevista o confirmación del experto; la entrevista primaria no está disponible aquí.
- **Entrevista adicional no adjunta:** se menciona una respuesta adicional, pero no se dispone de evidencia concreta que permita atribuirle una regla.
- **Hipótesis del equipo:** interpretación, secuencia, evento o decisión propuesta durante el modelado; no es un hecho confirmado.
- **Procedencia pendiente de verificar:** la documentación no atribuye la afirmación con suficiente precisión al caso o a una entrevista, o presenta solo una formulación resumida.

Estas etiquetas describen la evidencia disponible y no son una auditoría independiente. Cuando la procedencia no se puede verificar, la regla se conserva tal como está documentada y la incertidumbre queda explícita.

## Matriz concepto/regla → origen → proceso → hotspot/invariante → decisión

| Concepto / regla | Origen interno: sección y página | EventStorming / Domain Story | Hotspot / invariante | Decisión |
|---|---|---|---|---|
| Reservas como Core; Membresías como Supporting | Análisis estratégico, §2, pp. 6–10; criterio de nivel Alto, p. 1 | Beneficios y contratación | Caso límite de subdominio | DD-01; conservar reglas propias sin fijar tecnología |
| Ocho subdominios; Notificaciones transversal | Análisis estratégico, §2, pp. 6–7 | Context Map | Relaciones con vecinos | DD-08, DD-09 |
| Un BC con tres capacidades | Análisis estratégico, §3, pp. 11–18; criterio de nivel Alto, p. 1 | Tres procesos; DS-01–DS-03 | H-03, H-06, H-07 | DD-02/DD-03, hipótesis provisional |
| Pase diario, mensual flexible, escritorio dedicado y equipo | Análisis estratégico, §§2, 4 y 8, pp. 9, 20–25, 82–83 | Contratación | H-07, H-11 | RN-01, DD-03; procedencia pendiente de verificar |
| Un miembro no mantiene dos membresías activas simultáneamente | Análisis estratégico, §2 p. 9; §8 pp. 82–83 | Contratación; alternativa DS-01 | H-07; INV-01 | DD-03; procedencia pendiente de verificar |
| Compromiso mínimo mensual de 30 días, no aplicable al pase diario | Análisis estratégico, §§2, 4 y 8, pp. 9, 21–23, 82 | Cancelación durante ciclo | INV-04 | RN-04, DD-04; procedencia pendiente de verificar |
| Cambio de plan efectivo desde el ciclo siguiente | Análisis estratégico, §§2, 4 y 8, pp. 9, 22–24, 82–83 | Solicitud y aplicación; DS-01 | H-02; INV-03 | RN-05, POL-01, DD-04; procedencia pendiente de verificar |
| Cancelación de renovación sin reembolso anticipado; solicitud distinta de finalización | Análisis estratégico, §§2, 4 y 8, pp. 9, 23–24, 82–83 | Alternativas del ciclo | Retiro de solicitud por aclarar; RN-06/RN-07 | POL-02, DD-04; procedencia pendiente de verificar |
| Beneficios dependen de condiciones contratadas | Análisis estratégico, §§1, 4 y 8, pp. 4, 20–26, 83 | Concesión y consumo; DS-02 | H-03/H-04; INV-02 | DD-04/DD-05; hipótesis del equipo |
| Horas no utilizadas acumulables hasta un año | Análisis estratégico, §§2, 4, 5 y 8, pp. 9, 25–27, 40–44, 83–84 | Acumulación y caducidad | H-06; INV-05 | RN-09, POL-05; procedencia pendiente de verificar |
| Exceso de horas como consumo adicional; cobro de fin de mes con descuentos | Análisis estratégico, §§5–6, pp. 38–42, 58–60 | Horas extra; DS-02 | H-04/H-12; INV-07 | RN-10, POL-08, DD-07; entrevista general según el análisis |
| Reserva confirmada requiere disponibilidad y plan al día; no demuestra consumo | Análisis estratégico, §§5–6, pp. 37–44, 58–61 | Reserva confirmada externa | H-04/H-05/H-12; INV-06 | RN-11, DD-05; entrevista general para confirmación e hipótesis del equipo para separar reserva/consumo |
| Cancelación gratuita de reserva hasta cuatro horas antes; después se cobra la franja | Análisis estratégico, §6, p. 65 | Excepción DS-02 | H-05; restitución no resuelta | Mantener cargo separado de restitución; procedencia pendiente de verificar |
| Cinco días de impago en renovación mensual antes de suspender acceso | Análisis estratégico, §§5–6, pp. 44–45, 63–65 | Impago; DS-03 | H-01/H-08/H-09; R-05 | RN-13, POL-06, DD-06; caso inicial según el análisis |
| Factura pendiente no demuestra que la membresía finalizó | Análisis estratégico, §8, p. 83 | Impago/acceso | H-08/H-09; R-01/R-05 | RN-14, DD-06; procedencia pendiente de verificar |
| Regularizar puede permitir recuperar acceso; condiciones abiertas | Análisis estratégico, §§5–6 y 8, pp. 45, 64–65, 83 | Pago regularizado → acceso restablecido (candidato) | H-10 | RN-15, POL-07, DD-06; procedencia pendiente de verificar |
| Derecho contractual de acceso distinto de autorización/ingreso físico | Análisis estratégico, §§3, 4 y 7, pp. 13–16, 28–30, 70–78 | Impago; DS-03 | H-08–H-10; R-01/R-05 | DD-06; hipótesis de delimitación |
| Descuento distinto de precio final y cargo | Análisis estratégico, §§3, 4 y 7, pp. 14–15, 29–31, 74–79 | Consumo adicional | R-06 | DD-07; hipótesis de delimitación |
| Relaciones directas con Tarifas, Eventos y Espacios pendientes | Análisis estratégico, §§3, 7 y 9, pp. 15–16, 70–81, 89 | Exceso, evento y escritorio | H-03/H-11; coordinación pendiente | DD-08; hipótesis del equipo |
| Notificaciones como capacidad transversal | Análisis estratégico, §§2 y 7, pp. 7, 72–76 | DS-03 to-be | R-08 | DD-09; hipótesis del equipo |
| Integración y diseño táctico se posponen | Análisis estratégico, §9, pp. 88–89; criterio de alcance, pp. 3–4 | Sin contrato técnico | Preguntas para Sesión 4 | DD-10 |
| F-01–F-09 y mejoras to-be | Análisis estratégico, §6, pp. 53–61 | DS-01–DS-03 | H-01–H-12 según la historia | Propuesta funcional, no requisito aprobado |

## Trazabilidad de identificadores

| Grupo | Sección y artefacto | Procedencia |
|---|---|---|
| RN-01–RN-15, INV-01–INV-07, POL-01–POL-09 | Análisis estratégico, §8, pp. 82–87; [06-reglas-invariantes.md](06-reglas-invariantes.md) | La tabla principal indica la etiqueta cuando corresponde; las formulaciones que el análisis marca como candidatas siguen siendo candidatas. |
| H-01–H-12 y prioridades | Análisis estratégico, §§5 y 9, pp. 46–51 y 89; [08-hotspots-riesgos.md](08-hotspots-riesgos.md) | Preguntas, no reglas. La clasificación de prioridad reproduce la registrada en el análisis. |
| R-01–R-10 | Análisis estratégico, §7, pp. 79–81; [08-hotspots-riesgos.md](08-hotspots-riesgos.md) | Riesgos potenciales, no fallos confirmados. |
| DD-01–DD-10 | Análisis estratégico, §9, pp. 88–89; ADR en [decisiones/](../decisiones/0001-delimitacion-unico-bounded-context.md) | Decisiones estratégicas; DD-02/DD-03 son hipótesis principales. |
| DS-01–DS-03, F-01–F-09 | Análisis estratégico, §6, pp. 52–67; [04-domain-stories.md](04-domain-stories.md) | As-is combina evidencia y reconstrucción; to-be es una propuesta. |

## Límites de evidencia

El análisis atribuye algunas observaciones al caso inicial y otras a una entrevista general, pero no se cuenta aquí con material primario que permita verificarlas de forma independiente. Aunque se mencionan respuestas adicionales del experto, no se dispone de evidencia concreta para asignarles reglas específicas. Cuando el origen no está indicado, se marca **Procedencia pendiente de verificar**. No se descartan ni reinterpretan las reglas registradas. No se incluye una exportación separada del mapa colaborativo.
