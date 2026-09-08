# Privacidad desde el diseño y Accountability — la ley manda, los estándares aterrizan

> **Jerarquía de este archivo (contrato v3, ARQUITECTURA.md §6.1.b):** todo punto parte de lo que exige
> la Ley 19.628 modificada — eso es lo obligatorio. Los bloques `COMPLEMENTARIO` que siguen (ISO 29100,
> ISO/IEC 27701, NIST Privacy Framework, NIST AI RMF, doctrina del Diplomado U. Chile) no son ley chilena
> y no crean obligación nueva — solo dan el "cómo" operativo que la ley no detalla. Fuente de cada cita
> complementaria en `sources/complementario/`.

## 1. Privacidad desde el diseño y por defecto — Art. 14 quáter

> **TEXTO LITERAL** (Art. 14 quáter Ley 19.628 modificada, `sources/especifico/ley-21719-texto.txt`)
> "Con la finalidad de cumplir los principios y los derechos de los titulares establecidos en esta ley,
> el responsable debe aplicar medidas técnicas y organizativas adecuadas desde el diseño con anterioridad
> y durante el tratamiento de los datos personales. [...] Asimismo, el responsable de datos deberá
> aplicar medidas técnicas y organizativas para garantizar que, por defecto, sólo sean objeto de
> tratamiento los datos personales específicos y estrictamente necesarios para dicha actividad."

**Razonamiento aplicado:** son dos obligaciones distintas, no una — "desde el diseño" (anticipar la
privacidad al construir el sistema/proceso, no parchearla después) y "por defecto" (la configuración
inicial debe ser la más protectora, no la más permisiva). La ley exige el resultado (medidas técnicas y
organizativas adecuadas) pero no dice CÓMO construirlas paso a paso — ahí es donde entra el
complementario.

> **COMPLEMENTARIO** (NIST Privacy Framework 1.1, función Govern-P/Control-P,
> `sources/complementario/nist-privacy-framework-1.1.pdf.extracto/chunk_017.md`)
> "Govern-P – Develop and implement the organizational governance structure to enable an ongoing
> understanding of the organization's risk management priorities that are informed by privacy risk. [...]
> Control-P – Develop and implement appropriate activities to enable organizations or individuals to
> manage data with sufficient granularity to manage privacy risks."

**Cómo aterriza esto el Art. 14 quáter:** el NIST Privacy Framework traduce "medidas técnicas y
organizativas desde el diseño" en dos funciones operativas separables — primero **Govern-P** (fijar
políticas y valores de privacidad de la organización, ANTES de diseñar cualquier sistema) y luego
**Control-P** (dar a la organización granularidad real para limitar/gestionar el dato en el sistema ya
construido). Es una hoja de ruta de implementación, no una obligación legal adicional — la obligación
legal es una sola: cumplir el Art. 14 quáter.

> **COMPLEMENTARIO** (Diplomado U. Chile, MOD01.01,
> `sources/complementario/mod01.01-gobierno-corporativo-proteccion-datos.pdf.extracto/chunk_054.md`)
> "Privacy by Design Estratégico: Plataformas — Arquitectura tecnológica con privacidad integrada desde
> su concepción. Modelos de negocio — Estrategias comerciales que respetan derechos fundamentales.
> Contratos — Acuerdos con cláusulas robustas de protección de datos. Campañas — Iniciativas de marketing
> con privacidad como valor central."

**Razonamiento aplicado:** este material de doctrina extiende el "diseño" más allá de lo puramente
técnico (arquitectura de sistemas) a 4 planos donde un SLEP/colegio también debe aplicar el principio:
al construir una plataforma (ej. un sistema propio de gestión escolar), al definir un modelo de servicio
nuevo, al redactar contratos con proveedores, y al diseñar campañas de comunicación/marketing hacia
apoderados. Es una ampliación práctica razonable del Art. 14 quáter, no una fuente legal — no citar esto
como si fuera obligación normativa.

## 2. Principio de responsabilidad (accountability) — Art. 3° letra e)

> **TEXTO LITERAL** (Art. 3° letra e, `sources/especifico/ley-21719-texto.txt`)
> "Principio de responsabilidad. Quienes realicen tratamiento de los datos personales serán legalmente
> responsables del cumplimiento de los principios contenidos en este artículo y de las obligaciones y
> deberes de conformidad a la ley."

