# Aplicación al sector público — SLEP y organismos educativos

> Ángulo específico para servicios públicos (SLEP, DEM/DAEM, DEP). El régimen aplicable de tratamiento de
> datos por órganos públicos es el **Título IV de la Ley 19.628 modificada (Arts. 20-26)**, no el régimen
> general de privados (Título II) — texto completo de cada artículo en `mapa-articulos-ley21719.md` y
> `mapa-articulos-reglamento-mpi.md`; este archivo cruza ambos con el ángulo SLEP y cita solo el fragmento
> puntual que sostiene cada afirmación (formato dual TEXTO LITERAL + Razonamiento aplicado igual que los
> otros dos archivos de esta carpeta).

## Responsabilidad diferenciada frente a un privado

### Art. 44 — responsabilidad del jefe superior del órgano
> **TEXTO LITERAL** (Art. 44 Ley 19.628 modificada, sources/especifico/ley-21719-texto.txt línea 3052)
> "serán sancionadas con multa de veinte por ciento a cincuenta por ciento de la remuneración mensual del
> jefe superior del órgano público infractor [...] Tratándose de datos personales sensibles, la multa
> será del cincuenta por ciento de la remuneración mensual del jefe superior [...]"

**Razonamiento aplicado:** en un SLEP la responsabilidad administrativa recae personalmente sobre la
**Dirección Ejecutiva** — no es una multa institucional al presupuesto, es un descuento porcentual de la
remuneración del jefe de servicio. Cita completa y análisis en `mapa-articulos-ley21719.md` (Art. 44).

### Art. 45 — responsabilidad del funcionario infractor
> **TEXTO LITERAL** (Art. 45, línea 3111) "esta conducta se considerará una contravención grave a la
> probidad administrativa" (cuando el funcionario incurre en infracción gravísima)

**Razonamiento aplicado:** responsabilidad individual del funcionario que ejecutó la infracción,
acumulativa (no sustitutiva) a la del jefe superior — un mismo hecho puede escalar hasta sumario
administrativo del funcionario Y sanción a la Dirección Ejecutiva. Cita completa en
`mapa-articulos-ley21719.md` (Art. 45).

### Art. 46 — deber de reserva de los funcionarios
> **TEXTO LITERAL** (Art. 46, línea 3120) "deben guardar secreto o confidencialidad respecto de la
> información que tomen conocimiento en el ejercicio de sus cargos [...] se estimará que los hechos [...]
> vulneran gravemente el principio de probidad administrativa"

**Razonamiento aplicado:** el deber de reserva de cada funcionario que trata datos (no solo del DPO) está
conectado por ley al régimen general de probidad — su infracción no es solo un problema de datos
personales, activa además el Estatuto Administrativo.

### Art. 25 — datos de infracciones penales, civiles, administrativas y disciplinarias
> **TEXTO LITERAL** (Art. 25, línea 1747) "permanecerán accesibles al público por el período de cinco
> años" (infracciones civiles, administrativas y disciplinarias) — "Se prohíbe el tratamiento masivo de
> los datos personales contenidos en los registros electrónicos de infracciones [...] El incumplimiento
> [...] constituye una infracción gravísima" (línea 1749-1754)

**Razonamiento aplicado:** aplica directamente a sumarios administrativos y licencias médicas con causa
disciplinaria del personal SLEP — plazo de publicidad de 5 años y prohibición expresa de cruzar
masivamente esos registros (ej. para un "scoring de riesgo de personal") sin autorización legal
específica, bajo pena de infracción gravísima.

### Coexistencia con la Ley 20.285 (transparencia)
La Ley 21.719 no deroga ni reemplaza la Ley 20.285 — un dato puede ser público para efectos de
transparencia activa/pasiva y **simultáneamente** estar protegido como dato personal; no son regímenes
mutuamente excluyentes. El Art. 22 inciso 4° de la Ley 19.628 modificada ya exige expresamente
consentimiento del titular para responder una solicitud de transparencia que implique datos personales,
salvo el caso ya resuelto en el Art. 20 de la Ley 20.285 — se pide la base de licitud correcta en cada
caso, no se resuelve por defecto a favor de uno u otro régimen.

## DPO en el sector público — precisión importante

### Reglamento MPI Art. 7 inciso 2°
> **TEXTO LITERAL** "Los órganos públicos que establezcan un encargado de prevención o delegado de
> protección de datos personales deberán designar para ello a un funcionario de la dotación vigente del
> respectivo organismo." (cita completa y contexto en `mapa-articulos-reglamento-mpi.md`, Art. 7)

**Razonamiento aplicado:** a diferencia de una empresa privada, un SLEP no puede subcontratar
externamente la función de DPO — debe ser un funcionario de su propia dotación.

### Voluntariedad — corrección de una fuente interna del proyecto
> **TEXTO LITERAL** (Art. 49 Ley 19.628 modificada, línea 3179) "Los responsables de datos podrán
> voluntariamente adoptar un modelo de prevención de infracciones" — (Reglamento Art. 6, línea 253) "El
> responsable de datos **podrá** designar un delegado [...] designación que será **obligatoria en el
> marco de la adopción y certificación** de un programa de cumplimiento" — (Art. 48 Ley 19.628
> modificada, línea 3172) "Los responsables de datos [...] deberán adoptar acciones destinadas a prevenir
> la comisión de las infracciones [...]" (deber general de prevención, sin mencionar DPO)

