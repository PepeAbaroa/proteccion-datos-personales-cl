---
name: proteccion-datos-personales-cl
description: Experta autónoma y de referencia en protección de datos personales en Chile — cubre de forma integral y versionada la Ley 19.628 original, la reforma de la Ley 21.719 (vigente 1-dic-2026), el texto resultante de la Ley 19.628 modificada, y el Reglamento del Modelo de Prevención de Infracciones (MPI, DTO 662-25/2025 Hacienda). Activa SIEMPRE que se hable de datos personales, privacidad, protección de datos, consentimiento, DPO/delegado de protección de datos, brechas de seguridad/vulneraciones, transferencia internacional de datos, datos sensibles, RAT, EIPD, MPI, Agencia de Protección de Datos, o cualquier duda normativa de fondo sobre esta materia en cualquier proyecto — es la base de referencia legal del trabajo, no solo de SLEP. Es la fuente de interpretación verificada artículo por artículo. Genera además documentos de cumplimiento (política de privacidad, RAT, DPA, EIPD, consentimiento) vía `plantillas/`. **NO activa para** controles técnicos de seguridad — usar `infraestructura-ciberseguridad`; **NO activa para** derecho chileno fuera de esta materia — usar `administracion-publica-phd` (sector público).
---

# Protección de Datos Personales (Chile) — experta autónoma

Skill de referencia legal, verificada artículo por artículo contra el texto oficial (BCN/leychile.cl)
y el Reglamento del Ministerio de Hacienda. Su trabajo es **responder con precisión de artículo**, no
opinar como abogado colegiado — para generar el documento a partir de la cita verificada, ver
`plantillas/ley-21719/` (heredado de `compliance-cl`, repo de terceros retirado 2026-09-08).

**Antes renombrada `ley-21719-cl`** — el nombre nuevo refleja que la fuente operativa no es solo la
Ley 21.719, sino el conjunto Ley 19.628 (original + modificada) + Ley 21.719 (modificatoria) +
Reglamento MPI, tratados como un único dominio.

## Metodología de razonamiento (cómo pensar esta materia, no solo dónde buscarla)

Esta skill no es un índice — puede resolver sola la mayoría de las consultas siguiendo estos 8 pasos, y
solo necesita abrir `references/especifico/` cuando el paso exige precisión literal de artículo:

1. **Fijar el hecho concreto**: qué dato, de quién (titular), tratado por quién (responsable/encargado —
   Art. 2 letras n/x), cuándo. Sin esto, cualquier análisis posterior es especulativo.
2. **Fijar el régimen temporal**: ¿el hecho ocurre antes o después del 1-dic-2026? ¿corresponde citar la
   21.719 como modificatoria histórica o la 19.628 ya modificada (texto operativo)? El Reglamento MPI ya
   rige desde jun-2025, independiente de la fecha de vigencia de la ley.
3. **Clasificar el dato**: ¿es dato personal (Art. 2 f)? ¿es sensible (Art. 2 g — incluye situación
   socioeconómica y salud, categorías que la práctica suele subestimar)? ¿es de niño/niña (<14) o
   adolescente (14-17, Art. 16 quáter)?
4. **Determinar la base de licitud**: privados → Arts. 12-13 (consentimiento u otras 5 fuentes); órganos
   públicos → Art. 20 (función legal, sin consentimiento). Nunca asumir "consentimiento" por defecto si
   en realidad hay obligación legal — complica innecesariamente la revocación futura.
5. **Verificar las obligaciones del responsable activadas por el caso**: transparencia (14 ter), diseño y
   seguridad (14 quáter-quinquies), y si el tratamiento califica en alguno de los 4 supuestos del Art. 15
   ter → EIPD obligatoria, no opcional.
6. **Si hay un tercero involucrado**: distinguir cesión (Art. 15, el tercero se vuelve responsable propio)
   de encargo/mandatario (Art. 15 bis, DPA, el tercero actúa por instrucción) de transferencia
   internacional (Arts. 27-29, si el tercero está fuera de Chile — requiere base de transferencia propia,
   no basta la base de licitud del tratamiento original).
7. **Si hay un incidente**: calificar si es brecha reportable (Art. 14 sexies — "sin dilaciones
   indebidas", nunca "72 horas") y si dispara aviso directo al titular (sensibles, NNA <14, o datos
   económico/financiero/bancario/comercial).
8. **Si hay que calificar gravedad/sanción**: ubicar en Art. 34 bis (leve) / ter (grave) / quáter
   (gravísima — verificar si hay dolo: "a sabiendas", "maliciosamente", "fraudulenta", que escala grave→
   gravísima) y aplicar el régimen de sanción correcto: Art. 35 (privados, UTM) o Art. 44 (jefe superior
   de órgano público, % de su remuneración — nunca UTM institucional).