**Razonamiento aplicado:** la ley chilena llama a esto "principio de responsabilidad" — es el mismo
concepto que la doctrina internacional llama "accountability" (responsabilidad demostrable), pero el
texto legal no detalla CÓMO se demuestra el cumplimiento, solo que se es responsable de cumplirlo.

> **COMPLEMENTARIO** (Diplomado U. Chile, MOD01.03,
> `sources/complementario/mod01.03-gobernabilidad-accountability.pdf.extracto/chunk_005.md` y `chunk_006.md`)
> "La accountability o responsabilidad demostrable [...] exige a las organizaciones poder demostrar,
> mediante evidencia documental, que efectivamente están implementando las medidas necesarias para
> proteger adecuadamente los datos personales. [...] Componentes del accountability: El Registro de
> Actividades de Tratamiento (RAT) documenta todos los procesamientos de datos personales. Las
> Evaluaciones de Impacto (PIA) analizan riesgos potenciales antes de implementar nuevos tratamientos. La
> capacitación continua asegura que el personal esté actualizado, mientras que las políticas y
> procedimientos establecen reglas claras. Finalmente, la gestión de brechas garantiza respuestas
> adecuadas ante incidentes."

**Razonamiento aplicado — esto es lo que responde directamente "cómo se demuestra" el Art. 3° letra e):**
5 componentes concretos, cada uno con anclaje en un artículo específico de la ley que ya está en
`references/especifico/`: **RAT** (equivalente al contenido del Art. 14 ter + Art. 3 Reglamento MPI) →
**EIPD/PIA** (obligatoria en los 4 supuestos del Art. 15 ter) → **capacitación** (función del DPO, Art.
50 letra d / Reglamento Art. 13 letra f) → **políticas y procedimientos** (Art. 14 ter, política de
tratamiento publicada) → **gestión de brechas** (Art. 14 sexies). El principio de responsabilidad del
Art. 3° letra e) no es abstracto — se demuestra exactamente con estos 5 instrumentos, cada uno ya exigido
en otro artículo de la misma ley. **Nota de verificación:** el material del Diplomado menciona
"Ley 21.521 chilena" como fuente del principio junto al GDPR — esto no coincide con la fuente específica
verificada de esta skill (la ley de datos personales es la 19.628 modificada por la 21.719, no existe una
"Ley 21.521" identificada en `sources/especifico/`); se trata como posible error del material de origen,
no se propaga esa cita sin verificarla por separado.

> **COMPLEMENTARIO** (Diplomado U. Chile, MOD01.01,
> `sources/complementario/mod01.01-gobierno-corporativo-proteccion-datos.pdf.extracto/chunk_033.md`)
> "¿Qué es Accountability? Más allá del cumplimiento: no solo cumplir con la normativa, sino poder
> demostrarlo de manera efectiva. Implica un enfoque proactivo y documentado de la protección de datos."

**Razonamiento aplicado:** distinción práctica útil para auditoría — "cumplir" (hecho) vs. "poder
demostrar que se cumplió" (evidencia) son dos cosas distintas; un SLEP puede estar cumpliendo
sustantivamente la ley y aun así fallar el estándar de accountability si no tiene cómo probarlo
documentalmente ante una fiscalización de la Agencia.

## 3. Gobernanza de IA (angular adicional, cuando el tratamiento incluye IA/perfilamiento)

> **COMPLEMENTARIO** (NIST AI RMF 1.0, función GOVERN,
> `sources/complementario/nist-ai-rmf-100-1.pdf.extracto/chunk_026.md`)
> "GOVERN is a cross-cutting function that is infused throughout AI risk management [...] Documentation
> can enhance transparency, improve human review processes, and bolster accountability in AI system
> teams."

**Razonamiento aplicado:** cuando el tratamiento del Art. 14 quáter involucra decisiones automatizadas o
perfilamiento (Art. 8° bis, Art. 15 ter letra a), el "diseño" y la "responsabilidad demostrable" se
extienden al equipo que construye/opera el sistema de IA, no solo a quien redacta la política de
privacidad — el NIST AI RMF aporta aquí una función de gobierno específica para ese caso, complementaria
al Art. 14 quáter/Art. 3° letra e), nunca sustituta de ellos.

## Grafo
Se cita junto con `mapa-articulos-ley21719.md` (Arts. 3, 8 bis, 14 quáter, 15 ter, 50) — este archivo no
tiene sentido de forma aislada, es un cruce, no una fuente autónoma.