**Razonamiento aplicado:** la designación de DPO es, por texto expreso, **voluntaria en general** y
obligatoria **solo** si el organismo decide adoptar y certificar un programa de cumplimiento. El archivo
interno `.compliance-slep-context.md` del proyecto SLEP afirmaba que el DPO es "requerido por Art. 48" —
**esto no coincide con la lectura literal del Art. 48**, que es una norma general de prevención sin
mandato de designación (el mandato, condicionado, está en el Art. 49/Reglamento Art. 6, no en el 48).
Antes de tratar el DPO como obligación legal dura para un SLEP, verificar si existe una norma sectorial
distinta (instructivo de la Agencia, Ley 21.040, o reglamento propio de la Dirección de Educación
Pública) que sí lo imponga — no dar por buena la cita del Art. 48 sin confirmar contra el texto.

### Formalizar el DPO no es lo mismo que cubrir la función
Designar un DPO conforme al Reglamento Art. 8 (acto formal, máxima autoridad, autonomía — texto completo
en `mapa-articulos-reglamento-mpi.md`) activa el régimen completo de los Arts. 7-13, exista o no MPI
certificado. Un organismo que quiera cubrir la función sin comprometerse todavía a ese régimen completo
puede asignarla informalmente (ej. "coordinador de privacidad") sin dictar el acto de designación del
Art. 8 ni presentarla como DPO reglamentario ante la Agencia. Es una decisión de diseño institucional, no
una zona gris legal: si se formaliza como DPO, rige el estatuto completo aunque el MPI nunca llegue a
certificarse.

## Aplicación a la data del ecosistema SLEP (según `.compliance-slep-context.md` del proyecto)

### PIE (NEE/salud) y licencias médicas docentes
> **TEXTO LITERAL** (Art. 2 letra g, ver cita completa en `mapa-articulos-ley21719.md`) "Datos personales
> sensibles: [...] los datos relativos a la salud [...]"

**Razonamiento aplicado:** dato sensible por definición legal — exige consentimiento expreso/reforzado
(Art. 16) o base legal específica (Decretos 170/2009, 83/2015 para PIE); nunca tratarlo como dato común.

### IVE (Índice de Vulnerabilidad Escolar)
> **TEXTO LITERAL** (Art. 2 letra g) "[...] revelen [...] la situación socioeconómica [...]"

**Razonamiento aplicado:** dato socioeconómico sensible por definición legal expresa — no es una
categoría de sensibilidad "de facto" inventada por la práctica educativa, está en el texto mismo de la
ley.

### MRUN, RUT
> **TEXTO LITERAL** (Art. 2 letra f) "Dato personal: cualquier información vinculada o referida a una
> persona natural identificada o identificable [...] mediante uno o más identificadores, tales como el
> nombre, el número de cédula de identidad [...]"

**Razonamiento aplicado:** identificadores directos — la regla CGR del usuario que prohíbe llevarlos a
prompts tiene aquí su base legal exacta: son datos personales por definición del Art. 2 letra f), no una
prudencia interna sin respaldo normativo.

### Transferencia a Microsoft/SharePoint u otro cloud extranjero
> **TEXTO LITERAL** (Art. 27, ver cita completa en `mapa-articulos-ley21719.md`) "son lícitas las
> operaciones de transferencia internacional de datos en cualquiera de los siguientes casos [...]"

**Razonamiento aplicado:** si el proveedor cloud está fuera de Chile, aplica el Título V completo (Arts.
27-29) — pendiente DPA formal con base de transferencia identificada (país adecuado, cláusulas
contractuales, o modelo de certificación), ya señalado como crítico en el proyecto SLEP.

### Transferencias a MINEDUC/SIGE, DEMRE, CPEIP, JUNJI
> **TEXTO LITERAL** (Art. 22, ver cita completa en `mapa-articulos-ley21719.md`) "Los órganos públicos
> están facultados para comunicar o ceder datos personales [...] a otros órganos públicos, siempre que la
> comunicación o cesión [...] resulte necesaria para el cumplimiento de sus funciones legales y ambos
> órganos actúen dentro del ámbito de sus competencias."

**Razonamiento aplicado:** tratamiento entre órganos públicos — requiere base legal específica por
convenio o ley sectorial y publicación mensual del convenio en el sitio web institucional (mismo
artículo), no basta invocar "interés institucional" genérico.

## Relación con la skill `compliance-cl`
Esta skill (`proteccion-datos-personales-cl`) es la fuente de interpretación legal verificada artículo
por artículo, con texto literal citado y razonamiento separado. `compliance-cl` es el generador de
documentos (RAT, políticas, DPA, EIPD). Si hay una duda de fondo sobre qué dice la ley → resolver aquí
primero, con cita de artículo verificado contra `sources/especifico/`; luego pasar el hallazgo a
`compliance-cl` para que lo materialice en el documento correspondiente.