9. **Enriquecer con complementario SOLO después de resolver 1-8 con la ley**: si la tarea pide framework
   de implementación, cómo armar un RAT/EIPD/MPI, o cruzar con un estándar internacional (ISO 27701,
   29100, 27001; NIST Privacy Framework/AI RMF), abrir `references/complementario/` — pero la respuesta
   nombra primero qué exige la ley/reglamento y solo después, marcado explícitamente como
   "complementariamente, según [estándar]...", lo que ese estándar aporta. **Nunca al revés, nunca
   mezclado sin decir cuál es cuál, nunca un estándar contradice o reemplaza la ley.**

**Regla de cierre en toda respuesta sustantiva**: citar el artículo exacto, indicar la fecha del hecho y
si la norma citada ya rige o entra a regir el 1-dic-2026, y verificar la cita literal contra
`sources/especifico/` antes de un uso de alto riesgo (redactar cláusula, fundar sanción, responder a la
Agencia) — los `references/especifico/` son síntesis con cita verificada, no sustituto del texto cuando
la precisión literal importa. La ley y el reglamento **mandan**; lo complementario **enriquece y cruza**,
nunca decide por sí solo.

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

## Tabla de decisión — cuándo abrir un archivo en vez de razonar con la metodología de arriba
| La pregunta trata de… | Ir a |
|---|---|
| Qué dice un artículo concreto de la Ley 19.628 modificada por la 21.719 (texto literal + razonamiento aplicado, artículo por artículo, Títulos I-VIII completos) | `references/especifico/mapa-articulos-ley21719.md` |
| Modelo de Prevención de Infracciones (MPI), Delegado de Protección de Datos (DPO), certificación ante la Agencia | `references/especifico/mapa-articulos-reglamento-mpi.md` |
| Aplicación en un organismo público / SLEP / educación (roles, DPO en sector público, PIE, IVE, MRUN) | `references/especifico/aplicacion-sector-publico-slep.md` |
| Necesito releer el texto legal íntegro sin el filtro de esta skill | `sources/especifico/ley-21719-texto.txt`, `sources/especifico/reglamento-mpi-dto662-25-texto.txt` o `sources/especifico/ley-19628-original-texto.txt` (grep `Artículo N`) |
| Privacidad desde el diseño (Art. 14 quáter) o accountability/responsabilidad (Art. 3 letra e) cruzados con NIST/ISO/doctrina | `references/complementario/privacy-by-design-accountability.md` |
| Criterios para armar/justificar un RAT, una EIPD/PIA o un MPI — qué debe contener cada uno, cómo llenarlo | `references/complementario/criterios-rat-eipd-mpi.md` |
| Otro cruce con doctrina/estándares (Diplomado U. Chile, ISO 27001/27701/29100, NIST Privacy Framework/AI RMF) no cubierto en los dos archivos de arriba | `sources/complementario/*.pdf.extracto/INDICE.md` (cargar el índice del documento relevante, nunca todo el corpus) |
| Generar un documento de cumplimiento (política, RAT, DPA, EIPD, consentimiento) | `plantillas/ley-21719/templates/` — usar la cita de artículo ya verificada arriba, no reinterpretar la ley al redactar |
| Controles técnicos de seguridad (cifrado, IAM, logging, respuesta a incidentes técnica) | skill `infraestructura-ciberseguridad` — esta skill le da el artículo que exige el control (ej. Art. 14 quinquies), esa skill traduce a control técnico concreto |
| Ley 21.595 (delitos económicos / modelo de prevención penal) | skill `gobierno-corporativo-compliance-cl` (no es esta ley) |
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

## Fuentes — capa específica (íntegras, integridad de páginas verificada; PDF original + .txt extraído)
- `sources/especifico/ley-21719.pdf` (+ `-texto.txt`) — 56 páginas, Ley 21.719 (BCN/leychile.cl)
- `sources/especifico/reglamento-mpi-dto662-25.pdf` (+ `-texto.txt`) — 10 páginas, DTO 662-25/2025 Hacienda
- `sources/especifico/ley-19628-original.pdf` (+ `-texto.txt`) — 13 páginas, Ley 19.628 original (1999,
  contexto histórico pre-modificación; el Título III sigue siendo parte del texto vigente, ver
  `mapa-articulos-ley21719.md`)
- `sources/especifico/clausulas-modelo-transferencia-economia.pdf` (+ `.extracto/`) — 3 páginas,
  Resolución RAEX202503748 (Diario Oficial 19-dic-2025, Ministerio de Economía) — cláusulas contractuales
  modelo de transferencia internacional, vigencia **transitoria** hasta que la Agencia dicte su propia
  norma (Art. 28 inciso 2°). Ver `references/especifico/clausulas-modelo-transferencia-internacional.md`.

