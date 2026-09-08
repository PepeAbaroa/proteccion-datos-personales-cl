# Criterios de construcción — RAT, EIPD/PIA y MPI

> **Jerarquía**: el contenido MÍNIMO obligatorio de cada instrumento lo fija la ley/reglamento (bloques
> `TEXTO LITERAL`, ya citados en `references/especifico/`, aquí solo se referencian). Lo complementario
> aporta metodología de llenado y justificación práctica — nunca agrega un campo obligatorio que la ley
> no exige, y se marca explícitamente cuando exige más que el mínimo legal.

## 1. RAT (Registro de Actividades de Tratamiento)

**Qué exige la ley (dos fuentes que se combinan, no una sola):**
- Deber de transparencia del **Art. 14 ter** (12 elementos que deben estar siempre públicos) — cita
  completa en `mapa-articulos-ley21719.md`.
- Caracterización de actividades de tratamiento del **Reglamento MPI Art. 3 letra d)** (11 sub-elementos
  romanos i-xi, exigible si se quiere certificar un MPI, pero es el estándar de facto de cualquier RAT
  serio aunque no se certifique) — cita completa en `mapa-articulos-reglamento-mpi.md`.

**Cómo llenar cada campo — justificación exigida, no solo el dato:**
| Campo (Reglamento Art. 3 letra d) | Qué preguntar para llenarlo | Dónde falla más seguido |
|---|---|---|
| i. Tipo de dato, ¿incluye sensibles? | Revisar contra Art. 2 letra g) — situación socioeconómica y salud SON sensibles aunque no lo parezcan en la práctica | Subclasificar como "dato común" un dato que la ley ya define como sensible |
| ii. Ámbito territorial | ¿El proveedor/servidor está fuera de Chile? Si sí, dispara Título V | Omitir el ámbito cuando el proveedor es cloud extranjero |
| vi. Fuente de los datos | ¿Es de acceso público (Art. 2 letra i)? Si sí, igual se somete a la ley | Asumir que "público" = "sin restricción" |
| vii. Base de licitud | ¿Cuál de las 5 del Art. 13, o el Art. 20 si es órgano público? | Poner "consentimiento" quando en realidad hay obligación legal (complica revocación futura) |
| viii-ix. Terceros y transferencias internacionales | ¿Hay cesión (Art. 15) o encargo (Art. 15 bis)? ¿Hay transferencia internacional (Art. 27)? | Confundir cesión con encargo — cambia el régimen de responsabilidad |
| x. Plazos de supresión | ¿Cuál es el plazo legal o el criterio de necesidad del Art. 3 letra c)? | Dejar el campo en blanco o "indefinido" sin base legal para conservación indeterminada |
| xi. Decisiones automatizadas | ¿Hay perfilamiento (Art. 8 bis)? Si sí, EIPD obligatoria (ver §2) | No detectar que un sistema de "alerta temprana" de deserción ES elaboración de perfiles |

> **COMPLEMENTARIO** (MOD01.03, `sources/complementario/mod01.03-gobernabilidad-accountability.pdf.extracto/chunk_006.md`)
> "El Registro de Actividades de Tratamiento (RAT) documenta todos los procesamientos de datos
> personales."

**Razonamiento aplicado:** el RAT no es un documento aislado — es, según la doctrina de accountability
(ver `privacy-by-design-accountability.md`), la pieza base de la que dependen las otras 4 (EIPD, políticas,
capacitación, gestión de brechas): sin RAT actualizado no se puede saber qué tratamientos requieren EIPD
(§2) ni qué política de transparencia publicar (Art. 14 ter).

## 2. EIPD / PIA (Evaluación de Impacto en Protección de Datos)

**Cuándo es obligatoria por ley — Art. 15 ter (4 supuestos, cita completa en `mapa-articulos-ley21719.md`):**
(a) evaluación sistemática/perfilamiento con efectos jurídicos significativos, (b) tratamiento masivo o a
gran escala, (c) monitoreo sistemático de zona de acceso público, (d) datos sensibles sin consentimiento.
**La Agencia debe publicar una lista orientativa y orientaciones mínimas de metodología — verificar
activamente si ya lo hizo antes de asumir que no existe.**

