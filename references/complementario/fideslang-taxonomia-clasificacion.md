# Fideslang — taxonomía de clasificación de datos (complementaria al RAT)

> Verificado contra `sources/complementario/fideslang-docs-selectas.txt` (README oficial
> IABTechLab/fideslang + docs de fidesops, 2026-09-08). Fideslang es vocabulario/herramienta de
> clasificación, **no ley** — se usa para poblar el "qué es este dato" y "para qué se usa" del RAT
> (ver `criterios-rat-eipd-mpi.md` §1), nunca para decidir base de licitud, que sigue las reglas de
> `mapa-articulos-ley21719.md`.

## Qué es y para qué sirve aquí

Fideslang es una taxonomía open source (CC BY 4.0) para etiquetar de forma estandarizada qué dato procesa
un sistema, para qué se usa y de quién es. No es una norma chilena ni un estándar ISO — es un vocabulario
de ingeniería de privacidad, útil para que el llenado del RAT (Art. 14 ter + Reglamento Art. 3 letra d)
no dependa de categorías ad-hoc inventadas cada vez.

## Las 3 categorías vigentes (no 4 — ver advertencia de versión abajo)

> **COMPLEMENTARIO** (`fideslang-docs-selectas.txt`, README IABTechLab/fideslang)
> "The taxonomy is currently comprised of three classification groups that are used together to easily
> describe the data types and associated processing behaviors of an entire tech stack."

**1. Data Categories** — qué tipo de dato es.

> **COMPLEMENTARIO** — "Data Categories are labels used to describe the type of data processed by a
> system. […] Data Categories are hierarchical with natural inheritance, meaning you can classify data
> coarsely with a high-level category (e.g. `user.contact` data), or you can classify it with greater
> precision using subclasses (e.g. `user.contact.email` data)."

**Razonamiento aplicado:** la jerarquía con herencia es lo que la hace útil para un RAT real — un mismo
campo de base de datos puede etiquetarse solo como `user.contact` si no se necesita precisión, o bajar a
`user.contact.email` cuando el análisis de riesgo lo exige (ej. distinguir email de teléfono para efectos
de qué canal de notificación de brecha usar, Art. 14 sexies).

**2. Data Use Categories** — para qué se usa el dato.

> **COMPLEMENTARIO** — "Data Use Categories are labels that describe how, or for what purpose(s) a
> component of your system is using data. […] you can easily describe what you're using data for either
> coarsely (e.g. `provide.service.operations`) or with more precision using subclasses (e.g.
> `provide.service.operations.support.optimization`)."

**Razonamiento aplicado:** este campo mapea directo a la **finalidad** que exige declarar el Art. 14 ter
letra c) (finalidades del tratamiento) — la jerarquía evita que dos áreas de una misma institución
describan la misma finalidad con palabras distintas en el RAT, lo que en una auditoría real es la falla
más común de trazabilidad.

**3. Data Subject Categories** — de quién es el dato.

> **COMPLEMENTARIO** — "\"Data Subject\" is a label commonly used in the regulatory world to describe
> the users of a system whose data is being processed. […] Examples of a Data Subject are:
> `anonymous_user`, `employee`, `customer`, `patient`, `next_of_kin`."

**Razonamiento aplicado:** en un SLEP/establecimiento, esta categoría es la que obliga a distinguir
explícitamente **estudiante** (posible NNA, Art. 16 quáter), **apoderado/next_of_kin**, **docente/
funcionario (employee)** — cada uno activa reglas distintas (consentimiento de NNA, base de licitud
laboral vs. educativa). Etiquetar todo como "usuario genérico" es exactamente el error que esta categoría
existe para evitar.

## Advertencia de versión — Data Qualifiers ya NO existen

> **COMPLEMENTARIO** (`fideslang-docs-selectas.txt`, release notes IABTechLab/fideslang PR #186)
> "Fideslang 3.0 removed data qualifier and registry concepts, as well as deprecated attributes on Data
> Use, System, and Dataset." (cambio de diciembre de 2023).

**Razonamiento aplicado:** documentación o formación antigua sobre Fideslang puede mencionar un cuarto
grupo, "Data Qualifiers" (nivel de identificabilidad: identificado/pseudonimizado/anonimizado) — está
**eliminado desde la versión 3.0**. No usarlo como si fuera vigente. El concepto de "nivel de
identificabilidad" que cubría sigue siendo relevante para el RAT chileno (distinguir dato identificado de
pseudonimizado es clave para varias obligaciones), pero hoy hay que resolverlo con razonamiento propio
apoyado en la ley (Art. 2 letra f) y g)), no citando una categoría de Fideslang que ya no existe.

## Cómo se usa junto con el RAT (`criterios-rat-eipd-mpi.md` §1)

| Campo del RAT (Reglamento Art. 3 letra d) | Categoría Fideslang que ayuda a poblarlo |
|---|---|
| i. Tipo de dato, ¿incluye sensibles? | Data Category (ej. `user.health`, `user.financial` — la jerarquía obliga a bajar de nivel hasta ver si cae en una subcategoría sensible) |
| vii. Base de licitud / finalidad | Data Use Category (`provide.service...`) — describe la finalidad de forma consistente entre RAT de distintas áreas |
| — (no es campo explícito del Art. 3 letra d, pero determina el resto) | Data Subject Category — distingue estudiante/NNA de funcionario/apoderado antes de aplicar cualquier regla |

**Razonamiento aplicado — límite de uso:** Fideslang clasifica; **no decide** si el tratamiento es lícito
ni qué medida de seguridad aplicar — eso lo resuelve esta skill (base de licitud) y `04-tyb-db-architect`
(implementación técnica de la protección, ver `references/especifico/anonimizacion-enmascaramiento-tecnicas.md`
en esa skill para las técnicas concretas de enmascaramiento/pseudonimización sobre un dato ya clasificado
aquí).

## Grafo
Complementa `criterios-rat-eipd-mpi.md` §1 (RAT) — aporta vocabulario de clasificación, no reemplaza los
campos legales exigidos. Deriva a `04-tyb-db-architect` (`anonimizacion-enmascaramiento-tecnicas.md`) para
la implementación técnica de protección sobre un dato ya clasificado con esta taxonomía.