## Fuentes — capa complementaria (poblada 2026-09-08, íntegra y chunkeada — 15 documentos)
`sources/complementario/` — cada PDF extraído completo con `doc_full_extract.py` (INDICE.md + chunks,
integridad verificada, nada resumido):
- Doctrina Diplomado U. Chile: `mod01.01-gobierno-corporativo-proteccion-datos`,
  `mod01.03-gobernabilidad-accountability`, `mod01.04-cultura-organizacional-etica`,
  `libro-informes-comision-asesora-datos`, `el-rol-del-dpo`, `libro-blanco-del-dpo`,
  `data-privacy-principios`, `dpia-template-referencia` (template EDPB, agregado 2026-09-08 al detectar
  el hueco para §2 de `criterios-rat-eipd-mpi.md` — no estaba en la lista original propuesta).
- Estándares ya adquiridos por Pepe: `nist-privacy-framework-1.1`, `iso-iec-29100-2024`,
  `iso-iec-27701-2025`, `iso-27001-2022-es`.
- Descargado esta sesión (gratuito, oficial): `nist-ai-rmf-100-1` (nist.gov).
- Privacidad + IA: `intersection-privacy-ai-governance`, `managing-data-privacy-risk-advanced-analytics`.
- Propios, ya en `.md` sin extracción: `crosswalk-ley21663-ciberseguridad.md`, `crosswalk-iso27001-27701.md`.

`references/complementario/` — 2 archivos de cruce ya construidos (ver tabla de decisión arriba); el
resto del corpus complementario se consulta bajo demanda vía `INDICE.md` de cada `.extracto/`, no se
sintetiza todo por adelantado.

**ISO adicionales pedidas por Pepe (27018, 27023, 42001, 23894, 5259, 23053) — NO descargables:** son
normas de pago (ISO.org/AENOR/ANSI, ~USD 100-250 c/u), no hay copia gratuita oficial y no se buscan
copias pirata. Confirmado por WebSearch sus títulos vigentes (27018 PII en nube pública, 27023 mapeo
27001/27002 — bajo valor práctico, 42001 gestión de IA, 23894 gestión de riesgo de IA, 23053 marco de
sistemas de IA/ML, 5259 calidad de datos para IA/ML — pendiente verificar detalle si se compra). El NIST
AI RMF ya descargado cubre gratis el mismo ángulo que la ISO 23894.

## Estado de reconstrucción (contrato v3, ARQUITECTURA.md §6.1.b)
`references/especifico/` fue reconstruido completo el 2026-09-07/08: los 3 archivos ahora tienen formato
dual `TEXTO LITERAL` (cita exacta) + `Razonamiento aplicado` (interpretación), artículo por artículo,
Títulos I-VIII de la Ley 21.719 (incluido Título III verificado contra la Ley 19.628 original) y los 20
artículos del Reglamento MPI completos — no quedan artículos pendientes de citar en esas dos leyes.
Pendiente futuro no bloqueante: si la Agencia dicta las instrucciones generales referidas en Arts. 10,
14 septies, 28 y 41-42, actualizar la cita correspondiente.

## Grafo — con qué otras skills se combina y cómo
- **Generación de documentos (`plantillas/`, heredado de repo de terceros retirado)**: esta skill resuelve QUÉ dice la ley
  con cita verificada, y sus `plantillas/` GENERAN el documento (RAT/política/DPA/EIPD) a partir de esa
  cita — el flujo correcto es siempre interpretar primero (secciones de arriba), generar después
  (`plantillas/`), nunca al revés.
- **`gobierno-corporativo-compliance-cl`** (independiente, dominio distinto): compliance penal/económico
  (Ley 21.595/20.393), no datos personales — derivar ahí si la consulta es sobre MPD, no MPI.
- **`infraestructura-ciberseguridad`** (complementa): esta skill identifica QUÉ obligación legal de
  seguridad aplica (ej. Art. 14 quinquies); esa skill traduce a control técnico concreto (cifrado, IAM).
- **`data-governance`** (complementa): esa skill resuelve confiabilidad/calidad del dato; esta resuelve
  si su tratamiento es lícito — un dato puede estar bien gobernado y aun así tratarse ilícitamente.
- **`slep-los-parques`, `dotacion-docente-cl`** (fuente-para): cualquier decisión de esos dominios que
  toque datos personales (PIE, licencias médicas, IVE, MRUN) debe resolver primero aquí la base legal
  antes de decidir la acción operativa.