**Mientras la Agencia no publique su propia metodología**, esta skill usa como referencia de buena
práctica (NO como norma chilena) la estructura del template EDPB (autoridad europea, contexto GDPR):

> **COMPLEMENTARIO** (Template EDPB adoptado, `sources/complementario/dpia-template-referencia.pdf.extracto/chunk_002.md`)
> Estructura: "0 Overview of the processing (responsable, encargado, nombre, planificación) → 1
> Systematic description of the processing (datos tratados, finalidades, usos secundarios, naturaleza/
> alcance/contexto, arquitectura técnica) → 2 Analysis of the processing (licitud, minimización, plazos
> de conservación, calidad del dato, medidas de cumplimiento, medidas de diseño por defecto, medidas de
> seguridad) → 3 Considerations on necessity and proportionality → 4 Risk assessment and management."

**Razonamiento aplicado — mapeo directo a la ley chilena:** la sección "0-1" del template EDPB es, en
sustancia, el mismo contenido que ya exige el RAT (Art. 14 ter + Reglamento Art. 3 letra d) — no hay que
duplicar trabajo, se reutiliza. La sección "2.1 Lawfulness" corresponde a verificar la base de licitud
(Arts. 12-13/20 de la ley chilena, no el Art. 5 GDPR que cita el template). La sección "3" (necesidad y
proporcionalidad) corresponde exactamente al **principio de proporcionalidad del Art. 3° letra c)** de la
ley chilena — mismo concepto, nombre distinto.

> **COMPLEMENTARIO** (Template EDPB, `sources/complementario/dpia-template-referencia.pdf.extracto/chunk_010.md`)
> "A threat is any circumstance or event with the potential to adversely impact data subject's rights and
> freedoms [...] A risk source is the origin or underlying cause from which a threat can materialise
> [...] Impact is the consequences that can be expected from the threat materialisation."

**Razonamiento aplicado — cómo justificar el análisis de riesgo, no solo llenarlo:** tres preguntas
separadas y en ese orden — (1) ¿qué podría salir mal aunque el sistema funcione exactamente como está
diseñado? (amenaza estructural, no solo falla técnica), (2) ¿de dónde viene ese riesgo (diseño, tipo de
dato, plazo de conservación)?, (3) ¿qué le pasaría concretamente al titular si se materializa? Aplicado a
un SLEP: un sistema de "alerta de riesgo de deserción" bien construido y sin fallas igual genera riesgo
estructural de estigmatización de un alumno — eso se documenta en la EIPD aunque el sistema "funcione
perfecto".

**Advertencia de uso:** este template es europeo (GDPR), útil como metodología de buena práctica mientras
Chile no publique la suya, pero **nunca se cita como si fuera la norma chilena** — cualquier EIPD real
para un SLEP debe fundarse en el Art. 15 ter y adaptarse a la terminología y bases de licitud de la ley
19.628 modificada, no copiar artículos GDPR.

## 3. Matriz de riesgo de infracción (Reglamento MPI Art. 3 letra e)

> **TEXTO LITERAL** (Reglamento Art. 3 letra e, cita completa en `mapa-articulos-reglamento-mpi.md`)
> "La identificación de las actividades de tratamiento de datos o procesos de la entidad [...] en cuyo
> contexto se genere o incremente el riesgo de comisión de las infracciones señaladas en los artículos 34
> bis, 34 ter y 34 quáter de la ley Nº 19.628. A partir de las actividades o procesos de tratamiento
> identificadas, el responsable deberá determinar aquellas que presentan un mayor riesgo de incurrir en
> infracciones, incorporándolas en la respectiva matriz de riesgos. Dicha matriz deberá desarrollarse
> considerando la graduación de las sanciones previstas en la ley."

**Razonamiento aplicado:** la ley exige la matriz y exige que refleje la graduación de sanciones
(leve/grave/gravísima, Arts. 34 bis-quáter) — pero no da la fórmula de cálculo. Aquí es donde el
complementario aporta el método, no el criterio legal de qué calificar como riesgo (eso ya lo fija el
Art. 34).

