# ADR 0003 — Fronteras y relaciones con otros contextos

**Estado:** Aceptada provisionalmente  
**Etapa:** Diseño estratégico — Sesión 3  
**Decisiones relacionadas:** DD-05 a DD-09

## Contexto

El Bounded Context **Membresías y Planes** administra las condiciones contratadas, la vigencia de las membresías y los beneficios adquiridos. Sin embargo, algunos procesos necesitan información de otras capacidades de Nodo: reservar salas, reconocer pagos, permitir el ingreso o calcular el importe de consumos adicionales.

Debíamos decidir **dónde termina la responsabilidad de Membresías y Planes**, qué modelos vecinos intervienen y cómo reflejar esas relaciones sin atribuir a nuestro contexto decisiones que corresponden a otros.

## Decisión

Mantener **fronteras conceptuales separadas** y representar seis **Bounded Contexts vecinos candidatos**: Reservas y Disponibilidad, Facturación y Cobros, Control de Acceso, Tarifas y Precios, Agenda de Eventos, y Espacios y Recursos. Su delimitación definitiva deberá contrastarse con los equipos responsables.

En el Context Map se distinguirán las relaciones identificadas de aquellas cuya **comunicación directa** todavía debe validarse. **Notificaciones** se representará como una capacidad transversal, no automáticamente como un Bounded Context propio.

## Justificación

Las fronteras se justifican por decisiones y significados diferentes:

- **Reservas y Disponibilidad** decide si una sala puede ocuparse en una franja. **Membresías** determina qué horas y derechos tiene el miembro. Tener horas incluidas no garantiza disponibilidad física.
- **Facturación y Cobros** reconoce facturas, vencimientos y pagos. **Membresías** interpreta sus consecuencias contractuales. Una factura impaga no significa necesariamente que la membresía haya finalizado.
- **Control de Acceso** administra credenciales y autorizaciones de ingreso. **Membresías** establece las condiciones contractuales de acceso; tener ese derecho no equivale a haber abierto la puerta.
- **Tarifas y Precios** determina importes. El descuento concedido por un plan, el precio calculado y el cargo facturado son conceptos distintos.
- **Agenda de Eventos** gestiona solicitudes, depósitos y aprobaciones de eventos, que no deben confundirse con la contratación de una membresía.
- **Espacios y Recursos** administra los recursos físicos; queda por precisar quién asigna y libera un escritorio dedicado.

Estas diferencias permiten colaborar sin compartir obligatoriamente un único modelo de dominio.

## Alternativas no adoptadas

- **Incorporar reservas, cobros, acceso o precios a Membresías:** mezclaría reglas y responsabilidades distintas.
- **Suponer un Bounded Context definitivo por cada subdominio:** anticiparía decisiones que corresponden a los otros equipos.
- **Asignar flechas o patrones de integración:** excedería el alcance de la Sesión 3; se abordará en la Sesión 4.

## Consecuencias

- El **Context Map** mostrará relaciones identificadas con Reservas, Facturación y Control de Acceso, mediante líneas simples.
- Las relaciones directas con **Tarifas, Eventos y Espacios** seguirán marcadas como **pendientes de validación**.
- Cada contexto conservará la responsabilidad de interpretar sus propios conceptos y tomar sus decisiones.
- Notificaciones permanecerá como capacidad transversal. Los sistemas externos, como una pasarela de pagos, se distinguirán de los contextos de Nodo.

## Hotspots y revisión

- **H-04 y H-05:** cuándo se descuentan o restituyen horas al reservar o cancelar.
- **H-08 a H-10:** qué ocurre con los derechos y el acceso ante un impago o su regularización.
- **H-11:** quién asigna y libera escritorios dedicados.
- **Relaciones comerciales pendientes:** si Membresías intercambia información directamente con Tarifas y si existen beneficios aplicables a Eventos.

La decisión se revisará con las respuestas del experto y el análisis de los equipos vecinos.

**Referencia de respaldo:** análisis estratégico de Nodo, apartados 3 y 7; [`05-context-map.md`](../docs/05-context-map.md). La delimitación interna se documenta en el ADR 0001.
