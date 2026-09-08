# Crosswalk — Los 7 procesos × ISO/IEC 27001:2022 (Anexo A) e ISO/IEC 27701:2019

## Aviso de verificación
El texto de las normas ISO es propietario (no está disponible para grep/verificación local como la
ley chilena). Lo que sigue usa la **estructura pública conocida** de ISO 27001:2022 (93 controles del
Anexo A, en 4 temas: Organizacionales, Personas, Físicos, Tecnológicos) e ISO 27701:2019 (extensión de
gestión de privacidad sobre 27001/27002, con requisitos adicionales para PII Controller/Processor).
**Antes de usar este crosswalk en una auditoría de certificación real, contrastar cada número de
control contra el texto oficial adquirido** — el nivel de confianza aquí es "estructura general
correcta", no "cita verbatim verificada" como el resto del programa.

## Por qué vale la pena este crosswalk
Un Excel de auditoría inicial del proyecto (archivado en `../../03_clientes/SLEP_Los_Parques/entregables_historicos/Auditoria - Ley Proteccion y Tratamiento de Datos.xlsx`) ya cita
ISO 27701/27001/NIST/CIS como referencia de buenas prácticas, pero nunca formalizamos la
correspondencia. Sirve para: (a) una organización que ya tiene o busca ISO 27001 puede ver que gran
parte del trabajo de los 7 procesos también sirve para su SGSI, y (b) si más adelante se plantea
certificar el MPI, tener los controles ISO ya mapeados facilita cualquier auditoría externa conjunta.

## Tabla de correspondencia

| Proceso (Ley 19.628 modificada) | Controles ISO 27001:2022 Anexo A (temas) | Extensión ISO 27701:2019 |
|---|---|---|
| 1. Gobernanza e Inventario | A.5.9 Inventario de activos de información · A.5.1 Políticas de seguridad | Cláusula 5.2 — determinar el rol (PII Controller/Processor) e inventario de PII |
| 2. Licitud, Transparencia y Derechos | A.5.34 Privacidad y protección de PII (referencia cruzada directa) | Cláusulas 7.2-7.3 (Controller) / 8.2 (Processor) — bases legales, derechos del titular |
| 3. Datos Sensibles y NNA | A.5.12 Clasificación de la información · A.8.10 Eliminación de información | Anexo A/B de 27701 — categorías especiales de PII, menores de edad |
| 4. Ciclo de Vida y Terceros | A.5.19-A.5.23 Seguridad en relaciones con proveedores · A.8.10 Eliminación | Cláusula 7.2.6/8.2.6 — acuerdos de tratamiento con procesadores (equivalente al DPA) |
| 5. Seguridad y Gestión de Brechas | A.5.24-A.5.28 Gestión de incidentes de seguridad de la información | Cláusula 6.13 (extensión) — notificación de brechas de PII, distinta del incidente de seguridad genérico |
| 6. Sensibilización | A.6.3 Concienciación, educación y capacitación en seguridad de la información | Sin cláusula específica adicional — hereda de 27001 |
| 7. Monitoreo y Mejora Continua | A.5.35-A.5.36 Revisión independiente/cumplimiento · Cláusula 9-10 de ISO 27001 (evaluación de desempeño, mejora) | Cláusula 9 (extensión) — auditoría del sistema de gestión de privacidad |

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
