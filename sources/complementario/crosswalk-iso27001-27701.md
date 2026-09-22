# Crosswalk — Los 7 procesos × ISO/IEC 27001:2022 (Anexo A) e ISO/IEC 27701:2025 (2ª edición)

## Aviso de verificación
**ISO 27001: verificado al 100%** contra texto oficial completo (ver fuentes abajo) — Anexo A íntegro,
93 controles, 5.1 a 8.34, sin huecos. **ISO 27701: verificado contra texto OCR completo** —
`iso-iec-27701-2025.pdf` ya tiene capa de texto (OCR aplicado 2026-09-14) y fue extraído íntegro (72
páginas). **Es la Segunda Edición (2025-10), no la primera (2019)** que este crosswalk citaba
originalmente — la estructura de cláusulas cambió entre ediciones (ver corrección abajo). El OCR tiene
ruido de reconocimiento ("ISO/IEC" a veces sale "1S0/IEC") — al citar texto literal, limpiar visualmente
contra el chunk fuente antes de usar en un entregable.

**Corrección de edición**: las citas "Cláusula 5.2 (determinar rol Controller/Processor)", "7.2-7.3
Controller", "8.2 Processor", "7.2.6/8.2.6 (DPA)" y "6.13 (brechas)" de versiones anteriores de este
archivo correspondían a una estructura de la edición 2019 no confirmada localmente. La edición 2025
real tiene: Cláusula 4 Contexto (4.1-4.4) · Cláusula 5 Liderazgo (5.1 Liderazgo, **5.2 Política de
privacidad**, **5.3 Roles/responsabilidades/autoridades**) · Cláusula 6 Planificación (6.1 riesgo,
6.1.2 evaluación, 6.1.3 tratamiento) · Cláusula 7 Apoyo (7.1-7.5: recursos/competencia/**7.3
concienciación**/comunicación/información documentada) · Cláusula 8 Operación (8.1 planificación,
**8.2 evaluación de riesgo de privacidad**, 8.3 tratamiento) · Cláusula 9 Evaluación de desempeño
(9.1-9.3) · Cláusula 10 Mejora (10.1-10.2) — misma estructura de alto nivel que ISO 27001 (Anexo SL),
sin la separación Controller/Processor por cláusula que tenía la edición anterior. Esa separación vive
ahora en el **Anexo A**, no en el cuerpo: Tabla A.1 (controles para PII controllers), Tabla A.2
(PII processors), Tabla A.3 (seguridad de la información, ambos roles). Dentro de A.1 ("Conditions for
collection and processing"), verificados con texto completo: **A.1.2.2** identificar y documentar
propósito · **A.1.2.3** identificar base de licitud · **A.1.2.4-5** consentimiento · **A.1.2.6**
evaluación de impacto en privacidad (**EIPD**) · **A.1.2.7** contratos con encargados de tratamiento
(**DPA**) · **A.1.2.8** controlador conjunto (**equivalente ISO al escenario de holding/red de
colegios con matriz y colegios como responsables conjuntos**) · **A.1.2.9** registros de tratamiento
(**RAT**). A.2 (processors) y el resto de A.3 quedan pendientes de mapeo detallado — estructura
confirmada, contenido línea por línea no agotado en esta pasada.

**Nota de licencia**: los PDF de ISO 27001/NCh-ISO 27001 están licenciados a un tercero (uso exclusivo,
"prohibida la reproducción" impreso en cada página). Se usan aquí solo para verificación interna —
cualquier entregable de cliente cita el número de control y una paráfrasis breve propia, nunca el texto
literal del control.

## Por qué vale la pena este crosswalk
Un Excel de auditoría inicial del proyecto (archivado en `../../03_clientes/SLEP_Los_Parques/entregables_historicos/Auditoria - Ley Proteccion y Tratamiento de Datos.xlsx`) ya cita
ISO 27701/27001/NIST/CIS como referencia de buenas prácticas, pero nunca formalizamos la
correspondencia. Sirve para: (a) una organización que ya tiene o busca ISO 27001 puede ver que gran
parte del trabajo de los 7 procesos también sirve para su SGSI, y (b) si más adelante se plantea
certificar el MPI, tener los controles ISO ya mapeados facilita cualquier auditoría externa conjunta.

## Verificación local — ISO 27001 Anexo A, íntegro

Verificado 2026-09 contra dos fuentes oficiales completas, ambas extraídas íntegramente
(`doc_full_extract.py`, integridad de páginas confirmada): `nch-iso-27001-2023-oficial-es.pdf`
(adopción chilena, INN, español — fuente primaria de esta tabla) y `iso-27001-2022-oficial-en.pdf`
(texto ISO original, inglés, cruce de respaldo). Reemplazan a `iso-27001-2022-es.pdf`, que era una
copia parcial/de vista previa (solo 13 de 93 controles con texto legible) — se conserva en disco por
trazabilidad, pero ya no es la fuente de esta tabla. Los 93 controles del Anexo A (5.1-5.37 controles
organizacionales, 6.1-6.8 controles de personas, 7.1-7.14 controles físicos, 8.1-8.34 controles
tecnológicos) están confirmados con texto literal completo en español oficial.

## Tabla de correspondencia

| Proceso (Ley 19.628 modificada) | Controles ISO 27001:2022 Anexo A (verificados ✓) | Extensión ISO 27701:2025, 2ª edición (verificado contra texto OCR) | NIST Privacy Framework 1.1 |
|---|---|---|---|
| 1. Gobernanza e Inventario | **5.1** Políticas de seguridad de la información · **5.9** Inventario de información y otros activos | Cláusula 5.3 (roles, responsabilidades y autoridades) + Anexo **A.1.2.9** (registros de actividades de tratamiento — equivalente al RAT) | Identify-P, categoría ID.IM-P (Inventory and Mapping) |
| 2. Licitud, Transparencia y Derechos | **5.34** Privacidad y protección de la información de identificación personal (PII) | Anexo **A.1.2.2** (identificar y documentar el propósito) · **A.1.2.3** (identificar base de licitud) · **A.1.2.4-5** (consentimiento y derechos del titular) | Control-P; Communicate-P |
| 3. Datos Sensibles y NNA | **5.12** Clasificación de la información · **8.10** Eliminación de información | Pendiente de verificar en detalle — el Anexo A.2 (encargados) y el resto de A.3 (seguridad de la información) aún no están mapeados línea por línea en esta skill; no citar un número de cláusula hasta confirmarlo | Identify-P, categoría ID.RA-P (Risk Assessment) |
| 4. Ciclo de Vida y Terceros | **5.19** a **5.23** Seguridad en la relación con proveedores (5 controles completos: gestión de riesgo, acuerdos, cadena de suministro TIC, seguimiento, nube) · **8.10** Eliminación | Anexo **A.1.2.7** (contratos con encargados de tratamiento — equivalente al DPA) | Govern-P, categoría GV.DE-P (Data Processing Ecosystem) |
| 5. Seguridad y Gestión de Brechas | **5.24** a **5.28** Gestión de incidentes de seguridad completa (planificación, evaluación, respuesta, aprendizaje, recolección de evidencia) | Pendiente de verificar en detalle — mismo motivo que la fila 3 (Anexo A.2/A.3 sin mapeo línea por línea todavía) | Protect-P (gestión del incidente); Communicate-P, categoría CM.AW-P (notificación) |
| 6. Sensibilización | **6.3** Concientización, educación y formación en seguridad de la información | Cláusula **7.3** (concienciación) | Govern-P (cultura organizacional) |
| 7. Monitoreo y Mejora Continua | **5.35** Revisión independiente de seguridad de la información · **5.36** Cumplimiento de políticas, reglas y normas · Cláusulas 9-10 (evaluación de desempeño, mejora) | Cláusula **9** (evaluación de desempeño, 9.1-9.3) y Cláusula **10** (mejora, 10.1-10.2) — misma estructura de alto nivel que ISO 27001 (Anexo SL) | Govern-P, categoría GV.MT-P (Monitoring and Review) |

No cubiertos por ninguna fila de la tabla de 7 procesos, pero ya verificados y disponibles si una
tarea futura los necesita: Anexo **A.1.2.6** (evaluación de impacto en privacidad, EIPD) y Anexo
**A.1.2.8** (controlador conjunto — equivalente ISO al escenario de holding/grupo empresarial con
matriz y filiales como responsables conjuntos, o red de colegios con la misma figura).

## Fuentes de esta tabla
- `sources/complementario/nch-iso-27001-2023-oficial-es.pdf` (+ `.extracto/`, 30 páginas, íntegro) — NCh-ISO/IEC 27001:2023, adopción nacional INN, español.
- `sources/complementario/iso-27001-2022-oficial-en.pdf` (+ `.extracto/`, 26 páginas, íntegro) — ISO/IEC 27001:2022 original, inglés, usado como cruce de respaldo.

## Qué NO cubre este crosswalk
- No mapea la certificación del MPI (Art. 49°) contra ISO — son sistemas de certificación
  independientes, con auditores y organismos distintos; tener ISO 27701 no exime de nada del MPI ni
  viceversa.
- No reemplaza una gap analysis formal de certificación — eso requiere el texto oficial adquirido y,
  normalmente, un auditor líder ISO involucrado.

## Uso recomendado
Si el cliente (colegio, sostenedor o SLEP) ya tiene o está evaluando ISO 27001, mostrar esta tabla
ayuda a argumentar que construir los 7 procesos de este programa **no es trabajo aparte** — es, en
gran medida, el mismo trabajo con otro nombre. Vale como argumento de eficiencia ante quien decide
presupuesto.
