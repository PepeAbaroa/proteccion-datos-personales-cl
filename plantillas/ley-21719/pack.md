# Pack: Ley 21.719 — Protección de Datos Personales

> Vigencia **1-dic-2026** (publicada 13-dic-2024). Aplica a todos sin umbral. Gracia MIPYME (Ley 20.416):
> los primeros 12 meses (dic-2026 → dic-2027) la Agencia puede aplicar amonestación en vez de multa
> (Art. sexto transitorio). Numeración verificada en `references/mapa-articulos-21719.md`.

## Controles que exige (ver `references/controls.md`)
`gov-responsable`, `gov-registro` (RAT), `gov-politicas`, `gov-denuncias`/`data-rights-channel`,
`data-licitud`, `data-consent-text`, `data-derechos`, `data-info`, `data-minimizacion`, `data-dpa`,
`data-transfer`, `data-eipd`, `data-privacy-by-design`, `data-pseudonym`, `sec-tls`, `sec-rest`,
`sec-passwords`, `sec-mfa`, `sec-logs`, `sec-tenant`, `sec-secrets`, `sec-backups`, `inc-brechas`.

## Obligaciones clave (resumen)
- **Roles:** responsable (decide fines) vs encargado (Art. 15 bis: trata por cuenta de otro, según
  contrato; no usa los datos para fines propios).
- **Consentimiento (Art. 12):** previo, libre, específico, informado e inequívoco (acto afirmativo,
  casilla NO premarcada) y **revocable**. Carga de la prueba: del responsable.
- **Deber de información (Art. 14 ter):** identidad, finalidad, base, destinatarios, transferencias,
  retención, derechos, decisiones automatizadas, origen y cómo recurrir a la Agencia.
- **Derechos:** acceso, rectificación, supresión, oposición, portabilidad, bloqueo. Plazo **30 días
  corridos**, prorrogable **una sola vez por 30 más**. Rectificación/supresión/oposición siempre gratis;
  acceso gratis al menos trimestralmente.
- **Seguridad (Art. 14 quinquies)** proporcional + **privacy by design/default (Art. 14 quáter)** +
  seudonimización. **Brechas (Art. 14 sexies):** reportar **sin dilaciones indebidas** (NO 72h),
  registrar las vulneraciones, avisar a titulares si riesgo alto o si afecta datos sensibles/
  económicos/financieros/niños.
- **Datos sensibles (Art. 16):** consentimiento expreso y reforzado.
- **DPO:** voluntario para todo responsable, público o privado, sin excepción por tipo de organismo ni
  por escala de tratamiento (Art. 49-50 Ley 19.628 modificada) — obligatorio solo si se adopta el MPI.
  Si un órgano público lo designa, debe ser funcionario de la dotación vigente (Art. 7 inciso 2°
  Reglamento MPI + Art. quinto transitorio Ley 21.719); en micro/pyme privada lo puede asumir el dueño.
- **EIPD (Art. 15 ter):** dos niveles, verificado 2026-07-30. (1) Cláusula general (inciso 1°): juicio
  caso a caso si es "probable" un alto riesgo por naturaleza/alcance/contexto/tecnología/fines — puede
  gatillarla aunque ninguna letra de abajo aplique literalmente. (2) Piso obligatorio SIEMPRE si
  concurre alguna de 4 letras (a-d), no 5: a) evaluación sistemática/perfilado/decisión automatizada
  con efecto jurídico significativo (es UNA letra, no dos); b) tratamiento masivo **o a gran escala**
  (general, no dice "sensibles o niños"); c) observación/monitoreo sistemático de zona de acceso
  público; d) datos sensibles **en hipótesis de excepción del consentimiento** — aplica con cualquiera
  de las 6 excepciones del Art. 16 (incl. la e, ámbito laboral), sin excepción de proporcionalidad por
  tamaño (el Art. 14 septies no cubre el Art. 15 ter). No existe un criterio de "tecnología nueva" —
  estaba mal en versiones anteriores de este pack. Detalle: `templates/eipd.md`.
- **Transferencias internacionales (Arts. 27-29):** mecanismos válidos = a) país con nivel adecuado
  (determinado por **la Agencia**, Art. 28), b) cláusulas contractuales/normas corporativas vinculantes
  aprobadas por **la Agencia** (no por el Ministerio — corregido 2026-07-30), c) modelo de cumplimiento/
  certificación. Sin esos 3, hay 8 causales de excepción para transferencias específicas no habituales
  (consentimiento expreso, transferencias bancarias/financieras, tratados internacionales, convenios de
  cooperación entre órganos públicos, autorización legal expresa, colaboración judicial, ejecución de
  contrato, urgencia médica/sanitaria) — Art. 27.

## Sanciones (Art. 34 clasificación + Art. 35 montos — verificado)
Leve: amonestación o hasta 5.000 UTM · grave hasta 10.000 UTM · gravísima hasta 20.000 UTM.
Reincidencia (Art. 35): empresas de menor tamaño → 2% o 4% de ingresos anuales. Fiscaliza la Agencia.

## Atenuante
**MPI** (Modelo de Prevención de Infracciones, Arts. 49-53), voluntario, lo certifica la Agencia.

## Documentos a generar (templates/ → `<repo>/.compliance/docs/` con prefijo `21719-`)
`rat.md`, `politica-privacidad.md`, `consentimiento.md` (opt-in + aviso + sensibles), `canal-derechos.md`,
`dpa.md`, `anexo-transferencias.md`, `plan-respuesta-brechas.md`, `registro-vulneraciones.md`,
`eipd.md` (si el test del Art. 15 ter da obligatoria).
