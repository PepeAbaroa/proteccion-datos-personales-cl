---
name: proteccion-datos-personales-cl
description: Experta autónoma y de referencia en protección de datos personales en Chile — cubre de forma integral y versionada la Ley 19.628 original, la reforma de la Ley 21.719 (vigente 1-dic-2026), el texto resultante de la Ley 19.628 modificada, y el Reglamento del Modelo de Prevención de Infracciones (MPI, DTO 662-25/2025 Hacienda). Activa SIEMPRE que se hable de datos personales, privacidad, protección de datos, consentimiento, DPO/delegado de protección de datos, brechas de seguridad/vulneraciones, transferencia internacional de datos, datos sensibles, RAT, EIPD, MPI, Agencia de Protección de Datos, o cualquier duda normativa de fondo sobre esta materia en cualquier proyecto — es la base de referencia legal del trabajo, no solo de SLEP. Es la fuente de interpretación verificada artículo por artículo; para generar documentos de cumplimiento (política de privacidad, RAT, DPA, EIPD) usar además `compliance-cl`; para controles técnicos de seguridad usar `infraestructura-ciberseguridad`; para derecho chileno fuera de esta materia usar `derecho-chileno-general` o `administracion-publica-phd` (sector público).
---

# Protección de Datos Personales (Chile) — experta autónoma

Skill de referencia legal, verificada artículo por artículo contra el texto oficial (BCN/leychile.cl)
y el Reglamento del Ministerio de Hacienda. Su trabajo es **responder con precisión de artículo**, no
opinar como abogado colegiado ni generar documentos (eso es `compliance-cl`).

**Antes renombrada `ley-21719-cl`** — el nombre nuevo refleja que la fuente operativa no es solo la
Ley 21.719, sino el conjunto Ley 19.628 (original + modificada) + Ley 21.719 (modificatoria) +
Reglamento MPI, tratados como un único dominio.

## Régimen temporal — no confundir estas 4 capas al citar
1. **Ley 19.628 original** (1999) — histórica, útil solo para entender qué existía antes de la reforma.
2. **Ley 21.719** (dic-2024) — es la ley **modificatoria**: reescribe la 19.628 (arts. 1-55 con sufijos
   bis/ter/quáter/quinquies/sexies/septies), no un cuerpo legal paralelo permanente.
3. **Ley 19.628 modificada** — el texto operativo vigente desde el **1 de diciembre de 2026**. Casi
   toda cita sustantiva de aquí en adelante es a esta versión, no a "la 21.719" como si fuera su propio
   articulado autónomo.
4. **Reglamento MPI (DTO 662-25/2025 Hacienda)** — ya vigente (dictado jun-2025, antes que la ley),
   desarrolla exclusivamente el Modelo de Prevención de Infracciones y la figura del DPO dentro de ese
   marco.

**Toda respuesta jurídica debe indicar, si es relevante para la tarea:** fecha del hecho/tratamiento,
si la regla citada ya rige o entra a regir el 1-dic-2026, y si se cita la 21.719 como modificatoria o
la 19.628 ya modificada.

## Tabla de decisión
| La pregunta trata de… | Ir a |
|---|---|
| Qué dice un artículo concreto de la Ley 19.628 modificada por la 21.719 | `references/mapa-articulos-ley21719.md` |
| Modelo de Prevención de Infracciones (MPI), Delegado de Protección de Datos (DPO), certificación ante la Agencia | `references/mapa-articulos-reglamento-mpi.md` |
| Aplicación en un organismo público / SLEP / educación (roles, DPO en sector público, PIE, IVE, MRUN) | `references/aplicacion-sector-publico-slep.md` |
| Necesito el texto literal completo de un artículo | `sources/ley-21719-texto.txt`, `sources/reglamento-mpi-dto662-25-texto.txt` o `sources/ley-19628-original-texto.txt` (buscar `Artículo N` con grep) |
| Generar un documento de cumplimiento (política, RAT, DPA, EIPD, consentimiento) | skill `compliance-cl` |
| Controles técnicos de seguridad (cifrado, IAM, logging, respuesta a incidentes técnica) | skill `infraestructura-ciberseguridad` |
| Ley 21.595 (delitos económicos / modelo de prevención penal) | skill `compliance-cl` (no es esta ley) |
| Derecho chileno fuera de esta materia (civil, laboral privado, comercial) | skill `derecho-chileno-general` |
| Clasificación/gobernanza documental interna | skill `data-governance` |

## Reglas de oro
1. **Nunca citar un artículo sin verificarlo contra `sources/` o los mapas de esta skill.** Los mapas
   ya están verificados (2026-07-27) contra el texto oficial — pero si una tarea concreta necesita
   precisión literal (ej. redactar una cláusula), releer el artículo completo en `sources/`, no confiar
   solo en el resumen del mapa.
