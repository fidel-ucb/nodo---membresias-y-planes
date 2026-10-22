# ADR 0001 · Delimitación de un único Bounded Context

## Contexto

Se evaluaron límites dentro del subdominio Membresías y Planes con señales de lenguaje, reglas, actores, EventStorming y Domain Storytelling (análisis estratégico, §3, pp. 11–18; criterio de nivel Alto, p. 1).

## Decisión

Mantener provisionalmente un único BC `Membresías y Planes`, con Catálogo de Planes, Gestión de Membresías y Administración de Beneficios como capacidades internas. Corresponde a DD-02 y DD-03.

## Evidencia

Oferta, condiciones contratadas y derechos mantienen relaciones de dominio; no se demostró independencia suficiente de lenguaje, reglas, actores o evolución. Fronteras externas de reservas, cobros y acceso están mejor respaldadas. Figuras 2–8, escenarios DS y preguntas H-03/H-06/H-07 complementan la evidencia.

## Alternativas descartadas

- Dos BC: Catálogo de Planes y Gestión de Membresías. No se adopta por falta de evidencia de autonomía; H-03 puede hacer revisar esta alternativa.
- Tres BC: Catálogo, Membresías y Beneficios. No se adopta porque añadiría límites a procesos relacionados sin prueba de modelos independientes.

## Consecuencias

Las tres capacidades se documentan bajo una frontera única; no se crearán carpetas raíz separadas. Reexaminar si las respuestas a hotspots muestran reglas, vocabulario o responsabilidades que evolucionan independientemente.

## Estado

Aceptada provisionalmente hasta Sesión 3; DD-02 y DD-03 son hipótesis explícitas, sujetas a nueva evidencia.

## Hotspots

H-03 (cambio de plan con contratos vigentes), H-06 (caducidad), H-07 (equipo), además de escenarios de [07-bounded-context.md](../docs/07-bounded-context.md).
