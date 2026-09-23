# Evaluación de Impacto en Protección de Datos (EIPD) — [RAZÓN SOCIAL]

**RUT:** [RUT] · **Fecha:** [FECHA] · **Responsable:** [NOMBRE / CARGO] · **Tratamiento evaluado:** [NOMBRE]

> Art. 15 ter de la Ley 19.628 (incorporado por la Ley 21.719). La EIPD es **previa** al tratamiento y
> **obligatoria** cuando es probable un alto riesgo para los derechos del titular.

> **Órganos públicos (SLEP, DAEM, otros servicios):** el Art. 21 inc. 3° no incluye el Art. 15 ter entre
> las normas aplicables a los órganos públicos. Para ellos la EIPD no es una obligación del Art. 15 ter
> (ni procede la consulta facultativa de su inc. 4°): es una buena práctica y el medio para acreditar
> el cumplimiento de los Arts. 14 quáter (protección desde el diseño y por defecto) y 14 quinquies
> (medidas de seguridad), que sí les son aplicables. El test de abajo sirve igual para decidir cuándo
> hacerla.

## ¿Es obligatoria? (test del Art. 15 ter, dos niveles)

**Nivel 1 — cláusula general (inciso 1°, no solo las 4 letras de abajo):** "Cuando sea probable que un
tipo de tratamiento, por su naturaleza, alcance, contexto, tecnología utilizada o fines, pueda producir
un alto riesgo para los derechos de las personas titulares..." → juicio caso a caso. Puede gatillar la
EIPD aunque ninguna de las 4 letras siguientes aplique literalmente.

**Nivel 2 — piso obligatorio, SIEMPRE (inciso 2°, 4 letras exactas, no 5).** Marca lo que aplique. Con
UNO que aplique, la EIPD es obligatoria:
- [ ] a) Evaluación sistemática y exhaustiva de aspectos personales de los titulares, basada en
      tratamiento o decisiones automatizadas (incluida la elaboración de perfiles), que produzcan
      efectos jurídicos significativos — es UNA sola letra (perfilado y decisión automatizada van
      juntos, no por separado).
- [ ] b) Tratamiento **masivo** de datos **o a gran escala** — general; el texto NO dice "de datos
      sensibles o de niños" en esta letra (esa condición está en la letra d, más abajo).
- [ ] c) Tratamiento que implique **observación o monitoreo sistemático** de una zona de acceso público.
- [ ] d) Tratamiento de **datos sensibles y especialmente protegidos**, en las hipótesis de
      **excepción del consentimiento** (es decir, cuando se tratan sin consentimiento del titular,
      bajo alguna excepción legal) — más acotado que "cualquier tratamiento masivo de sensibles",
      pero más amplio de lo que parece: aplica con CUALQUIERA de las excepciones del Art. 16 inc. 2°
      (letras a-f) o, para datos de salud, de perfil biológico y biométricos (Arts. 16 bis y 16 ter),
      con cualquiera de las del Art. 16 bis inc. 2° (letras a-f), incluidas las rutinarias — ej.
      licencias médicas del personal: Art. 16 bis inc. 2° letra e) (medicina laboral / evaluación de
      la capacidad laboral) o f) (ley que lo permita e indique la finalidad), considerando la
      prohibición del inc. 3° para datos de salud recolectados en el ámbito laboral salvo autorización
      legal expresa. No existe una excepción de proporcionalidad por tamaño de entidad para la EIPD: el
      Art. 14 septies (diferenciación de estándares) solo cubre los deberes de información (Art. 14
      ter) y seguridad (Art. 14 quinquies), no el Art. 15 ter.

→ **No existe un quinto criterio de "tecnología nueva con riesgos no evaluados"** — no está en el texto
de la ley.

→ Si NO marcaste ninguno (ni el nivel 1 ni el nivel 2): documenta aquí por qué el tratamiento NO es de
alto riesgo y archiva. Si marcaste alguno: completa el resto.

→ **Profundidad, no obligación:** la ley no fija un formato de EIPD. El inciso 3° encarga a la Agencia
publicar una lista orientativa y "orientaciones mínimas" para realizarla, "considerando a lo menos" la
descripción de las operaciones de tratamiento, su finalidad, la evaluación de la necesidad y la
proporcionalidad, y la evaluación de los riesgos y medidas de mitigación (secciones 1-4 abajo). Mientras
la Agencia no las publique, esos elementos son la referencia; cuando las publique, ajustar esta
plantilla. Para
tratamientos rutinarios y de riesgo bajo/medio (ej. licencias
médicas), una EIPD abreviada con esas mismas 4 secciones, en 1-2 páginas, es válida — no hace falta el
mismo nivel de detalle que un sistema de perfilado de riesgo alto.

## 1. Descripción del tratamiento
Finalidad, categorías de datos (incluye si hay sensibles), titulares, flujos, proveedores y
transferencias internacionales. [COMPLETAR — se prellena del RAT.]

## 2. Necesidad y proporcionalidad
¿El dato es necesario para el fin? ¿Se podría lograr con menos datos (minimización)? Base de licitud.

## 3. Riesgos identificados
| Riesgo | Probabilidad | Impacto | Nivel |
|---|---|---|---|
| Acceso no autorizado / fuga | | | |
| Uso para un fin distinto | | | |
| Decisión automatizada injusta / sesgo | | | |
| Reidentificación de datos | | | |

## 4. Medidas de mitigación
Por cada riesgo alto: control técnico u organizativo que lo reduce (cifrado, minimización,
seudonimización, intervención humana en decisiones automatizadas, etc.).

## 5. Conclusión
Riesgo residual aceptable: [sí/no]. Si la evaluación demuestra alto riesgo, el responsable **podrá
consultar** a la Agencia para obtener recomendaciones (Art. 15 ter, inciso 4°: "Los responsables podrán
consultar a la Agencia de Protección de Datos Personales, cuando en virtud del resultado de la
evaluación, el tratamiento demuestre ser de alto riesgo a efectos de obtener recomendaciones de parte de
dicha entidad."). Es **facultativa** y no es una autorización previa: la ley no condiciona el inicio del
tratamiento a esa consulta.

---
*Borrador generado con proteccion-datos-personales-cl (plantillas/ley-21719). No constituye asesoría legal; revisar con un abogado.*

---

## Historial de cambios (no copiar al documento del cliente)

- 2026-07-30 — Test del Art. 15 ter verificado contra el texto. Se agregó el Nivel 1 (cláusula general
  del inciso 1°), que faltaba en versiones anteriores (hallazgo al diseñar el instrumento d en
  `ProteccionDatos-CL`, v6). Se eliminó un quinto criterio de "tecnología nueva con riesgos no
  evaluados" que una versión anterior incluía por error.
- 2026-09-22 — "Profundidad, no obligación": antes decía que la ley fija un "contenido mínimo"; el
  inciso 3° no impone contenido al responsable, fija los criterios de las orientaciones de la Agencia.
- 2026-09-22 — Conclusión: antes decía "consulta previa a la Agencia antes de iniciar el tratamiento",
  importado del modelo RGPD Art. 36, que sí la exige; en la Ley 19.628 la consulta es facultativa.
- 2026-09-22 — Letra d): antes citaba el Art. 16 letra e) (ámbito laboral) como excepción para
  licencias médicas; para datos de salud rige el Art. 16 bis inc. 2° (letras e/f) y su inc. 3°. Se
  corrigió "Art. 15 ter de la Ley 21.719" por "de la Ley 19.628 (incorporado por la Ley 21.719)" y se
  agregó la salvedad para órganos públicos (Art. 21 no incluye el Art. 15 ter).
