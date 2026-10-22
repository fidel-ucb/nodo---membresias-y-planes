# ADR 0002 — Clasificación Core frente a Supporting

**Estado:** Aceptada para el escenario actual; revisable si cambia la estrategia de Nodo  
**Etapa:** Diseño estratégico — Sesión 3  
**Decisión relacionada:** DD-01

## Contexto

Nodo ofrece espacios de coworking, salas de reuniones y eventos mediante reservas y distintas modalidades de membresía. Para orientar el esfuerzo de diseño debemos identificar qué capacidad aporta su principal **ventaja competitiva**, en lugar de clasificar como *Core* todo aquello que resulta indispensable para operar.

Dos candidatos relevantes son **Reservas y Disponibilidad**, que administra la ocupación de los espacios, y **Membresías y Planes**, que establece las condiciones de contratación y los beneficios de los miembros.

## Decisión

Clasificar **Reservas y Disponibilidad como Core** y **Membresías y Planes como Supporting**, según la estrategia y los problemas de negocio descritos para Nodo.

## Justificación

La confiabilidad de las reservas incide directamente en la posibilidad de prestar el servicio prometido. Nodo necesita evitar que dos personas ocupen el mismo recurso en franjas incompatibles, respetar los **15 minutos de limpieza** entre reservas de una sala y gestionar situaciones en las que la demanda supera la disponibilidad.

Una reserva confirmada que luego no puede atenderse perjudica la experiencia del cliente y su confianza en Nodo. Por ello, el valor diferencial propuesto se concentra en **asignar recursos compartidos de manera confiable**, más que en ofrecer simplemente un calendario.

Membresías y Planes también es fundamental: define pases diarios, planes mensuales, escritorios dedicados y planes de equipo, así como horarios, horas de sala y descuentos. Sin embargo, **ser necesario o tener reglas complejas no basta para ser Core**. La evidencia disponible no identifica actualmente la personalización de membresías como el principal motivo por el que los clientes elegirían Nodo frente a otros coworkings.

## Alternativa considerada

**Membresías y Planes como Core.** Sería defendible si Nodo compitiera principalmente mediante planes muy personalizables, beneficios exclusivos o modalidades difíciles de replicar. Esta estrategia no está respaldada por el escenario analizado, por lo que **no se adopta actualmente**.

## Consecuencias

- Priorizar el diseño propio y la protección de las reglas críticas de **Reservas y Disponibilidad**, como la prevención de solapamientos.
- Conservar en **Membresías y Planes** el control de las reglas específicas de contratación, vigencia y beneficios, evaluando la reutilización de componentes para funciones comunes.
- Considerar soluciones existentes para capacidades genéricas, sin comprometer todavía tecnologías ni proveedores.
- Mantener esta clasificación independiente de la decisión de cuántos *Bounded Contexts* existen: **Core/Supporting clasifica subdominios, no contextos**.

## Cuestiones abiertas

- **Estrategia competitiva:** confirmar si la confiabilidad de las reservas sigue siendo el principal diferenciador de Nodo a medida que evolucione el negocio.
- **H-04 y H-05:** determinar cuándo se consumen y restituyen las horas incluidas al confirmar, modificar o cancelar reservas. Estas preguntas afectan la coordinación entre ambos modelos, **pero no cambian por sí solas su clasificación estratégica**.

**Referencia de respaldo:** análisis estratégico de Nodo, apartado 2, y decisiones DD-01. La delimitación de Membresías y Planes se explica en el ADR 0001.
