# ADR 0001 — Un único Bounded Context para Membresías y Planes

**Estado:** Aceptada provisionalmente  
**Etapa:** Diseño estratégico — Sesión 3  
**Decisiones relacionadas:** DD-02 y DD-03

## Contexto

En Nodo identificamos tres capacidades dentro del subdominio **Membresías y Planes**:

- **Catálogo de Planes:** define las modalidades ofrecidas y sus beneficios.
- **Gestión de Membresías:** administra las contrataciones, renovaciones, cambios y cancelaciones.
- **Administración de Beneficios:** mantiene los derechos de uso y saldos de horas de cada membresía.

Debíamos decidir si estas capacidades requerían modelos separados (*Bounded Contexts*) o si podían compartir uno. Una división funcional no implica, por sí sola, una frontera de modelo.

## Decisión

Mantener **un único Bounded Context, `Membresías y Planes`**, con las tres capacidades anteriores organizadas internamente, pero **sin tratarlas como contextos independientes**.

## Justificación

Las capacidades comparten un modelo coherente de **oferta comercial → condiciones contratadas → derechos adquiridos**. Por ejemplo, el Catálogo define las horas incluidas de un plan; Gestión de Membresías establece qué condiciones contrató un miembro; y Administración de Beneficios controla las horas que le corresponden y su utilización.

Contrastamos la separación mediante lenguaje ubicuo, independencia de reglas, responsables, EventStorming y Domain Storytelling. Aunque encontramos responsabilidades distintas, **no hay evidencia suficiente de modelos internos incompatibles o autónomos**.

En cambio, sí aparecen fronteras externas más claras: **Reservas** decide la ocupación de salas; **Facturación** gestiona obligaciones y pagos; y **Control de Acceso** administra el ingreso físico. Membresías conserva las condiciones contractuales y los beneficios.

## Alternativas no adoptadas

- **Dos contextos (Catálogo / Membresías y Beneficios):** permitirían separar la oferta de los contratos, pero todavía no se ha demostrado que necesiten modelos independientes.
- **Tres contextos (Catálogo / Membresías / Beneficios):** añadirían fronteras y coordinación sin evidencia suficiente que lo justifique.

## Consecuencias

- El Context Map representará **un único BC central** con tres capacidades internas.
- El repositorio tendrá **una carpeta de Bounded Context**, no tres contextos separados.
- Las capacidades podrán organizarse en módulos internos cuando corresponda; esta decisión **no define aún clases, aggregates ni servicios**.

## Hotspots y revisión

La decisión se revisará si la validación con el experto demuestra autonomía real de reglas, lenguaje o responsabilidades, especialmente en:

- **H-03:** efecto de modificar planes sobre membresías ya contratadas.
- **H-06:** consumo y caducidad de horas acumuladas.
- **H-07:** titularidad y distribución de beneficios en planes de equipo.

**Referencia de respaldo:** análisis estratégico de Nodo, apartado 3. La clasificación del Core y las relaciones con otros contextos se documentan en ADR independientes.
