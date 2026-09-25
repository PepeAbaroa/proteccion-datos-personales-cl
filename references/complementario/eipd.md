# EIPD operativa — fases, escalas, factores, medidas y reevaluación

> **Jerarquía**: lo obligatorio en Chile es solo lo que dice la ley (Art. 15 ter y los deberes de los Arts.
> 14 quáter, 14 quinquies y 14 sexies; ver `references/especifico/mapa-articulos-ley21719.md`). Todo lo
> que aquí viene de la AEPD o del EDPB describe el RGPD europeo: **metodología comparada, no norma
> chilena**. Se usa para *llenar y justificar* una EIPD, nunca para agregar obligaciones.
>
> Fuentes públicas (página = la impresa en el documento):
> - **AEPD-GR**: AEPD, *Gestión del riesgo y evaluación de impacto en tratamientos de datos personales* (2021).
> - **AEPD-GP**: AEPD, *Guía práctica para las Evaluaciones de Impacto en la Protección de Datos sujetas al RGPD* (2018).
> - **AEPD-PbD**: AEPD, *Guía de Privacidad desde el Diseño* (oct. 2019).
> - **EDPB-2026**: EDPB, *Template [2026] for Data Protection Impact Assessment – Explainer*, v1.0, adoptado
>   el 10-mar-2026 **para consulta pública** (borrador; puede cambiar).
> Complementa `criterios-rat-eipd-mpi.md` §2 (contenido y mapeo del template EDPB) — no lo repite.

## 1. Filtro de obligatoriedad (antes de empezar)

1. **Supuestos siempre obligatorios — Art. 15 ter inc. 2°**: a) evaluación sistemática/perfilamiento con
   efectos jurídicos significativos; b) tratamiento masivo o a gran escala; c) monitoreo sistemático de zona
   de acceso público; d) datos sensibles y especialmente protegidos **en las hipótesis de excepción del
   consentimiento** (no "cualquier dato sensible").
2. **Cláusula general — Art. 15 ter inc. 1°**: probable alto riesgo por naturaleza, alcance, contexto,
   **tecnología utilizada** o fines. Método práctico: calcular el riesgo inherente con §3; si sale Alto o
   Muy alto, hacer EIPD.
3. **Heurística comparada** (mientras la Agencia no publique su lista orientativa, Art. 15 ter inc. 3°): en
   la UE se presume alto riesgo con dos o más criterios de las listas de la autoridad o de WP248, y el
   responsable puede exigirla con uno solo (AEPD-GR p. 134, 136).
4. **Órgano público**: el Art. 21 no remite al Art. 15 ter → buena práctica salvo exigencia específica
   (ver `criterios-rat-eipd-mpi.md` §2).
5. Documentar siempre la decisión (obligatoria / recomendada / no requerida) y quién la sugirió (AEPD-GR p. 137).

## 2. Cuatro fases operativas

La EIPD es un **proceso** que dura todo el ciclo de vida, no un informe (AEPD-GR p. 25-26). Estructura
recomendada, compatible con AEPD-GP (contexto → gestión de riesgos → conclusión + supervisión, p. 6-7,
12) y con las secciones 0-6 de EDPB-2026:

| Fase | Pasos | Salidas | Fuente comparada | Ancla CL |
|---|---|---|---|---|
| **1 Entender** | ficha (responsable, encargados, nombre del RAT, fechas, equipo, alcance, motivo); fines bien definidos (fin último, no el medio); descripción sistemática; ciclo de vida por etapa (captura → almacenamiento → uso → cesión → destrucción) con actividades, tecnología, intervinientes y datos; activos de soporte | ficha, descripción, tabla de ciclo de vida, inventario de activos | EDPB-2026 p. 5-7; AEPD-GR p. 29, 60-70; AEPD-GP p. 12-13 | Art. 15 ter inc. 3°; Reglamento MPI Art. 3 d) (caracterización = insumo del RAT) |
| **2 Descubrir riesgos y mitigarlos** | licitud; minimización/conservación/calidad; medidas previstas; juicio de **idoneidad, necesidad y proporcionalidad** (si no se supera, se rediseña: la seguridad no compensa la falta de necesidad); escenarios "por diseño" y por fallo/ataque; riesgo inherente; tratamiento; riesgo residual | análisis de licitud, juicio de proporcionalidad, registro de escenarios, niveles inherente/residual | AEPD-GR p. 138-139; EDPB-2026 p. 10-12; AEPD-GP p. 20-33 | Arts. 3° b)-d), 12-13, 16, 16 quáter, 14 quinquies |
| **3 Formalizar** | plan de acción (control, descripción, responsable, plazo, estado); opinión del delegado y qué se hizo con ella; opinión de titulares o por qué no; decisión (a) abandonar, (b) consultar, (c) seguir, (d) seguir con condiciones | plan, acta del delegado, decisión firmada | AEPD-GP p. 33-34; EDPB-2026 p. 13 | Art. 50 (delegado facultativo); Reglamento MPI Art. 13 g)-h); Art. 15 ter inc. final (consulta **facultativa**) |
| **4 Seguir** | verificar implantación antes de operar (si vence el plazo, se puede detener el tratamiento); monitoreo; reevaluación por disparadores (§6); cada vulneración reabre la evaluación | informe de seguimiento, versiones | AEPD-GP p. 34, 36; AEPD-GR p. 52-53 | Art. 14 quáter ("con anterioridad y durante"); Art. 14 quinquies d); Art. 14 sexies |