> **COMPLEMENTARIO** (Template EDPB, `sources/complementario/dpia-template-referencia.pdf.extracto/chunk_012.md` y `chunk_013.md`)
> "Risk level calculation usually follows the standard Risk = likelihood × severity, typically using
> qualitative scales to derive a level (for example, low/medium/high). [...] Identify risk modulating
> factors, characteristics that increase or decrease the likelihood or severity of a risk [...] Examples
> of aggravating (upward-modulating) factors are a very large number of data subjects or high data
> sensitivity, data subjects in a situation of dependency or vulnerability (children, patients, workers,
> migrants) [...] A risk in data protection may be deemed non-acceptable if the potential severity of its
> impact is very high, even when its likelihood of occurring is low [...] Residual risk is the risk that
> still remains after the controller has [...] added additional mitigating measures."

**Razonamiento aplicado — método de construcción de la matriz, mapeado a la ley chilena:**
1. **Listar actividades de tratamiento** (vienen del RAT de §1) que puedan calzar en alguna letra de los
   Arts. 34 bis/ter/quáter.
2. **Para cada una, estimar riesgo = probabilidad × severidad** — la severidad NO se inventa: se deriva
   directamente de en cuál de los 3 artículos calzaría si se materializa (34 bis = severidad baja, 34 ter
   = media, 34 quáter = alta) — esto es lo que exige literalmente "considerando la graduación de las
   sanciones" del Reglamento.
3. **Aplicar factores agravantes específicos de un SLEP** (ya validados como factor real, no genérico):
   alto volumen de titulares (toda la matrícula), datos sensibles (PIE/salud/IVE), titulares en situación
   de vulnerabilidad (**niños, niñas y adolescentes** — coincide exactamente con el criterio agravante N°5
   del Art. 37 de la ley: "Si el tratamiento realizado incluye datos personales sensibles o [...] de
   niños, niñas y adolescentes").
4. **Un riesgo de severidad muy alta no se acepta aunque su probabilidad sea baja** — regla explícita del
   complementario, coherente con que la ley clasifica ciertas conductas como gravísimas (Art. 34 quáter)
   independientemente de cuán infrecuentes sean.
5. **Distinguir riesgo inherente (antes de medidas) vs. residual (después de aplicar protocolos del Art.
   3 letra f del Reglamento)** — la matriz debe mostrar ambos, no solo el final, para que se entienda qué
   trabajo de mitigación se hizo.

## 4. MPI (Modelo de Prevención de Infracciones)

**Checklist legal completo ya está en `mapa-articulos-reglamento-mpi.md` (Art. 3, letras a-j)** — no se
repite aquí. Resumen de las piezas que dependen de lo ya construido en §1-3:
- Letra d) del Art. 3 Reglamento = el RAT de §1.
- Letra e) del Art. 3 Reglamento (matriz de riesgos de infracción) = es directamente la matriz de §3,
  nutrida además por las EIPD de §2 (los tratamientos de alto riesgo del Art. 15 ter suelen coincidir con
  los de mayor riesgo de infracción).
- Letra b)-c) (delegado y sus medios) = ver `aplicacion-sector-publico-slep.md` para el caso SLEP
  (funcionario de dotación vigente, nunca externo).

> **COMPLEMENTARIO** (MOD01.03, accountability, ver `privacy-by-design-accountability.md` §2)
> Los 5 componentes de accountability (RAT, EIPD, capacitación, políticas, gestión de brechas) son,
> tomados en conjunto, funcionalmente equivalentes al contenido mínimo del programa de cumplimiento del
> Art. 3 del Reglamento MPI — construir accountability de facto según la doctrina complementaria deja a
> una institución a un paso de poder certificar un MPI formal si decide hacerlo.

**Razonamiento aplicado — justificación de por qué construir esto aunque no se certifique:** aunque el
MPI sea voluntario (Art. 49, ya establecido en `mapa-articulos-ley21719.md`), los mismos 5 instrumentos
sirven como evidencia de diligencia debida (Art. 36 N°5, atenuante) incluso sin certificación formal — no
se pierde el trabajo si finalmente no se certifica.

## Grafo
Depende de `mapa-articulos-ley21719.md` (Arts. 3, 14 ter, 15 ter, 34 bis-quáter, 36, 49-51),
`mapa-articulos-reglamento-mpi.md` (Art. 3, Arts. 6-13) y `privacy-by-design-accountability.md`. Se
entrega a `compliance-cl` como insumo de construcción de documentos, no lo reemplaza.
