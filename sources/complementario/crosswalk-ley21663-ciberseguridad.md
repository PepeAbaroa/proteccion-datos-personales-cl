# Crosswalk — Ley 19.628 modificada (protección de datos) × Ley 21.663 (Marco de Ciberseguridad e Infraestructura Crítica)

## Aviso de verificación (léelo antes de usar esto con un cliente)
A diferencia del resto de esta carpeta, **el contenido de este archivo sobre la Ley 21.663 NO está
verificado artículo por artículo contra el texto oficial** — no hay una copia local de esa ley en las
fuentes de la skill `proteccion-datos-personales-cl` (que cubre 19.628/21.719/Reglamento MPI, no
ciberseguridad). Lo que sigue es la estructura general de la ley tal como es públicamente conocida
(promulgada 2024, crea la Agencia Nacional de Ciberseguridad - ANCI). **Antes de citar un artículo
específico de la Ley 21.663 en un documento real, verificarlo contra el texto en bcn.cl/leychile.cl**
— exactamente la misma disciplina que se aplicó al resto de este programa con la Ley 19.628/21.719.

## Por qué son "primas hermanas" y no la misma cosa
Ambas leyes regulan la protección de un activo (datos personales vs. infraestructura/sistemas), ambas
crean una agencia fiscalizadora nueva, y ambas exigen reportar incidentes — pero:
- **Autoridad distinta**: Agencia de Protección de Datos Personales (19.628 modificada) vs. Agencia
  Nacional de Ciberseguridad, ANCI (21.663).
  Verificar cuál corresponde en Chile, y que efectivamente sea la ANCI la que aplica la Ley 21.663.
- **Objeto distinto**: la 19.628 protege al titular del dato (la persona); la 21.663 protege la
  continuidad/integridad de servicios y sistemas — un incidente puede afectar solo sistemas (sin
  datos personales involucrados, activa solo 21.663) o solo datos personales sin comprometer sistemas
  críticos (activa solo 19.628), o ambos a la vez.
- **Sujetos regulados con distinto alcance**: la 21.663 tiene una categoría reforzada de "Operadores
  de Importancia Vital" (OIV) con obligaciones más estrictas — un colegio o sostenedor individual
  probablemente NO califica como OIV (esa categoría apunta a infraestructura crítica nacional: energía,
  telecomunicaciones, salud, financiero, etc.) — **verificar si el sector educación tiene alguna
  categoría regulada específica antes de asumir que no aplica en absoluto.**

## Dónde SÍ se cruzan de verdad (para el Proceso 5 de este programa)
| Situación | Qué exige la Ley 19.628 modificada (ya cubierto en Proceso 5) | Qué probablemente exige la Ley 21.663 (verificar) |
|---|---|---|
| Un ransomware cifra el servidor con datos de estudiantes | Reportar a la Agencia de Protección de Datos "sin dilaciones indebidas" (Art. 14 sexies) + aviso a titulares si aplica | Probablemente reportar también a la ANCI si el sistema afectado calza en el alcance de la ley — **verificar umbral de aplicación** |
| Un proveedor de la plataforma de gestión escolar sufre una brecha | Activa el Proceso 4 (DPA) + Proceso 5 (brecha) igual | Si el proveedor es un "servicio esencial" bajo la 21.663, puede tener su propio deber de reporte independiente del colegio — **verificar** |
| Un ataque de phishing sin acceso efectivo a datos | Puede no activar el deber de reportar de la 19.628 (falta "riesgo razonable" de daño a titulares) | Puede igual ser relevante para gestión de ciberseguridad interna, aunque no haya brecha de datos reportable |

## Recomendación práctica (sin necesidad de verificar cada artículo todavía)
En el **Proceso 5** (`../01_instrumentos_plantilla/05_plantillas_vivas/05_protocolo_respuesta_brechas.md`), agregar como paso de
evaluación una pregunta explícita: *"¿este incidente, además de afectar datos personales, compromete
la continuidad de un sistema o servicio? Si es así, evaluar en paralelo si corresponde reporte bajo la
Ley 21.663, con su propio plazo y autoridad — no asumir que un solo reporte cubre ambas leyes."* Esto
ya se puede instalar como buena práctica sin tener verificado el detalle fino del articulado.

## Pendiente real
Verificación completa de la Ley 21.663 con el mismo estándar que el resto de este programa (extracción
total del texto oficial, mapa de artículos verificado) — no se hizo esta noche porque no hay fuente
local y el foco de la sesión era la Ley 19.628/21.719. Si se va a usar este cruce con un cliente real,
es un prerequisito antes de citar un artículo específico de la 21.663.
