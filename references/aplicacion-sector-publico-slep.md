# Aplicación al sector público — SLEP y organismos educativos

> Ángulo específico para servicios públicos (SLEP, DEM/DAEM, DEP). El régimen aplicable de tratamiento
> de datos por órganos públicos es el **Título IV de la Ley 19.628 modificada (Arts. 20-26)**, no el
> régimen general de privados (Título II) — ver `mapa-articulos-ley21719.md`.

## Puntos que cambian frente a un privado
- **Art. 44**: responsabilidad administrativa recae en el **jefe superior del órgano público** — en un
  SLEP, la Dirección Ejecutiva.
- **Art. 45**: responsabilidad del funcionario infractor (individual, no solo institucional).
- **Art. 46**: deber de reserva/confidencialidad de los funcionarios.
- **Art. 25**: reglas especiales para datos de infracciones penales/administrativas/disciplinarias que
  procesa el organismo (ej. sumarios, licencias médicas con causa).
- Coexiste con **Ley 20.285** (transparencia): un dato puede ser público para efectos de transparencia
  activa/pasiva y aun así estar protegido como dato personal — no son mutuamente excluyentes, se pide
  la base de licitud correcta en cada caso (transparencia vs. protección de datos no chocan si se
  aplica el test de daño/interés público correctamente).

## DPO en el sector público — precisión importante
El **Reglamento MPI (Art. 7 inciso 2°)** exige que, si un órgano público designa un delegado de
protección de datos, este **debe ser un funcionario de la dotación vigente** — no puede subcontratarse
externamente como sí puede hacer una empresa privada.

**Punto a verificar activamente, no asumir:** la designación del DPO es, por el texto de la Ley
19.628 (Art. 49, "podrán adoptar e implementar **voluntariamente**") y del Reglamento (Art. 6, "podrá
designar... obligatoria **en el marco de la adopción y certificación** de un programa de cumplimiento"),
en principio **voluntaria** — se vuelve obligatoria solo si el organismo decide certificar un MPI.
El `.compliance-slep-context.md` del proyecto SLEP afirma que el DPO es "requerido por Art. 48" para
organismos públicos — **esto no coincide con la lectura literal de Arts. 48-49** (el 48 es una norma
general de prevención, no un mandato de designación). Antes de tratar el DPO como obligación legal
dura para el SLEP, verificar si existe una norma sectorial distinta (ej. instructivo de la Agencia,
Ley 21.040, o reglamento propio de la Dirección de Educación Pública) que sí lo imponga — no dar por
buena la cita sin confirmar contra el texto.

**Matiz adicional — formalizar el DPO no es lo mismo que cubrir la función (verificado Arts. 6-8):**
designar un DPO conforme al Art. 8 (acto formal, máxima autoridad, autonomía) activa el régimen
completo de los Arts. 7-13, exista o no MPI certificado. Un organismo que quiera tener la función
cubierta sin comprometerse todavía a ese régimen completo puede asignarla informalmente (ej.
"coordinador de privacidad") sin dictar el acto de designación del Art. 8 ni presentarla como DPO
reglamentario ante la Agencia. Es una decisión de diseño institucional, no una zona gris legal: si se
formaliza como DPO, rige el estatuto completo aunque el MPI nunca llegue a certificarse.

## Aplicación a la data del ecosistema SLEP (según `.compliance-slep-context.md`)
- **PIE** (NEE/salud) y **licencias médicas docentes** → datos sensibles, Art. 16 y ss. (consentimiento
  expreso/reforzado o base legal específica; nunca tratarlos como dato común).
- **IVE** → dato socioeconómico sensible (Art. 2 letra g).
- **MRUN, RUT** → datos personales identificadores (Art. 2 letra f) — regla CGR del usuario ya prohíbe
  llevarlos a prompts; esta skill refuerza la base legal de por qué.
- **Transferencia a Microsoft/SharePoint** → si el proveedor cloud está fuera de Chile, aplica Título V
  (Arts. 27-29, transferencia internacional) — pendiente DPA formal, ya identificado como crítico.
- **Transferencias a MINEDUC/SIGE, DEMRE, CPEIP, JUNJI** → tratamiento entre órganos públicos (Art. 22,
  comunicación/cesión por órgano público) — requiere base legal específica por convenio o ley sectorial,
  no basta el interés institucional genérico.

## Relación con la skill `compliance-cl`
Esta skill (`ley-21719-cl`) es la fuente de interpretación legal verificada artículo por artículo.
`compliance-cl` es el generador de documentos (RAT, políticas, DPA, EIPD). Si hay una duda de fondo
sobre qué dice la ley → resolver aquí primero, con cita de artículo verificado; luego pasar el hallazgo
a `compliance-cl` para que lo materialice en el documento correspondiente.