**Riesgo "por diseño" vs. "por fallo"** (EDPB-2026 p. 10-11): los primeros existen aunque todo funcione como
se diseñó (identificadores únicos, conservación larga, perfilamiento); los segundos surgen de desviaciones
(errores, malas configuraciones, abuso interno, ataques) y deben cubrir al menos acceso ilegítimo,
modificación no deseada y desaparición de datos.

## 3. Escalas y cálculo (método comparado)

- **Probabilidad** 1-4: despreciable (fortuito) · limitada (ocasional) · significativa (bastante frecuente) ·
  máxima (muy frecuente) (AEPD-GP p. 27). Evidencia para justificarla: si el factor ya está presente o hubo
  materializaciones en el último año → muy alta; una materialización en alguna entidad el último año,
  vulnerabilidades o tecnología inmadura → alta; alguna en 10 años → baja; ninguna → improbable (AEPD-GR p. 76-77).
  La probabilidad de brecha crece con los años de operación (AEPD-GR p. 96).
- **Impacto** 1-4 sobre daño físico, material o moral: despreciable · limitado · significativo · máximo
  (irreversible) (AEPD-GP p. 27-28). Criterios: irreversibilidad, datos sensibles, discriminación, NNA o
  vulnerables, suplantación, pérdida financiera, ruptura de secreto (AEPD-GR p. 75-76).
- **Riesgo = P × I**; bandas: Bajo 1-2 · Medio >2-6 · Alto >6-9 · Muy alto >9 (AEPD-GP p. 26, 29).
  Alternativa cualitativa: con impacto muy significativo el riesgo es Muy alto incluso con probabilidad
  improbable (AEPD-GR p. 75) — coherente con EDPB-2026 p. 12 (severidad muy alta puede ser inaceptable
  aunque la probabilidad sea baja).
- **Moduladores**: gran número de titulares, alta sensibilidad, dependencia o vulnerabilidad (NNA, pacientes,
  trabajadores), exposición a adversarios suben el nivel; las medidas de diseño lo bajan (EDPB-2026 p. 12).
- **Nivel del tratamiento**: nunca menor que el del factor más alto; los factores interactúan y pueden
  acumularse (AEPD-GR p. 102-103).
- **Residual**: reestimar según efectividad de controles — despreciable (no baja), significativa
  (reestimar), máxima (baja a Bajo) (AEPD-GR p. 126-127).
- **Aceptación**: en el método comparado, residual Bajo o Medio es asumible; superior a Medio exige más
  medidas e iterar (AEPD-GR p. 127). **La ley chilena no fija umbral**: el responsable decide y debe poder
  acreditar sus medidas (Art. 14 quinquies inc. final); si el resultado es alto riesgo *puede* consultar a la
  Agencia (Art. 15 ter inc. final). En la UE, en cambio, residual alto obliga a consulta previa — no trasladar.

## 4. Factores de riesgo con nivel mínimo sugerido (AEPD-GR p. 78-94, extracto)

| Categoría | Muy alto | Alto | Medio / Bajo |
|---|---|---|---|
| Fines | rastreo de contactos; decidir sobre derechos fundamentales; predicción genética | perfilamiento, puntuación, inferencia; vigilancia; decisiones automatizadas; decidir acceso a servicios/contratos | control de trabajadores, localización (Medio); control físico de acceso (Bajo) |
| Datos | salud, genéticos, categorías especiales, penales | biométricos, medios de pago, sensibles seudonimizados | preferencias, finanzas, metadatos, identificadores (Medio) |
| Extensión | gran número de titulares; volumen muy elevado | sistemático, exhaustivo, gran escala, recopilación excesiva | duración o alcance geográfico (Medio) |
| Titulares | niños (<14), víctimas, enfermedad mental, vulnerables/desequilibrio de poder | discapacidad, pacientes, exclusión social | mayores (Medio); trabajadores (Bajo) |
| Técnica | IoT | biometría facial/huella, localización, tecnologías nuevas o inmaduras, videovigilancia | apps, web, automatización (Medio) |
| Recogida | — | cruce de bases, recogida poco transparente | zonas públicas, fuentes múltiples (Medio) |
| Comunicaciones | transferencia habitual a país sin nivel adecuado | difusión de identificadores únicos | falta de transparencia de actores (Medio) |