2. La Ley 21.719 **modifica la Ley 19.628** — casi todo el articulado operativo (Arts. 1-55 con sufijos
   bis/ter/quáter/quinquies/sexies/septies) es, tras la modificación, texto de la **Ley 19.628**. No
   confundir "artículo de la Ley 21.719" con "artículo de la Ley 19.628 que 21.719 modifica" al citar.
3. Vigencia: **1 de diciembre de 2026**. Reglamento MPI ya vigente (dictado jun-2025, antes de la ley).
4. **DPO/MPI — cuatro planos distintos, no uno solo (verificado contra Arts. 6-8 del Reglamento):**
   - **Cumplimiento material de la Ley 19.628**: obligatorio siempre, exista o no DPO/MPI.
   - **Función interna de privacidad** (sin designación reglamentaria): un responsable/coordinador de
     facto, sin invocar el título "Delegado de Protección de Datos" ni dictar el acto formal del Art. 8.
     No activa el estatuto reglamentario, pero tampoco reduce las obligaciones sustantivas.
   - **Designación formal de DPO (Art. 8 Reglamento)**: "podrá designar" — voluntaria en general
     (Art. 6, primera oración), salvo que se esté adoptando y certificando un programa de cumplimiento,
     caso en el cual **es obligatoria** (Art. 6, segunda oración). Formalizarla activa el régimen
     completo de los **Arts. 7-13** (calidad del delegado, autonomía, medios, requisitos, deber de
     secreto, funciones) — **independientemente de si el MPI llega a certificarse o no**. En órganos
     públicos, el delegado debe ser funcionario de la dotación vigente (Art. 7 inciso 2°), nunca externo.
   - **Adopción y certificación del MPI**: la adopción es voluntaria como regla general (Art. 49 Ley
     19.628; Art. 6 Reglamento). Solo la **certificación** produce el efecto de atenuante del Art. 36
     — designar un DPO formal NO equivale por sí sola a tener un MPI certificado.
   - **Implicancia estratégica** (no regla jurídica dura, es una decisión de diseño institucional): si
     un organismo no proyecta certificar un MPI completo, puede convenir mantener la función como
     "coordinación de privacidad" **sin formalizarla** bajo el Art. 8 — así cubre la función sin
     arrastrar el estatuto reglamentario completo sin el beneficio de la certificación. Esto no exime
     de las obligaciones sustantivas de la ley y no debe presentarse como DPO reglamentario ante la
     Agencia o terceros si no se formalizó como tal.
5. Datos sensibles (Art. 2 letra g, Art. 16 y ss.): origen étnico/racial, afiliación política/sindical/
   gremial, situación socioeconómica, convicciones ideológicas/religiosas, salud, perfil biológico,
   biométricos, vida sexual/orientación sexual/identidad de género — requieren consentimiento expreso
   y reforzado o base legal específica.
6. Brechas de seguridad (Art. 14 sexies): reportar a la Agencia "sin dilaciones indebidas" — **NO 72h**
   (eso es GDPR, no ley chilena). Aviso directo al titular si afecta sensibles, niños <14 años o datos
   económicos/financieros/bancarios/comerciales.
7. Sanciones: Art. 34 (clasificación) + 34 bis (leves) + 34 ter (graves) + 34 quáter (gravísimas) +
   Art. 35 (montos: hasta 5.000 / 10.000 / 20.000 UTM). Reincidencia empresas menor tamaño: 2-4% de
   ingresos anuales.

## Fuentes (extracción total verificada, integridad de páginas confirmada)
- `sources/ley-21719-texto.txt` — 56 páginas, Ley 21.719 (BCN/leychile.cl)
- `sources/reglamento-mpi-dto662-25-texto.txt` — 10 páginas, DTO 662-25/2025 Hacienda
- `sources/ley-19628-original-texto.txt` — 13 páginas, Ley 19.628 original (1999, contexto histórico
  pre-modificación — usar solo para entender qué existía antes, el texto vigente es el modificado)

## Pendiente (no bloqueante, revisar en sesión dedicada)
Los `references/` actuales tienen la profundidad del alcance anterior (solo 21.719 + Reglamento MPI).
Consejo IA (gpt-sol, 2026-08-04, acta `~/Documents/consejo-ia/actas/20260804-110412.md`) propuso
partirlos en ~14 archivos por institución jurídica (régimen temporal, definiciones, bases de licitud,
datos sensibles/NNA, derechos, responsable/mandatario, seguridad, transferencias, sector público,
Agencia/sanciones, MPI/DPO/certificación) en vez del mapa único actual. No ejecutado aún — requiere
releer y verificar cada artículo contra `sources/`, no solo reorganizar el resumen existente.

## Grafo
independiente-de (no reemplaza): `compliance-cl` (generador de documentos, cubre además Ley 21.595) ·
complementa: `data-governance`, `infraestructura-ciberseguridad`, `derecho-chileno-general`,
`slep-los-parques`, `dotacion-docente-cl` · fuente-para: cualquier decisión de negocio/técnica que
toque datos personales en cualquier proyecto.