Ancla chilena de los factores más usados: sensibles Art. 2° g) y 16; salud 16 bis; biométricos 16 ter;
NNA 16 quáter (niño <14, adolescente 14-17; sensibles de <16 con consentimiento de padres); geolocalización
16 sexies; decisiones automatizadas 8° bis; transferencias 27-28. Los niveles son europeos y ajustables.

## 5. Medidas (catálogo resumido)

- **Clasificación**: preventivas/detección/correctivas; reducir, evitar, aceptar, transferir; organizativas,
  legales, técnicas (AEPD-GR p. 38; AEPD-GP p. 31-32). Cumplir el deber de información o atender derechos
  no es mitigación; solo lo que excede el mínimo cuenta (AEPD-GR p. 39).
- **Sobre el concepto del tratamiento**: eliminar/aislar fases, tecnología menos invasiva, supervisión humana,
  acotar titulares/ámbitos/tiempo, eliminar fines secundarios, limitar lo que ve el encargado (AEPD-GR p. 104-105).
- **Privacidad desde el diseño — 8 estrategias** (AEPD-PbD p. 17-24): orientadas a datos — *minimizar*
  (seleccionar, excluir, podar, eliminar), *ocultar* (restringir, ofuscar, disociar, agregar), *separar*
  (aislar, distribuir), *abstraer* (sumarizar, agrupar, perturbar); orientadas a procesos — *informar*
  (facilitar, explicar, notificar), *controlar* (consentir, alertar, elegir, actualizar, retirar), *cumplir*
  (definir, mantener, defender), *demostrar* (registrar, auditar, informar). Ancla CL: Art. 14 quáter;
  seudonimización y cifrado en Art. 14 quinquies a).
- **Seguridad** (AEPD-GP p. 58-63): acceso por necesidad de saber y revocación oportuna; logs; detección de
  intrusiones y parches; respaldos y restauración (Art. 14 quinquies b-c); borrado automático al vencer el
  plazo; identificadores sin datos triviales; disociación robusta; verificación periódica de eficacia
  (Art. 14 quinquies d). Controles técnicos detallados → skill `infraestructura-ciberseguridad`.
- **Plan de acción**: control, descripción, responsable, plazo, estado, efectividad esperada, evidencia
  (AEPD-GP p. 33; EDPB-2026 p. 13).

## 6. Cuándo reevaluar (disparadores, AEPD-GR p. 128; AEPD-GP p. 38)

- **Naturaleza**: cambia el responsable, la implementación o la tecnología; se reemplaza a personas por
  sistemas; cambian encargos; una medida resulta ineficaz.
- **Ámbito**: más titulares, nuevas categorías de datos, más volumen o frecuencia, más alcance.
- **Contexto**: desaparece la justificación; incidentes o brechas propios o en tratamientos similares; nuevas
  amenazas; cambios normativos (p. ej., instrucciones de la Agencia bajo el Art. 14 septies).
- **Fines**: se agregan o cambian fines.
- Ejemplos: nuevo canal, automatización, externalización. Un cambio menor igual se valora y se documenta que
  no requiere medidas nuevas (AEPD-GP p. 7). Si un cambio vuelve obligatoria una EIPD que no se hizo, se hace
  de inmediato (AEPD-GR p. 131).

## 7. Qué NO trasladar del RGPD

Consulta previa obligatoria (Art. 36 RGPD) · listas nacionales europeas y excepción del Art. 35.10 ·
delegado obligatorio · opinión de interesados como deber (aquí es buena práctica) · referencias a la LOPDGDD,
al ENS o a la Constitución española · la plantilla EDPB como formato "oficial" (en Chile lo fijará la Agencia).

## Grafo
Depende de `references/especifico/mapa-articulos-ley21719.md` (Arts. 2°, 3°, 8° bis, 14 quáter-septies,
15 ter, 16-16 sexies, 21, 27-28, 50) y `mapa-articulos-reglamento-mpi.md` (Arts. 3, 13). Se usa junto con
`criterios-rat-eipd-mpi.md` §2-3 y `privacy-by-design-accountability.md`; la plantilla de documento está en
`plantillas/ley-21719/templates/eipd.md`.
