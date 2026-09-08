# Mapa de artículos — Ley 21.719 (texto literal + razonamiento aplicado)

> Verificado contra `sources/especifico/ley-21719-texto.txt` (extraído del PDF oficial BCN/leychile.cl,
> 56/56 páginas íntegras) y, para el Título III, contra `sources/especifico/ley-19628-original-texto.txt`
> (13/13 páginas). La Ley 21.719 opera como una batería de modificaciones a la Ley 19.628 — el texto
> vigente desde el 1-dic-2026 es la Ley 19.628 con estos artículos reemplazados/insertados. Toda cita de
> artículo de aquí en adelante es a la Ley 19.628 ya modificada, salvo que se diga lo contrario.
>
> **Formato de este archivo**: cada artículo trae dos bloques — `TEXTO LITERAL` (cita exacta copiada del
> archivo fuente, sin parafrasear) y `Razonamiento aplicado` (interpretación, cruces con otros artículos,
> implicancia práctica — esto sí es criterio de esta skill, no texto de la ley). Nunca se mezclan sin
> etiqueta. Para artículos de pura organización interna de la Agencia (Título VI, gran parte) el
> razonamiento es breve porque no hay mucho que interpretar más allá de la estructura misma.

---

## Título I — Objeto, ámbito de aplicación y definiciones

### Artículo 1° — Objeto y ámbito de aplicación
> **TEXTO LITERAL** (Art. 1°, sources/especifico/ley-21719-texto.txt líneas 38-56)
> "Objeto y ámbito de aplicación. La presente ley tiene por objeto regular la forma y condiciones en la
> cual se efectúa el tratamiento y protección de los datos personales de las personas naturales, en
> conformidad al artículo 19, N° 4, de la Constitución Política de la República.
> Todo tratamiento de datos personales que realice una persona natural o jurídica, incluidos los órganos
> públicos, debe respetar los derechos y libertades de las personas y quedará sujeto a las disposiciones
> de esta ley.
> El régimen de tratamiento y protección de datos establecido en esta ley no se aplicará al tratamiento
> de datos que se realice en el ejercicio de las libertades de emitir opinión y de informar reguladas por
> las leyes a que se refiere el artículo 19, N° 12, de la Constitución Política de la República. Los
> medios de comunicación social quedarán sujetos a las disposiciones de esta ley en lo relativo al
> tratamiento de datos que efectúen con una finalidad distinta a la de opinar e informar.
> Tampoco serán aplicables las normas de la presente ley al tratamiento de datos que efectúen las
> personas naturales en relación con sus actividades personales."

**Razonamiento aplicado:** tres exclusiones expresas de ámbito: (1) libertad de opinar/informar (prensa
en su rol editorial, no en su rol de tratador comercial de datos — un medio que vende bases de datos de
suscriptores sí queda sujeto), (2) actividades estrictamente personales (ej. agenda de contactos de un
privado), (3) implícita: solo personas naturales son "titulares" — datos de personas jurídicas quedan
fuera. Para SLEP/colegios, ninguna exclusión aplica: el tratamiento de datos de alumnos/funcionarios es
"órgano público" tratando datos con fines institucionales, no opinar/informar ni actividad personal.

### Artículo 1° bis — Ámbito de aplicación territorial
> **TEXTO LITERAL** (Art. 1° bis, líneas 71-96)
> "Las disposiciones de la presente ley se aplicarán al tratamiento de datos personales que se realice
> bajo cualquiera de las siguientes circunstancias:
> a) Cuando el responsable o mandatario estén establecidos o constituidos en el territorio nacional.
> b) Cuando el mandatario, con independencia de su lugar de establecimiento o constitución, realice las
> operaciones de tratamiento de datos personales a nombre de un responsable establecido o constituido en
> el territorio nacional.
> c) Cuando el responsable o mandatario no se encuentren establecidos en el territorio nacional pero sus
> operaciones de tratamiento de datos personales estén destinadas a ofrecer bienes o servicios a titulares
> que se encuentren en Chile, independientemente de si a éstos se les requiere un pago, o a monitorear el
> comportamiento de titulares que se encuentran en el territorio nacional, incluyendo su análisis,
> rastreo, perfilamiento o predicción de comportamiento.
> La presente ley también se aplicará al tratamiento de datos personales que sea realizado por un
> responsable al que, sin estar establecido en el territorio nacional, le resulte aplicable la
> legislación nacional a causa de un contrato o del derecho internacional."

**Razonamiento aplicado:** extraterritorialidad tipo RGPD Art. 3 pero no idéntica — la letra c) cubre
tanto ofrecer bienes/servicios como monitorear comportamiento (analytics, tracking web). Relevante para
cualquier SaaS extranjero (Google Workspace, Microsoft 365, plataformas de evaluación educativa
extranjeras) que trate datos de alumnos/apoderados chilenos: aunque el proveedor no tenga oficina en
Chile, si ofrece el servicio a usuarios en Chile queda sujeto a esta ley igual que a su propia
jurisdicción — no es excusa para el responsable chileno delegar el cumplimiento en el proveedor extranjero.

### Artículo 2° — Definiciones
> **TEXTO LITERAL** (Art. 2° letras clave, líneas 106-267)
> "a) Almacenamiento de datos: la conservación o custodia de datos en un registro o base de datos.
> c) Comunicación de datos personales: dar a conocer por el responsable de datos, de cualquier forma,
> datos personales a personas distintas del titular a quien conciernen los datos, sin llegar a cederlos
> o transferirlos.
> f) Dato personal: cualquier información vinculada o referida a una persona natural identificada o
> identificable. Se considerará identificable toda persona cuya identidad pueda determinarse, directa o
> indirectamente, en particular mediante uno o más identificadores, tales como el nombre, el número de
> cédula de identidad, el análisis de elementos propios de la identidad física, fisiológica, genética,
> psíquica, económica, cultural o social de dicha persona. Para determinar si una persona es identificable
> deberán considerarse todos los medios y factores objetivos que razonablemente se podrían usar para dicha
> identificación en el momento del tratamiento.
> g) Datos personales sensibles: tendrán esta condición aquellos datos personales que se refieren a las
> características físicas o morales de las personas o a hechos o circunstancias de su vida privada o
> intimidad, que revelen el origen étnico o racial, la afiliación política, sindical o gremial, la
> situación socioeconómica, las convicciones ideológicas o filosóficas, las creencias religiosas, los
> datos relativos a la salud, al perfil biológico humano, los datos biométricos, y la información
> relativa a la vida sexual, a la orientación sexual y a la identidad de género de una persona natural.
> i) Fuentes de acceso público: todas aquellas bases de datos o conjuntos de datos personales, cuyo
> acceso o consulta puede ser efectuada en forma lícita por cualquier persona, tales como el Diario
> Oficial, medios de comunicación o los registros públicos que disponga la ley. El tratamiento de datos
> personales provenientes de fuentes de acceso público se someterá a las disposiciones de esta ley.
> k) Anonimización: procedimiento irreversible en virtud del cual un dato personal no puede vincularse o
> asociarse a una persona determinada, ni permitir su identificación, por haberse destruido o eliminado
> el nexo con la información que vincula, asocia o identifica a esa persona. Un dato anonimizado deja de
> ser un dato personal.
> l) Seudonimización: tratamiento de datos personales que se efectúa de manera tal que ya no puedan
> atribuirse a un titular sin utilizar información adicional, siempre que dicha información adicional
> figure por separado y esté sujeta a medidas técnicas y organizativas destinadas a garantizar que los
> datos personales no se atribuyan a una persona natural identificada o identificable.
> n) Responsable de datos o responsable: toda persona natural o jurídica, pública o privada, que decide
> acerca de los fines y medios del tratamiento de datos personales, con independencia de si los datos son
> tratados directamente por ella o a través de un tercero mandatario o encargado.
> p) Consentimiento: toda manifestación de voluntad libre, específica, inequívoca e informada, otorgada a
> través de una declaración o una clara acción afirmativa, mediante la cual el titular de datos, su
> representante legal o mandatario, según corresponda, autoriza el tratamiento de los datos personales
> que le conciernen.
> w) Elaboración de perfiles: toda forma de tratamiento automatizado de datos personales que consista en
> utilizar esos datos para evaluar, analizar o predecir aspectos relativos al rendimiento profesional,
> situación económica, de salud, preferencias personales, intereses, fiabilidad, comportamiento, ubicación
> o movimientos de una persona natural.
> x) Tercero mandatario o encargado: la persona natural o jurídica que trate datos personales, por cuenta
> del responsable de datos."

**Razonamiento aplicado:** tres puntos de aplicación práctica frecuente. (1) "Dato personal" (f) es
amplísimo — incluye cualquier dato "identificable" indirectamente, no solo nombre/RUT: una nota de
evaluación cruzada con curso+fecha ya identifica a un alumno específico. (2) La lista de "sensibles" (g)
incluye **situación socioeconómica** — esto es clave para SLEP/colegios: los datos de clasificación
SEP/prioritario-preferente y las fichas de becas JUNAEB son datos sensibles por definición legal, no una
categoría aparte inventada por la práctica. (3) "Responsable" (n) vs. "tercero mandatario/encargado" (x)
es la distinción DPA: un proveedor cloud (Microsoft, Google) que solo procesa por instrucción del
colegio es "encargado", no "responsable" — pero si decide fines propios (ej. usa los datos para entrenar
sus propios modelos sin instrucción del colegio) pasa a ser responsable con responsabilidad propia
(ver Art. 15 bis).

### Artículo 3° — Principios
> **TEXTO LITERAL** (Art. 3°, líneas 271-343)
> "El tratamiento de los datos personales se rige por los siguientes principios:
> a) Principios de licitud y lealtad. Los datos personales sólo pueden tratarse de manera lícita y leal.
> El responsable deberá ser capaz de acreditar la licitud del tratamiento de datos personales que realiza.
> b) Principio de finalidad. Los datos personales deben ser recolectados con fines específicos, explícitos
> y lícitos. El tratamiento de los datos personales debe limitarse al cumplimiento de estos fines. [...]
> no se pueden tratar los datos personales con fines distintos a los informados al momento de la
> recolección, salvo que el tratamiento sea para fines compatibles con los autorizados originalmente; que
> exista una relación contractual o precontractual [...]; que el titular otorgue nuevamente su
> consentimiento, y cuando lo disponga la ley.
> c) Principio de proporcionalidad. Los datos personales que se traten deben limitarse estrictamente a
> aquéllos que resulten necesarios, adecuados y pertinentes en relación con los fines del tratamiento.
> Los datos personales pueden ser conservados sólo por el período de tiempo que sea necesario para
> cumplir con los fines del tratamiento, luego de lo cual deben ser suprimidos o anonimizados [...]
> d) Principio de calidad. Los datos personales deben ser exactos, completos, actuales y pertinentes en
> relación con su proveniencia y los fines del tratamiento.
> e) Principio de responsabilidad. Quienes realicen tratamiento de los datos personales serán legalmente
> responsables del cumplimiento de los principios contenidos en este artículo y de las obligaciones y
> deberes de conformidad a la ley.
> f) Principio de seguridad. [...] el responsable debe garantizar estándares adecuados de seguridad,
> protegiéndolos contra el tratamiento no autorizado o ilícito, y contra su pérdida, filtración, daño
> accidental o destrucción. [...]
> g) Principio de transparencia e información. El responsable debe entregar al titular toda la
> información que sea necesaria para el ejercicio de los derechos que establece esta ley [...]
> h) Principio de confidencialidad. El responsable de datos personales y quienes tengan acceso a ellos
> deberán guardar secreto o confidencialidad acerca de los mismos. [...] Este deber subsiste aún después
> de concluida la relación con el titular."

**Razonamiento aplicado:** son 8 principios (a la letra h), un más que el listado habitual de 7 de otros
regímenes — la novedad chilena es tratar **confidencialidad** (h) como principio autónomo, no solo como
deber derivado. Los principios son el estándar contra el cual se mide toda infracción (Art. 34): cada
inciso del Art. 3° corresponde a una categoría de infracción posible. Para auditoría práctica: (b)
finalidad + (c) proporcionalidad son los que más frecuentemente falla un colegio que reutiliza datos
recolectados para matrícula en usos no informados (ej. marketing de servicios extracurriculares) sin
nuevo consentimiento ni compatibilidad de fines.

---

## Título I — De los derechos del titular de datos personales (Arts. 4-11)

### Artículo 4° — Derechos del titular de datos
> **TEXTO LITERAL** (Art. 4°, líneas 350-365)
> "Toda persona, actuando por sí o a través de su representante legal o mandatario, según corresponda,
> tiene derecho de acceso, rectificación, supresión, oposición, portabilidad y bloqueo de sus datos
> personales, de conformidad a la presente ley. Tales derechos son personales, intransferibles e
> irrenunciables y no pueden limitarse por ningún acto o convención. En caso de fallecimiento del titular
> de datos, los derechos que reconoce esta ley pueden ser ejercidos por sus herederos. Con todo, los
> herederos no podrán acceder a los datos del causante, ni solicitar su rectificación o supresión, cuando
> la persona fallecida lo hubiese prohibido expresamente o así lo establezca una ley."

**Razonamiento aplicado:** 6 derechos (no 5): acceso, rectificación, supresión, oposición, portabilidad
y **bloqueo** — el bloqueo (Art. 8° ter) suele olvidarse en resúmenes previos a esta ley. Son
irrenunciables: una cláusula contractual que diga "el titular renuncia a ejercer sus derechos ARCO+"
sería nula. La extensión a herederos es relevante para el caso de un funcionario o alumno fallecido: el
colegio/SLEP debe evaluar si hay prohibición expresa antes de negar acceso a herederos.

### Artículo 5° — Derecho de acceso
> **TEXTO LITERAL** (Art. 5°, líneas 367-399)
> "El titular de datos tiene derecho a solicitar y obtener del responsable, confirmación acerca de si los
> datos personales que le conciernen están siendo tratados por él, y en tal caso, acceder a dichos datos
> y a la siguiente información: a) Los datos tratados y su origen. b) La finalidad o finalidades del
> tratamiento. c) Las categorías, clases o tipos de destinatarios [...] d) El período de tiempo durante
> el cual los datos serán tratados. e) Los intereses legítimos del responsable, cuando el tratamiento se
> base en lo dispuesto en el artículo 13, letra d). f) La información significativa sobre la lógica
> aplicada en el caso de que el responsable realice tratamiento de datos de conformidad con el artículo
> 8° bis. El responsable siempre estará obligado a entregar información y a dar acceso a los datos
> solicitados excepto cuando una ley disponga expresamente lo contrario."

**Razonamiento aplicado:** acceso no es solo "ver mis datos" — obliga a explicar origen, finalidad,
destinatarios, plazo y (si aplica) la lógica de decisiones automatizadas. La única excusa válida para
negar acceso es una ley que expresamente lo prohíba (ej. secreto de investigación penal Art. 24) — no
basta una política interna del responsable.

### Artículo 6° — Derecho de rectificación
> **TEXTO LITERAL** (Art. 6°, líneas 401-412)
> "El titular de datos tiene derecho a solicitar y obtener del responsable, la rectificación de los datos
> personales que le conciernen y que están siendo tratados por él, cuando sean inexactos, desactualizados
> o incompletos. Los datos rectificados deberán ser comunicados a las personas, entidades u organismos a
> los cuales el responsable haya comunicado o cedido los referidos datos, salvo en los casos en que dicha
> comunicación sea imposible o exija un esfuerzo desproporcionado. Efectuada la rectificación, no se
> podrán volver a tratar los datos sin rectificar."

**Razonamiento aplicado:** obligación en cascada — si el colegio cedió el dato erróneo a MINEDUC/SIGE,
debe notificar la corrección salvo imposibilidad o esfuerzo desproporcionado (estándar que la Agencia
aún no ha reglamentado con precisión numérica, se aplica caso a caso).

### Artículo 7° — Derecho de supresión
> **TEXTO LITERAL** (Art. 7°, líneas 414-451)
> "El titular de datos tiene derecho a solicitar y obtener del responsable, la eliminación de los datos
> personales que le conciernen, en los siguientes casos: a) Cuando los datos no resulten necesarios en
> relación con los fines del tratamiento [...] b) Cuando el titular haya revocado su consentimiento [...]
> c) Cuando los datos hayan sido obtenidos o tratados ilícitamente [...] d) Cuando se trate de datos
> caducos. e) Cuando los datos deban suprimirse para el cumplimiento de una sentencia judicial [...] f)
> Cuando el titular haya ejercido su derecho de oposición [...] No procede la supresión cuando el
> tratamiento sea necesario: i. Para ejercer el derecho a las libertades de emitir opinión y de informar.
> ii. Para el cumplimiento de una obligación legal o la ejecución de un contrato [...] iii. Para el
> cumplimiento de una función pública o para el ejercicio de una actividad de interés público. iv. Por
> razones de interés público en el área de la salud pública [...] v. Para tratamientos con fines
> históricos, estadísticos o científicos [...] vi. Para la formulación, ejercicio o defensa de una
> reclamación administrativa o judicial."

**Razonamiento aplicado:** un SLEP/colegio puede **rechazar legítimamente** una solicitud de supresión
del expediente académico de un exalumno invocando la excepción (ii) — obligación legal de conservar
registros escolares — o (iii) función pública. No es automática la obligación de borrar todo lo que se
pida; hay que fundar en cuál excepción aplica antes de negar.

### Artículo 8° — Derecho de oposición
> **TEXTO LITERAL** (Art. 8°, líneas 453-486)
> "El titular de datos tiene derecho a oponerse ante el responsable a que se realice un tratamiento
> específico o determinado [...] a) Cuando la base de licitud del tratamiento sea la satisfacción de
> intereses legítimos del responsable [...] b) Si el tratamiento se realiza exclusivamente con fines de
> mercadotecnia o marketing directo [...] c) Si el tratamiento se realiza respecto de datos obtenidos de
> una fuente de acceso público y no existe otro fundamento legal para su tratamiento. No procederá la
> oposición al tratamiento cuando éste se realice con fines de investigación científica o histórica o
> fines estadísticos, y siempre que fueran necesarios para el cumplimiento de una función pública [...]"

**Razonamiento aplicado:** la oposición por marketing directo (letra b) es de ejercicio **absoluto** —
no exige justificación del titular ni admite ponderación del responsable (a diferencia de la letra a,
donde el responsable puede resistir acreditando "motivos legítimos imperiosos").

### Artículo 8° bis — Decisiones individuales automatizadas
> **TEXTO LITERAL** (Art. 8° bis, líneas 488-515)
> "El titular de datos tiene derecho a oponerse y a no ser objeto de decisiones basadas en el tratamiento
> automatizado de sus datos personales, incluida la elaboración de perfiles, que produzca efectos
> jurídicos en él o le afecte significativamente. El inciso anterior no se aplicará en los siguientes
> casos: a) Cuando la decisión sea necesaria para la celebración o ejecución de un contrato [...] b)
> Cuando exista consentimiento previo y expreso del titular [...] c) Cuando lo señale la ley [...] En
> todos los casos [...] el responsable deberá adoptar las medidas necesarias para asegurar los derechos y
> libertades del titular, su derecho a la información y transparencia, el derecho a obtener una
> explicación, a la intervención humana, a expresar su punto de vista y a solicitar la revisión de la
> decisión."

**Razonamiento aplicado:** directamente aplicable a cualquier sistema de IA/scoring que un SLEP use para
clasificar riesgo de deserción, priorizar becas o evaluar postulantes — si la decisión "afecta
significativamente" y es automatizada sin intervención humana real, el titular tiene derecho a
explicación e intervención humana aunque exista base legal para el tratamiento subyacente. Es un derecho
distinto y adicional, no sustituido por tener una base de licitud del Art. 12-13.

### Artículo 8° ter — Derecho de bloqueo del tratamiento
> **TEXTO LITERAL** (Art. 8° ter, líneas 516-535)
> "El titular de datos tiene derecho a solicitar la suspensión temporal de cualquier operación de
> tratamiento de sus datos personales cuando formule una solicitud de rectificación, supresión u
> oposición [...] mientras dicha solicitud no se resuelva. [...] El ejercicio de este derecho no
> afectará el almacenamiento de los datos por parte del responsable."

**Razonamiento aplicado:** el bloqueo es cautelar, no definitivo — congela el uso activo del dato
mientras se resuelve el fondo, pero el responsable puede seguirlo almacenando (no está obligado a
borrarlo durante el bloqueo).

### Artículo 9° — Derecho a la portabilidad
> **TEXTO LITERAL** (Art. 9°, líneas 537-563)
> "El titular de datos tiene derecho a solicitar y recibir una copia de los datos personales que le
> conciernen [...] en un formato electrónico estructurado, genérico y de uso común [...] cuando concurran
> las siguientes circunstancias: a) El tratamiento se realice en forma automatizada, y b) El tratamiento
> esté basado en el consentimiento del titular. [...] Con todo, el ejercicio del derecho de portabilidad
> no supondrá la supresión de los datos ante el responsable cedente, a menos que el titular de ellos así
> lo pida conjuntamente en la solicitud."

**Razonamiento aplicado:** portabilidad tiene requisito doble acumulativo (automatizado + basado en
consentimiento) — no aplica a tratamientos basados en obligación legal o interés legítimo, que es la
base típica de datos escolares/administrativos de un SLEP (Art. 20, órganos públicos no requieren
consentimiento). En la práctica, portabilidad rara vez opera contra un órgano público por esta razón.

### Artículo 10 — Forma y medios de ejercer los derechos
> **TEXTO LITERAL** (Art. 10, líneas 565-612)
> "[...] Los responsables de datos deberán implementar mecanismos y herramientas tecnológicas que
> permitan que el titular ejerza sus derechos en forma expedita, ágil y eficaz. [...] El ejercicio de los
> derechos de rectificación, supresión y oposición siempre serán gratuitos para el titular. El derecho de
> acceso también se ejercerá en forma gratuita, al menos trimestralmente. [...]"

**Razonamiento aplicado:** gratuidad es la regla — cobro solo procede si el titular ejerce acceso o
portabilidad más de una vez por trimestre, y el monto lo fija la Agencia por instrucción general (aún no
dictada a la fecha de verificación de esta skill).

### Artículo 11 — Procedimiento ante el responsable de datos
> **TEXTO LITERAL** (Art. 11, líneas 614-701)
> "[...] Recibida la solicitud el responsable deberá acusar recibo de ella y pronunciarse a más tardar
> dentro de los treinta días corridos siguientes a la fecha de ingreso de la solicitud. Este plazo podrá
> ser prorrogado, por una sola vez, hasta por treinta días corridos. [...] En caso de denegación total o
> parcial de la solicitud, el responsable deberá fundar su decisión [...] señalar al titular que dispone
> de un plazo de treinta días hábiles para formular una reclamación ante la Agencia [...] Cuando se
> formule una solicitud de rectificación, supresión u oposición, el titular tendrá derecho a solicitar y
> obtener del responsable el bloqueo temporal [...] el responsable deberá responder al requerimiento
> dentro de los dos días hábiles siguientes a su recepción."

**Razonamiento aplicado:** los plazos operativos clave para cualquier procedimiento interno ARCO+ de un
SLEP: **30 días corridos** para responder (prorrogable una vez por 30 más) y **2 días hábiles** para
responder una solicitud de bloqueo temporal — este último plazo corto suele omitirse en protocolos
internos que solo contemplan el de 30 días.

---

## Título II — Del tratamiento de los datos personales (Párrafo 1°, Arts. 12-15 ter)

### Artículo 12 — Regla general del tratamiento de datos (consentimiento)
> **TEXTO LITERAL** (Art. 12, líneas 714-756)
> "Es lícito el tratamiento de los datos personales que le conciernen al titular, cuando otorgue su
> consentimiento para ello. El consentimiento del titular debe ser libre, informado y específico en
> cuanto a su finalidad o finalidades. [...] Se presume que el consentimiento para tratar datos no ha
> sido libremente otorgado cuando el responsable lo recaba en el marco de la ejecución de un contrato o
> la prestación de un servicio en que no es necesario efectuar esa recolección. [...] Corresponde al
> responsable probar que contó con el consentimiento del titular y que el tratamiento de datos fue
> realizado en forma lícita, leal y transparente."

**Razonamiento aplicado:** la carga de la prueba de la licitud recae SIEMPRE en el responsable, nunca en
el titular — este es el fundamento legal directo de la "carga de la prueba invertida" ya aplicada en el
ejemplo del teléfono del director (ver `sources/complementario` pendiente de validación,
`02_casos_referencia/21_caso_compuesto.md`). La presunción de consentimiento viciado en contratos de
adhesión es relevante para cualquier formulario de matrícula que pida consentimiento para fines no
esenciales al servicio educativo.

### Artículo 13 — Otras fuentes de licitud del tratamiento
> **TEXTO LITERAL** (Art. 13, líneas 758-786)
> "Es lícito el tratamiento de datos personales, sin el consentimiento del titular, en los siguientes
> casos: a) Cuando el tratamiento esté referido a datos relativos a obligaciones de carácter económico,
> financiero, bancario o comercial y se realice de conformidad con las normas del Título III de esta ley
> [...] b) Cuando el tratamiento sea necesario para la ejecución o el cumplimiento de una obligación
> legal o lo disponga la ley. c) Cuando el tratamiento de datos sea necesario para la celebración o
> ejecución de un contrato entre el titular y el responsable [...] d) Cuando el tratamiento sea necesario
> para la satisfacción de intereses legítimos del responsable o de un tercero, siempre que con ello no se
> afecten los derechos y libertades del titular. [...] e) Cuando el tratamiento de datos sea necesario
> para la formulación, ejercicio o defensa de un derecho ante los tribunales de justicia u órganos
> públicos. El responsable deberá acreditar la licitud del tratamiento de datos."

**Razonamiento aplicado:** son 5 bases de licitud alternativas al consentimiento — la base típica de un
SLEP para tratar datos de alumnos/apoderados es la letra b) (obligación legal, ej. Ley 21.040, normativa
MINEDUC) o excepcionalmente d) (interés legítimo, con ponderación exigible frente al titular). Elegir la
base correcta desde el inicio (y no "consentimiento" por defecto cuando en realidad hay obligación legal)
evita la trampa de tener que gestionar revocaciones de consentimiento sobre datos que la ley igual obliga
a tratar.

### Artículo 14 — Obligaciones del responsable de datos
> **TEXTO LITERAL** (Art. 14, líneas 788-823)
> "El responsable de datos [...] tiene las siguientes obligaciones: a) Informar y poner a disposición del
> titular los antecedentes que acrediten la licitud del tratamiento [...] b) Asegurar que los datos
> personales se recojan de fuentes de acceso lícitas con fines específicos, explícitos y lícitos [...] c)
> Comunicar o ceder [...] información exacta, completa y actual. d) Suprimir o anonimizar los datos
> personales del titular cuando fueron obtenidos para la ejecución de medidas precontractuales. e)
> Cumplir con los demás deberes, principios y obligaciones [...]"

**Razonamiento aplicado:** obligación (a) —poder acreditar la licitud "cuando le sea requerida"— es la
base operativa de mantener un Registro de Actividades de Tratamiento (RAT): sin RAT, un responsable no
puede cumplir materialmente esta obligación cuando la Agencia o un titular se lo exija.

### Artículo 14 bis — Deber de secreto o confidencialidad
> **TEXTO LITERAL** (Art. 14 bis, líneas 825-853)
> "El responsable de datos está obligado a mantener secreto o confidencialidad acerca de los datos
> personales que conciernan a un titular, salvo cuando el titular los hubiere hecho manifiestamente
> públicos. Este deber subsiste aún después de concluida la relación con el titular. En caso de que el
> responsable haya realizado alguna acción sobre datos personales obtenidos de fuentes de acceso público,
> tales como organizarlos o clasificarlos bajo algún criterio, o combinarlos o complementarlos con otros
> datos, los datos personales que resulten de dicha acción se encontrarán protegidos bajo el presente
> deber de secreto o confidencialidad."

**Razonamiento aplicado:** incluso datos de fuente pública (ej. Diario Oficial) quedan protegidos por
secreto una vez que el responsable los organiza/cruza con otra información — "agregación crea
protección" aunque las piezas individuales fueran públicas. Esto es exactamente el fundamento legal del
ejemplo del teléfono del director: cruzar un dato público con contexto adicional genera un dato personal
protegido nuevo.

### Artículo 14 ter — Deber de información y transparencia
> **TEXTO LITERAL** (Art. 14 ter, líneas 855-915)
> "El responsable de datos debe facilitar y mantener permanentemente a disposición del público [...] al
> menos, la siguiente información: a) La política de tratamiento de datos personales [...] b) La
> individualización del responsable [...] y la identificación del encargado de prevención, si existiere.
> c) El domicilio postal, la dirección de correo electrónico [...] d) Las categorías [...] de datos que
> trata [...] e) La política y las medidas de seguridad adoptadas [...] f) El derecho que le asiste al
> titular [...] g) El derecho [...] de recurrir ante la Agencia [...] h) En su caso, la transferencia de
> datos personales a un tercer país [...] i) El periodo durante el que se conservarán los datos [...] j)
> La fuente de la cual provienen [...] k) [...] la existencia del derecho a retirarlo en cualquier
> momento [...] l) La existencia de decisiones automatizadas [...]"

**Razonamiento aplicado:** son 12 elementos mínimos de una política de privacidad publicada — este
artículo es, en la práctica, el checklist obligatorio de contenido de la política de privacidad que
`compliance-cl` debe generar; cualquier política que omita uno de estos 12 puntos es incompleta frente a
esta ley, no solo "mejorable".

### Artículo 14 quáter — Deber de protección desde el diseño y por defecto
> **TEXTO LITERAL** (Art. 14 quáter, líneas 916-940)
> "Con la finalidad de cumplir los principios y los derechos de los titulares [...] el responsable debe
> aplicar medidas técnicas y organizativas adecuadas desde el diseño con anterioridad y durante el
> tratamiento [...] Asimismo, el responsable de datos deberá aplicar medidas técnicas y organizativas
> para garantizar que, por defecto, sólo sean objeto de tratamiento los datos personales específicos y
> estrictamente necesarios para dicha actividad."

**Razonamiento aplicado:** privacy by design/default — aplicable directamente al diseño de cualquier
formulario o sistema nuevo (matrícula, encuestas, apps): la configuración por defecto debe minimizar
campos recolectados, no maximizar "por si sirve después" (choca con proporcionalidad del Art. 3° letra c).

### Artículo 14 quinquies — Deber de adoptar medidas de seguridad
> **TEXTO LITERAL** (Art. 14 quinquies, líneas 942-981)
> "El responsable de datos debe adoptar las medidas necesarias para resguardar el cumplimiento del
> principio de seguridad [...] Las medidas aplicadas [...] deben asegurar la confidencialidad,
> integridad, disponibilidad y resiliencia de los sistemas [...] que en su caso incluya, entre otros: a)
> La seudonimización y el cifrado de datos personales. b) La capacidad de garantizar la confidencialidad,
> integridad, disponibilidad y resiliencia permanentes [...] c) La capacidad de restaurar la
> disponibilidad y el acceso [...] de forma rápida en caso de incidente [...] d) Un proceso de
> verificación, evaluación y valoración regulares [...] Ante la ocurrencia de un incidente de seguridad,
> y en caso de controversia judicial o administrativa, corresponderá al responsable acreditar la
> existencia y el funcionamiento de las medidas de seguridad adoptadas [...]"

**Razonamiento aplicado:** este artículo es el puente directo hacia `infraestructura-ciberseguridad` —
cifrado, seudonimización, disponibilidad/resiliencia y planes de recuperación no son "buenas prácticas
opcionales" sino contenido mínimo exigido por ley, y la carga de la prueba de que existían es del
responsable ante cualquier incidente.

### Artículo 14 sexies — Deber de reportar vulneraciones (brechas)
> **TEXTO LITERAL** (Art. 14 sexies, líneas 983-1022)
> "El responsable deberá reportar a la Agencia, por los medios más expeditos posibles y sin dilaciones
> indebidas, las vulneraciones a las medidas de seguridad que ocasionen la destrucción, filtración,
> pérdida o alteración accidental o ilícita de los datos personales que trate o la comunicación o acceso
> no autorizados a dichos datos, cuando exista un riesgo razonable para los derechos y libertades de los
> titulares. El responsable deberá registrar estas comunicaciones [...] Cuando dichas vulneraciones se
> refieran a datos personales sensibles, datos relativos a niños y niñas menores de catorce años o datos
> relativos a obligaciones de carácter económico, financiero, bancario o comercial, el responsable deberá
> también efectuar esta comunicación a los titulares de estos datos [...] Esta comunicación deberá
> realizarse en un lenguaje claro y sencillo [...] La notificación se deberá realizar a cada titular
> afectado y si ello no fuere posible, se realizará mediante la difusión o publicación de un aviso en un
> medio de comunicación social masivo y de alcance nacional."

**Razonamiento aplicado:** confirma lo ya verificado en la skill — el estándar es "sin dilaciones
indebidas", **no 72 horas** (eso es GDPR, no ley chilena; no citar 72h como si fuera la regla local).
Aviso directo al titular obligatorio en 3 escenarios: datos sensibles, niños menores de 14, o datos
económico/financiero/bancario/comercial — para un SLEP, una brecha que afecte datos de salud/PIE (siempre
sensibles) o de alumnos menores de 14 años dispara automáticamente el deber de aviso individual, no solo
el reporte a la Agencia.

### Artículo 14 septies — Diferenciación de estándares de cumplimiento
> **TEXTO LITERAL** (Art. 14 septies, líneas 1024-1040)
> "Los estándares o condiciones mínimas que se impongan al responsable de datos para el cumplimiento de
> los deberes de información y de seguridad establecidos en los artículos 14 ter y 14 quinquies [...]
> serán determinados considerando el tipo de dato [...], si el responsable es una persona natural o
> jurídica, el tamaño de la entidad [...], la actividad que desarrolla y el volumen, naturaleza y las
> finalidades de los datos personales que trata. [...] serán determinados por la Agencia mediante
> instrucción general."

**Razonamiento aplicado:** el estándar de seguridad/información NO es uniforme — es proporcional al
tamaño/tipo de responsable. Falta la instrucción general de la Agencia que fije el detalle; hasta que se
dicte, el estándar mínimo se interpreta con criterio de proporcionalidad razonable, no exigiendo a un
colegio pequeño el mismo nivel que a un banco.

### Artículo 15 — Cesión de datos personales
> **TEXTO LITERAL** (Art. 15, líneas 1042-1083)
> "Los datos personales podrán ser cedidos con el consentimiento del titular y para el cumplimiento de
> los fines del tratamiento. También se podrán ceder [...] cuando la cesión sea necesaria para el
> cumplimiento y la ejecución de un contrato [...]; cuando exista un interés legítimo [...]; y cuando lo
> disponga la ley. [...] La cesión de datos deberá constar por escrito o a través de cualquier medio
> electrónico idóneo. [...] Una vez perfeccionada la cesión, el cesionario adquiere la condición de
> responsable de datos para todos los efectos legales. [...] Si se verifica una cesión de datos sin contar
> con el consentimiento del titular, siendo éste necesario, la cesión será nula, debiendo el cesionario
> suprimir todos los datos recibidos [...]"

**Razonamiento aplicado:** cesión ≠ tratamiento por encargado (Art. 15 bis) — en la cesión, el receptor
se vuelve responsable propio e independiente; en el encargo, el tercero sigue actuando por cuenta del
responsable original. Confundir ambas figuras en un contrato con un proveedor (ej. tratarlo como "cesión"
cuando en realidad es un encargo de tratamiento) cambia completamente el régimen de responsabilidad
aplicable.

### Artículo 15 bis — Tratamiento a través de tercero mandatario o encargado (DPA)
> **TEXTO LITERAL** (Art. 15 bis, líneas 1085-1141)
> "El responsable puede efectuar el tratamiento de datos en forma directa o a través de un tercero
> mandatario o encargado. En este último caso, el tercero [...] realiza el tratamiento [...] conforme al
> encargo y a las instrucciones que le imparta el responsable, quedándole prohibido su tratamiento para
> un objeto distinto del convenido [...] Si el tercero [...] trata los datos con un objeto distinto del
> encargo convenido o los cede o entrega sin haber sido autorizado [...], se le considerará como
> responsable de datos para todos los efectos legales, debiendo responder personalmente por las
> infracciones [...] y solidariamente con el responsable de datos por los daños ocasionados [...] El
> tratamiento [...] se regirá por el contrato celebrado [...] En el contrato se deberá establecer el
> objeto del encargo, la duración [...], la finalidad del tratamiento, el tipo de datos personales
> tratados, las categorías de titulares [...] y los derechos y obligaciones de las partes. El encargado no
> podrá delegar parte o la totalidad del encargo, salvo [...] autorización específica y por escrito [...]
> La Agencia pondrá a disposición del público modelos tipo de contratos [...] El tercero [...] deberá
> cumplir con lo dispuesto en los artículos 14 bis y 14 quinquies. [...] Cumplida la prestación [...] los
> datos [...] deben ser suprimidos o devueltos al responsable [...]"

**Razonamiento aplicado:** este es el fundamento legal completo del contrato DPA (Data Processing
Agreement) exigido a todo proveedor cloud/tercero que procese datos por cuenta del SLEP/colegio —
contenido mínimo obligatorio del contrato: objeto, duración, finalidad, tipo de datos, categorías de
titulares, derechos/obligaciones, prohibición de subdelegación sin autorización escrita, deber de
suprimir/devolver datos al término. Si el proveedor se excede del encargo, pasa a responder como
responsable propio Y solidariamente con el responsable original — el DPA no blinda al colegio de
responsabilidad solidaria, solo ordena el reparto interno de responsabilidad.

### Artículo 15 ter — Evaluación de Impacto en Protección de Datos (EIPD)
> **TEXTO LITERAL** (Art. 15 ter, líneas 1143-1181)
> "Cuando sea probable que un tipo de tratamiento, por su naturaleza, alcance, contexto, tecnología
> utilizada o fines, pueda producir un alto riesgo para los derechos de las personas titulares [...] el
> responsable [...] deberá realizar, previo al inicio de las operaciones del tratamiento, una evaluación
> del impacto [...] La evaluación de impacto se requerirá siempre en casos de: a) Evaluación sistemática y
> exhaustiva de aspectos personales [...] basadas en tratamiento o decisiones automatizadas, como la
> elaboración de perfiles [...] b) Tratamiento masivo de datos o a gran escala. c) Tratamiento que
> implique observación o monitoreo sistemático de una zona de acceso público. d) Tratamiento de datos
> sensibles y especialmente protegidos, en las hipótesis de excepción del consentimiento. La Agencia [...]
> establecerá y publicará una lista orientativa [...] también establecerá las orientaciones mínimas [...]"

**Razonamiento aplicado:** la EIPD es **obligatoria por ley** (no una buena práctica) en 4 supuestos que
casi todos ocurren en un SLEP: (a) perfilamiento de alumnos con riesgo de deserción, (b) tratamiento
masivo (toda la base de matrícula), (c) monitoreo de zona pública (cámaras de establecimiento), (d)
tratamiento de sensibles sin consentimiento (PIE, salud, situación socioeconómica bajo base legal). Un
SLEP que no ha hecho ninguna EIPD tiene al menos 3-4 procesos que la exigen desde ya.

---

## Título II §2 — Del tratamiento de datos personales sensibles (Arts. 16-16 ter)

### Artículo 16 — Regla general para datos sensibles
> **TEXTO LITERAL** (Art. 16, líneas 1186-1257)
> "El tratamiento de los datos personales sensibles sólo puede realizarse cuando el titular [...]
> manifiesta su consentimiento en forma expresa [...] Sin perjuicio de lo anterior, es lícito el
> tratamiento [...] sin el consentimiento [...] en los siguientes casos: a) Cuando el tratamiento se
> refiere a datos [...] que el titular ha hecho manifiestamente públicos [...] b) Cuando el tratamiento
> se basa en un interés legítimo realizado por una persona jurídica de derecho público o [...] privado
> que no persiga fines de lucro [...] [4 condiciones acumulativas] [...] c) Cuando el tratamiento [...]
> resulte indispensable para salvaguardar la vida, salud o integridad física o psíquica del titular [...]
> d) Cuando el tratamiento [...] sea necesario para la formulación, ejercicio o defensa de un derecho ante
> los tribunales [...] e) Cuando el tratamiento [...] sea necesario para el ejercicio de derechos y el
> cumplimiento de obligaciones [...] en el ámbito laboral o de seguridad social [...] f) Cuando el
> tratamiento [...] lo autorice o mandate expresamente la ley."

**Razonamiento aplicado:** para datos sensibles el consentimiento debe ser **expreso** (no basta el
inequívoco genérico del Art. 12) — declaración escrita, verbal o medio tecnológico equivalente, nunca
tácito ni por silencio. La letra (f) es la base de licitud típica de un SLEP para tratar PIE/salud/IVE:
"lo autorice o mandate expresamente la ley" (decretos 170/2009, 83/2015 y normativa JUNAEB), no
consentimiento del apoderado — importante porque el consentimiento no es revocable respecto de una
obligación legal.

### Artículo 16 bis — Datos de salud y perfil biológico
> **TEXTO LITERAL** (Art. 16 bis, líneas 1259-1325)
> "[...] los datos personales relativos a la salud del titular, así como aquéllos relativos al perfil
> biológico [...] sólo podrán ser tratados para los fines previstos por las leyes especiales en materia
> sanitaria. [...] en los siguientes casos [sin consentimiento]: a) [indispensable para salvaguardar vida
> o integridad] [...] b) En casos de alerta sanitaria legalmente decretada. c) Cuando sean utilizados con
> fines históricos, estadísticos o científicos [...] d) [...] tribunales [...] e) Cuando el tratamiento
> sea necesario para fines de medicina preventiva o laboral, evaluación de la capacidad laboral del
> trabajador, diagnóstico médico [...] f) Cuando la ley así lo permita [...] Se prohíbe el tratamiento y
> la cesión de los datos relativos a la salud [...] cuando los datos o muestras han sido recolectados en
> el ámbito laboral, educativo, deportivo, social, de seguros, de seguridad o identificación, salvo que la
> ley expresamente autorice su tratamiento en casos calificados [...]"

**Razonamiento aplicado:** hay una **prohibición reforzada** específica para datos de salud recolectados
en el ámbito **educativo** (mencionado expresamente en el inciso final) — un colegio no puede tratar/ceder
libremente datos de salud de un alumno recolectados en ese contexto salvo que una ley lo autorice
expresamente en un caso calificado (ej. PIE bajo Decreto 170). Esto es más estricto que la regla general
de sensibles del Art. 16.

### Artículo 16 ter — Datos biométricos
> **TEXTO LITERAL** (Art. 16 ter, líneas 1327-1357)
> "Son datos personales biométricos aquellos obtenidos a partir de un tratamiento técnico específico,
> relativos a las características físicas, fisiológicas o conductuales de una persona que permitan o
> confirmen la identificación única de ella, tales como la huella digital, el iris, los rasgos de la mano
> o faciales y la voz. Sólo podrán tratarse [...] siempre que el responsable proporcione al titular la
> siguiente información específica: a) La identificación del sistema biométrico usado; b) La finalidad
> específica [...]; c) El período durante el cual los datos [...] serán utilizados, y d) La forma en que
> el titular puede ejercer sus derechos."

**Razonamiento aplicado:** relevante para cualquier sistema de control de acceso o asistencia por huella
digital en un establecimiento — exige informar 4 elementos específicos antes de implementar el sistema,
no basta el aviso genérico de la política de privacidad.

---

## Título II §3 — Categorías especiales de datos (Arts. 16 quáter-16 sexies)

### Artículo 16 quáter — Datos de niños, niñas y adolescentes
> **TEXTO LITERAL** (Art. 16 quáter, líneas 1363-1394)
> "El tratamiento de los datos personales que conciernen a los niños, niñas y adolescentes, sólo puede
> realizarse atendiendo al interés superior de éstos y al respeto de su autonomía progresiva. [...] para
> tratar los datos personales de los niños y niñas se requiere el consentimiento otorgado por sus padres o
> representantes legales o por quien tiene a su cargo el cuidado personal [...] salvo que expresamente lo
> autorice o mandate la ley. Los datos personales de los adolescentes se podrán tratar de acuerdo a las
> normas de autorización previstas [...] para los adultos [...] Los datos personales sensibles de los
> adolescentes menores de dieciséis años sólo se podrán tratar con el consentimiento otorgado por sus
> padres [...] Para los efectos de esta ley, se consideran niños o niñas a los menores de catorce años, y
> adolescentes, a los mayores de catorce y menores de dieciocho años. Constituye una obligación especial
> de los **establecimientos educacionales** y de todas las personas o entidades públicas o privadas que
> traten o administren datos personales de niños, niñas y adolescentes [...] velar por el uso lícito y la
> protección de la información personal [...]"

**Razonamiento aplicado:** define edades con precisión legal — **niño/niña: <14 años; adolescente: 14-17
años**. Regla escalonada: niños siempre requieren consentimiento parental (salvo mandato legal);
adolescentes 14-17 se tratan como adultos salvo que el dato sea **sensible y el adolescente tenga menos
de 16 años**, caso en que vuelve a requerirse consentimiento parental. El inciso final impone una
**obligación especial y expresa a los establecimientos educacionales por nombre** — no es una obligación
genérica de "cualquier responsable", la ley singulariza a los colegios como sujeto reforzado de este
deber.

### Artículo 16 quinquies — Fines históricos, estadísticos, científicos y de estudios
> **TEXTO LITERAL** (Art. 16 quinquies, líneas 1395-1425)
> "Se entiende que existe un interés legítimo en el tratamiento de datos personales [...] cuando el
> tratamiento se realiza exclusivamente con fines históricos, estadísticos, científicos y para estudios o
> investigaciones, todos los cuales deben atender fines de interés público. Los responsables [...] deberán
> adoptar y acreditar que han cumplido con todas las medidas de calidad y seguridad necesarias [...] En el
> caso de los datos personales sensibles, el responsable debe identificar los riesgos posibles e
> implementar las medidas tendientes a su reducción o mitigación. Cumplidas estas condiciones, el
> responsable podrá almacenar y utilizar los datos por un período indeterminado de tiempo. [...] deberán
> previamente adoptar las medidas necesarias para anonimizar los datos que se publiquen."

**Razonamiento aplicado:** habilita conservación **indeterminada** (excepción a la regla general de
proporcionalidad temporal del Art. 3° letra c) — pero exige exclusividad del fin y anonimización previa a
toda publicación. Relevante para bases de datos de investigación educativa (SIMCE agregado, estudios
longitudinales) siempre que sea exclusivamente para ese fin, no un uso mixto con fines operativos.

### Artículo 16 sexies — Datos de geolocalización
> **TEXTO LITERAL** (Art. 16 sexies, líneas 1427-1436)
> "El tratamiento de los datos personales de geolocalización del titular se podrá realizar bajo las
> mismas fuentes de licitud establecidas en los artículos 12 y 13. El titular de datos deberá ser
> informado de manera clara, suficiente y oportuna, del tipo de datos de geolocalización que serán
> tratados, de la finalidad y duración del tratamiento y si los datos se comunicarán o cederán a un
> tercero para la prestación de un servicio con valor añadido."

**Razonamiento aplicado:** confirma lo ya verificado — geolocalización NO es una categoría de dato
sensible aparte, se rige por las bases generales (Arts. 12-13), solo con deber de información reforzado.
Aplicable a apps de transporte escolar con tracking GPS de buses/alumnos.

---

## Título III — Obligaciones de carácter económico, financiero, bancario o comercial (Arts. 17-19, Ley 19.628 original modificada puntualmente)

### Artículo 17 — Régimen de comunicación de datos comerciales
> **TEXTO LITERAL** (Art. 17 Ley 19.628 original, sources/especifico/ley-19628-original-texto.txt líneas 430-472, con los ajustes puntuales de la Ley 21.719 N°9 ya incorporados: "bancos de datos"→"bases de datos" y el nuevo inciso 8° sobre supresión de obligaciones prescritas)
> "Los responsables de los registros o bancos de datos personales sólo podrán comunicar información que
> verse sobre obligaciones de carácter económico, financiero, bancario o comercial, cuando éstas consten
> en letras de cambio y pagarés protestados; cheques protestados [...] como asimismo el incumplimiento de
> obligaciones derivadas de mutuos hipotecarios y de préstamos o créditos de bancos, sociedades
> financieras [...] No podrá comunicarse la información relacionada con las deudas contraídas con
> empresas públicas o privadas que proporcionen servicios de electricidad, agua, teléfono y gas; tampoco
> las deudas contraídas con instituciones de educación superior [...] ni alguna deuda contraída con la
> finalidad de recibir para sí o para terceros **un servicio educacional formal en cualquiera de sus
> niveles**; ni las deudas contraídas con prestadores de salud [...] Los responsables deberán suprimir de
> sus registros o bases de datos, toda aquella información personal relativa a obligaciones prescritas,
> sin necesidad de mediar solicitud, orden judicial, ni instrucción de la autoridad de protección de
> datos [inciso agregado por Ley 21.719]."

**Razonamiento aplicado:** confirma y cierra el punto que quedaba `[verificar]` en versiones previas de
este mapa — **cualquier deuda por servicio educacional formal está expresamente excluida** del régimen
DICOM/boletín comercial, en cualquier nivel (básica, media, superior). Un colegio/SLEP no puede reportar
morosidad de matrícula/mensualidad a un boletín comercial invocando este Título; tampoco puede ser objeto
de ese reporte por deudas asociadas al servicio educativo que presta. La supresión de obligaciones
prescritas ahora es automática, sin necesidad de solicitud del deudor.

### Artículo 18 — Plazo máximo de comunicación
> **TEXTO LITERAL** (Art. 18, líneas 560-570 ley-19628-original)
> "En ningún caso pueden comunicarse los datos a que se refiere el artículo anterior [...] luego de
> transcurridos cinco años desde que la respectiva obligación se hizo exigible. Tampoco se podrá continuar
> comunicando los datos relativos a dicha obligación después de haber sido pagada o haberse extinguido por
> otro modo legal."

**Razonamiento aplicado:** tope duro de 5 años desde exigibilidad, y cese inmediato al pagar — sin
relación operativa directa con SLEP dado que el Art. 17 ya excluye las deudas educacionales de este
régimen.

### Artículo 19 — Deber de actualizar/bloquear al pagarse la obligación
> **TEXTO LITERAL** (Art. 19, líneas 571-597 ley-19628-original)
> "El pago o la extinción de estas obligaciones [...] no produce la caducidad [...] mientras estén
> pendientes los plazos que establece el artículo precedente. Al efectuarse el pago [...] el acreedor
> avisará tal hecho, a más tardar dentro de los siguientes siete días hábiles, al responsable del registro
> o banco de datos [...] La infracción de cualquiera de estas obligaciones se conocerá y sancionará de
> acuerdo a lo previsto en el artículo 16 [ley 19.628 original — remite ahora al Título VII de la ley
> vigente, según la modificación del inciso final]."

**Razonamiento aplicado:** plazo operativo de 7 días hábiles para que el acreedor avise el pago al
boletín comercial. Sin aplicación práctica directa a SLEP por la exclusión del Art. 17, salvo que el
sostenedor mismo actúe como acreedor de servicios no educacionales (arriendos, concesiones de casino).

**Relevancia indirecta para SLEP/colegio (dato sensible "situación socioeconómica"):** el Art. 12 letra
a) de esta ley menciona el tratamiento de "situación socioeconómica" "de conformidad con las normas del
Título III" — pero esa referencia cruzada no desarrolla una regla operativa propia para el uso educativo
de datos socioeconómicos (SEP, becas, JUNAEB, clasificación prioritario/preferente). No inventar una
regla que el texto no da: tratar ese dato sensible por la vía general del Art. 16 (consentimiento expreso
o base legal específica de los programas de subvención), no por el Título III.

---

## Título IV — Del tratamiento de datos personales por los órganos públicos (Arts. 20-26)

**Régimen directamente aplicable a SLEP** — ver también `aplicacion-sector-publico-slep.md`.

### Artículo 20 — Regla general
> **TEXTO LITERAL** (Art. 20, líneas 1498-1507)
> "Es lícito el tratamiento de los datos personales que efectúan los órganos públicos cuando se realiza
> para el cumplimiento de sus funciones legales, dentro del ámbito de sus competencias [...] En esas
> condiciones, los órganos públicos actúan como responsables de datos y no requieren el consentimiento del
> titular para tratar sus datos personales."

**Razonamiento aplicado:** este es el artículo que fundamenta por qué un SLEP normalmente NO necesita
consentimiento de apoderados/alumnos para tratar sus datos — la base de licitud por defecto es el
cumplimiento de función legal, no el consentimiento. Pedir consentimiento igual (como hacen muchos
formularios de matrícula) genera confusión sobre el régimen jurídico real y una falsa sensación de
revocabilidad.

### Artículo 21 — Principios y normas aplicables
> **TEXTO LITERAL** (Art. 21, líneas 1509-1540)
> "El tratamiento [...] que realicen los órganos públicos se rige por los principios establecidos en el
> artículo 3° [...] y los principios generales que rigen la Administración del Estado, especialmente los
> principios de coordinación, probidad y eficiencia. [...] son aplicables al tratamiento de datos que
> efectúen los órganos públicos, las disposiciones establecidas en los artículos 2°, 14, 14 bis, 14 ter,
> 14 quáter, 14 quinquies, 14 sexies y 15 bis, los artículos de los Párrafos Segundo y Tercero del Título
> II y los artículos del Título V y del Título VII [...] Asimismo, le son aplicables los artículos 4°,
> 5°, 6°, 7° y 8°, en conformidad a lo dispuesto en el artículo 23."

**Razonamiento aplicado:** lista de remisión expresa — un SLEP SÍ está sujeto a: definiciones (Art. 2),
obligaciones del responsable (14-14 sexies), tratamiento de sensibles (Título II §2-3), transferencia
internacional (Título V) e infracciones/sanciones (Título VII), y a los derechos ARCO+ básicos (Arts.
4-8) por reenvío del Art. 23. Confirma que casi todo el cuerpo sustantivo de la ley aplica igual a un
órgano público, con las reglas especiales del propio Título IV encima.

### Artículo 22 — Comunicación o cesión de datos por un órgano público
> **TEXTO LITERAL** (Art. 22, líneas 1542-1590)
> "Los órganos públicos están facultados para comunicar o ceder datos personales [...] a otros órganos
> públicos, siempre que la comunicación o cesión [...] resulte necesaria para el cumplimiento de sus
> funciones legales y ambos órganos actúen dentro del ámbito de sus competencias. [...] se debe realizar
> para un tratamiento específico y el órgano público receptor no los podrá utilizar para otros fines. [...]
> El órgano público receptor [...] sólo puede conservarlos por el tiempo necesario [...] Para los efectos
> de poder comunicar o ceder datos personales a personas o entidades privadas, los organismos públicos
> deberán contar con el consentimiento del titular, salvo que la comunicación o cesión [...] sea necesaria
> para cumplir las funciones del organismo público en materia de fiscalización o inspección. [...] Los
> organismos públicos deberán informar mensualmente a través de su página web institucional los convenios
> suscritos con otros organismos públicos y con entidades privadas relativos a cesión o transferencia de
> datos personales."

**Razonamiento aplicado:** transferencias SLEP→MINEDUC/SIGE/DEMRE/CPEIP/JUNJI (entre órganos públicos) no
requieren consentimiento si son necesarias para función legal de ambos — pero SLEP→proveedor privado
(ej. software cloud) SÍ requiere consentimiento salvo fiscalización/inspección, lo que en la práctica casi
nunca aplica a un proveedor tecnológico. Deber de transparencia activa: publicar mensualmente en el sitio
web los convenios de cesión — obligación concreta y verificable de auditoría (¿el sitio web del SLEP
publica esto hoy?).

### Artículo 23 — Ejercicio de derechos, tutela y reclamo de ilegalidad
> **TEXTO LITERAL** (Art. 23, líneas 1592-1630)
> "El titular de datos podrá ejercer ante el órgano público los derechos de acceso, rectificación y
> oposición [...] Los organismos públicos no acogerán las solicitudes [...] en los siguientes casos: a)
> Cuando con ello se impida o entorpezca el cumplimiento de las funciones fiscalizadoras, investigativas,
> de protección a víctimas y testigos o sancionatorias [...] y b) Cuando con ello se afecte el carácter
> secreto de la información establecido por la ley. El ejercicio de los derechos [...] se deberá realizar
> [...] dirigiéndose al jefe superior del servicio. El titular podrá reclamar ante la Agencia [...]"

**Razonamiento aplicado:** en un SLEP, las solicitudes ARCO+ se dirigen formalmente al jefe superior del
servicio — Director(a) Ejecutivo(a) — no a cualquier funcionario; delegar la recepción operativa está
bien, pero el responsable formal ante la Agencia es esa autoridad.

### Artículo 24 — Regímenes especiales
> **TEXTO LITERAL** (Art. 24, líneas 1632-1693)
> "El tratamiento, comunicación o cesión de datos personales sensibles, realizado por órganos públicos
> competentes en las materias que a continuación se indican, estarán sujetos exclusivamente al régimen de
> regulación especial [...]: a) [prevención/investigación penal] [...] b) [seguridad de la Nación,
> defensa] [...] c) [emergencia o catástrofe declarada] [...] d) [protegidos por normas de secreto,
> reserva o confidencialidad de sus leyes] [...]"

**Razonamiento aplicado:** régimen residual/de excepción, aplicable a organismos con competencias
penales/de seguridad — no es el régimen típico de un SLEP salvo situaciones puntuales de colaboración con
Carabineros/Fiscalía por hechos ocurridos en un establecimiento (letra a).

### Artículo 25 — Datos de infracciones penales, civiles, administrativas y disciplinarias
> **TEXTO LITERAL** (Art. 25, líneas 1695-1767)
> "Los datos personales relativos a la comisión y sanción de infracciones penales, civiles,
> administrativas y disciplinarias sólo pueden ser tratados por los organismos públicos para el
> cumplimiento de sus funciones legales [...] No podrán comunicarse o hacerse públicos [...] una vez
> prescrita la acción [...] o una vez que se haya cumplido o prescrito la pena o la sanción impuesta [...]
> Las personas que se desempeñen en los órganos públicos están obligadas a guardar secreto respecto de
> esta información [...] Respecto de las infracciones civiles, administrativas y disciplinarias,
> permanecerán accesibles al público por el período de cinco años. Se prohíbe el tratamiento masivo de los
> datos personales contenidos en los registros electrónicos de infracciones [...] El incumplimiento [...]
> constituye una infracción gravísima [...]"

**Razonamiento aplicado:** directamente aplicable a sumarios administrativos y medidas disciplinarias
docentes/funcionarias del SLEP — plazo de publicidad de 5 años para infracciones administrativas/
disciplinarias, y prohibición expresa de tratamiento masivo de esos registros (infracción gravísima si se
incumple) — un cruce masivo de datos de sumarios para "análisis de riesgo de personal" sin autorización
legal específica encajaría en esta prohibición.

### Artículo 26 — Reglamento
> **TEXTO LITERAL** (Art. 26, líneas 1769-1781)
> "Las condiciones, modalidades e instrumentos para la comunicación o cesión de datos personales entre
> organismos públicos y con personas u organismos privados, se regularán a través de un reglamento
> expedido por el Ministerio Secretaría General de la Presidencia [...] previo informe de la Agencia. [...]
> Con todo, este reglamento no será aplicable a aquellas cesiones en las que tenga participación alguno de
> los órganos a los que se refiere el Título VIII de esta ley."

**Razonamiento aplicado:** reglamento pendiente de dictación (distinto del Reglamento MPI ya vigente,
que es de Hacienda) — verificar activamente si ya fue publicado antes de asumir que existe un
procedimiento reglado detallado para cesiones órgano público↔privado.

---

## Título V — De la transferencia internacional de datos personales (Arts. 27-29)

### Artículo 27 — Regla general de autorización
> **TEXTO LITERAL** (Art. 27, líneas 1788-1854)
> "Cumpliéndose los requisitos [...] son lícitas las operaciones de transferencia internacional de datos
> en cualquiera de los siguientes casos: a) Cuando la transferencia se realice a [...] un país que
> proporcione niveles adecuados de protección [...] b) Cuando la transferencia [...] quede amparada por
> cláusulas contractuales, normas corporativas vinculantes, u otros instrumentos jurídicos [...] c) Cuando
> [...] adopten un modelo de cumplimiento o mecanismo de certificación [...] En ausencia de una decisión
> de adecuación o de garantías adecuadas, se podrá realizar una transferencia específica y que no sea
> habitual, si se cumple alguno de los siguientes supuestos: a) [consentimiento expreso] b) [transferencias
> bancarias/financieras/bursátiles reguladas] c) [tratados internacionales ratificados] d) [convenios de
> cooperación de órganos públicos] e) [autorizada expresamente por ley] f) [colaboración judicial
> internacional] g) [contrato con el titular] h) [urgencia médica o sanitaria]"

**Razonamiento aplicado:** 3 vías generales + 8 excepciones específicas para casos no habituales — para
cualquier uso de nube extranjera (Microsoft 365, Google Workspace, Zoom) hay que verificar primero si
Chile tiene lista de países adecuados vigente (Art. 28) o si el proveedor ofrece cláusulas contractuales
tipo aprobadas por la Agencia; no basta "mencionarlo en el RAT" sin resolver bajo cuál de las 3 vías
generales (o, si no aplican, cuál de las 8 excepciones puntuales) se ampara la transferencia.

### Artículo 28 — Determinación de países adecuados y garantías
> **TEXTO LITERAL** (Art. 28, líneas 1855-1928)
> "Se entiende que el ordenamiento jurídico de un país posee niveles adecuados de protección [...] cuando
> cumple con estándares similares o superiores a los fijados en esta ley. La Agencia determinará
> fundadamente los países [...] considerando, a lo menos, los siguientes: a) [principios] b) [derechos y
> autoridad de control] c) [obligaciones de información y seguridad] d) [responsabilidades por
> infracciones]. Se considerarán garantías adecuadas aquellos instrumentos [...] que otorguen derechos
> exigibles y acciones legales efectivas [...] La Agencia podrá aprobar cláusulas modelo [...] Cuando la
> transferencia se efectúe entre sociedades [...] de un mismo grupo empresarial [...] las transferencias
> podrán quedar amparadas en normas corporativas vinculantes previamente aprobadas por la Agencia. [...]
> Corresponderá al responsable de datos que efectuó la transferencia [...] acreditar ante la Agencia que
> ésta se practicó de conformidad a las reglas [...]"

**Razonamiento aplicado:** la lista de países adecuados y los modelos de cláusulas los aprueba/publica la
Agencia — verificar activamente en su sitio web al momento de contratar un proveedor extranjero, no
asumir que un país es "adecuado" solo porque lo es bajo GDPR (los estándares chilenos son autónomos
aunque similares). **Mientras la Agencia no dicte su propia norma**, rige de forma transitoria la
Resolución del Ministerio de Economía RAEX202503748 (19-dic-2025) que aprobó cláusulas contractuales
modelo — ver `clausulas-modelo-transferencia-internacional.md`, verificado contra
`sources/especifico/clausulas-modelo-transferencia-economia.pdf`.

### Artículo 29 — Fiscalización
> **TEXTO LITERAL** (Art. 29, líneas 1930-1942)
> "La Agencia fiscalizará las operaciones de transferencia internacional de datos, pudiendo formular
> recomendaciones, adoptar medidas conservativas y en casos calificados, suspender temporalmente el envío
> de los datos."

**Razonamiento aplicado:** la Agencia puede suspender cautelarmente un flujo internacional de datos en
curso — riesgo operativo real para cualquier institución cuya operación dependa de un proveedor cloud
extranjero sin base de licitud clara para la transferencia.

---

## Título VI — Agencia de Protección de Datos Personales (Arts. 30-32 bis)

*Artículos de organización interna de la Agencia — se cita el texto por integridad (contrato v3 exige
"sin saltarse nada"), con razonamiento breve porque la aplicación práctica para un responsable de datos
externo es baja: son normas sobre CÓMO se organiza el regulador, no sobre qué debe hacer el regulado.*

### Artículo 30 — Creación de la Agencia
> **TEXTO LITERAL** (líneas 1950-1964): "Créase la Agencia de Protección de Datos Personales, corporación
> autónoma de derecho público, de carácter técnico, descentralizado, con personalidad jurídica y
> patrimonio propio, que se relacionará con el Presidente de la República a través del Ministerio de
> Economía, Fomento y Turismo. La Agencia tendrá por objeto velar por la efectiva protección de los
> derechos que garantizan la vida privada de las personas y sus datos personales [...] y fiscalizar el
> cumplimiento de sus disposiciones."

**Razonamiento aplicado:** confirma que la Agencia es autónoma (no depende jerárquicamente de un
ministerio, solo se "relaciona" con el Presidente a través de Economía) — relevante para evaluar su
independencia real frente a fiscalizados que sean también órganos del Estado.

### Artículo 30 bis — Funciones y atribuciones de la Agencia
> **TEXTO LITERAL** (líneas 1966-2063, resumen de las letras operativamente relevantes): "a) Dictar
> instrucciones y normas generales y obligatorias [...] previa consulta pública [...] b) Aplicar e
> interpretar administrativamente las disposiciones [...] c) Fiscalizar el cumplimiento [...] podrá
> requerir [...] la entrega de cualquier documento, libro o antecedente [...] d) Determinar las
> infracciones e incumplimientos [...] e) Ejercer la potestad sancionadora [...] f) Resolver las
> solicitudes y reclamos [...] m) Certificar, registrar y supervisar los modelos de prevención de
> infracciones [...]"

**Razonamiento aplicado:** confirma potestad de requerir "cualquier documento, libro o antecedente" en
fiscalización (letra c) — un responsable no puede negarse a exhibir su RAT o registros de tratamiento
ante un requerimiento fundado de la Agencia.

### Artículo 30 ter — Dirección de la Agencia
> **TEXTO LITERAL** (líneas 2078-2099): "La dirección superior de la Agencia le corresponderá al Consejo
> Directivo [...] a) Ejercer las atribuciones [...] b) Establecer normativa interna [...] c) Establecer
> políticas de planificación [...] d) Dictar normas de carácter general, circulares [...] e) Formular al
> Presidente [...] propuestas de reforma [...] f) Elaborar [...] una cuenta pública anual [...]"

**Razonamiento aplicado:** sin implicancia directa para responsables externos — estructura de gobierno
interno colegiado (Consejo Directivo).

### Artículo 30 quáter — Miembros del Consejo Directivo
> **TEXTO LITERAL** (líneas 2101-2146, resumen): "El Consejo Directivo [...] estará integrado por tres
> consejeros, designados por el Presidente de la República, con acuerdo del Senado [...] Los consejeros
> durarán seis años en sus cargos, no podrán ser designados para un nuevo periodo y se renovarán de forma
> individual, cada dos años. [...] exige dedicación exclusiva. [...] El quorum mínimo para sesionar será
> de dos consejeros."

**Razonamiento aplicado:** 3 consejeros, mandato de 6 años no renovable, dedicación exclusiva — diseño
pensado para independencia técnica frente a ciclos políticos de 4 años.

### Artículo 30 quinquies — Inhabilidades e incompatibilidades
> **TEXTO LITERAL** (líneas 2148-2212, resumen): "El cargo de consejero es incompatible con el desempeño
> de todo cargo o servicio [...] en el sector privado. [...] incompatible con la calidad de integrante de
> los órganos de dirección de los partidos políticos, funcionarios de la Administración del Estado [...]
> Adicionalmente, no podrá ser designado consejero: a) [condenado por delitos de función pública,
> tributarios, fe pública] [...] c) [sancionado grave/gravísimo en los últimos 5 años] d) [gerente,
> delegado de datos, director de empresa de tratamiento de datos en el último año]"

**Razonamiento aplicado:** régimen de inhabilidades diseñado para evitar captura regulatoria — nadie que
haya sido delegado de protección de datos o director de una empresa de tratamiento de datos en el último
año puede ser consejero.

### Artículo 30 sexies — Remoción y cesación
> **TEXTO LITERAL** (líneas 2214-2245, resumen): "Los consejeros serán removidos por la Corte Suprema
> [...] por incapacidad, mal comportamiento o negligencia manifiesta [...] Además de la remoción, serán
> causales de cesación: a) Expiración del plazo [...] b) Renuncia [...] c) Postulación a un cargo de
> elección popular. d) Inhabilidad o incompatibilidad sobreviniente [...]"

**Razonamiento aplicado:** remoción reservada a la Corte Suprema (no al Ejecutivo) — refuerza autonomía
frente al Presidente que los propuso.

### Artículo 30 septies — Remuneración
> **TEXTO LITERAL** (líneas 2247-2255): "El presidente [...] percibirá una remuneración bruta
> mensualizada equivalente a la de un Subsecretario de Estado [...] Los demás consejeros percibirán una
> remuneración equivalente al 85% de la remuneración que corresponda al presidente [...]"

**Razonamiento aplicado:** sin implicancia para responsables externos.

### Artículo 30 octies — Estatutos de la Agencia
> **TEXTO LITERAL** (líneas 2257-2262): "Los estatutos de la Agencia establecerán sus normas de
> funcionamiento [...] serán propuestos por la Agencia al Presidente de la República y su aprobación se
> dispondrá mediante decreto supremo [...]"

**Razonamiento aplicado:** sin implicancia directa; verificar si el decreto de estatutos ya fue dictado
al momento de cualquier consulta formal ante la Agencia (afecta su forma de funcionamiento operativo).

### Artículo 30 nonies — Funciones del presidente del Consejo
> **TEXTO LITERAL** (líneas 2264-2314, resumen): "El presidente [...] será el jefe de servicio [...] y
> tendrá la representación judicial y extrajudicial [...] a) Ejercer el rol de jefe de servicio [...] d)
> Representar legal, judicial y extrajudicialmente a la Agencia. [...] f) Contratar al personal [...]"

**Razonamiento aplicado:** identifica a la autoridad con representación legal de la Agencia para efectos
de notificaciones formales o gestiones ante ella.

### Artículo 31 — Coordinación con el Consejo para la Transparencia
> **TEXTO LITERAL** (líneas 2316-2357, resumen): "Cuando la Agencia deba dictar una instrucción [...] que
> pueda tener efectos en los ámbitos de competencia del Consejo para la Transparencia [...] le remitirá
> [...] y requerirá [...] un informe [...] dentro del plazo de treinta días corridos [...] A su vez, cuando
> el Consejo para la Transparencia deba dictar una instrucción [...] que tenga claros efectos en los
> ámbitos de competencia de la Agencia [...] requerirá informe a la Agencia [...]"

**Razonamiento aplicado:** mecanismo formal de coordinación entre transparencia y protección de datos —
relevante en la práctica cuando un SLEP enfrenta una solicitud de transparencia que colisiona con
protección de datos: ambos reguladores tienen un canal de coordinación previsto por ley, no queda
librado a la interpretación aislada del SLEP.

### Artículo 32 — Personal de la Agencia y fiscalización
> **TEXTO LITERAL** (líneas 2359-2409, resumen): "Las personas que presten servicios a la Agencia se
> regirán por el Código del Trabajo. [...] serán aplicables [...] las normas de probidad [...] Las
> personas que desempeñen funciones directivas [...] serán seleccionadas mediante concurso público [...]
> Alta Dirección Pública [...] la Agencia deberá cumplir con las normas [...] de Administración Financiera
> del Estado [...] estará sometida a la fiscalización de la Contraloría [...] Las resoluciones de la
> Agencia estarán exentas del trámite de toma de razón [...]"

**Razonamiento aplicado:** las resoluciones de la Agencia son exentas de toma de razón CGR — son
ejecutables de inmediato, sin el control previo de legalidad que sí aplica a otros actos administrativos;
esto acelera la ejecutoriedad de sus sanciones.

### Artículo 32 bis — Del patrimonio
> **TEXTO LITERAL** (líneas 2411-2426, resumen): "El patrimonio de la Agencia estará formado por: a) El
> aporte [...] en la Ley de Presupuestos [...] b) Los bienes muebles e inmuebles [...] c) Las donaciones
> [...] d) Las herencias y legados [...] e) Los aportes de la cooperación internacional."

**Razonamiento aplicado:** sin implicancia directa para responsables externos.

---

## Título VII — Responsabilidad, infracciones y sanciones (Arts. 33-53)

### Artículo 33 — Régimen general de responsabilidad
> **TEXTO LITERAL** (Art. 33, líneas 2432-2438)
> "El responsable de datos, sea una persona natural o jurídica, de derecho público o privado, que en sus
> operaciones de tratamiento de datos personales infrinja los principios señalados en el artículo 3° y
> los derechos y obligaciones establecidos en esta ley, será sancionado de conformidad con las normas del
> presente Título."

**Razonamiento aplicado:** unifica el estándar de responsabilidad para público y privado en un mismo
artículo base — las diferencias de régimen (multas en UTM vs. % de remuneración del jefe superior)
vienen después, en los artículos específicos (35 vs. 44).

### Artículo 34 — Infracciones leves, graves y gravísimas (clasificación general)
> **TEXTO LITERAL** (Art. 34, líneas 2445-2455)
> "Las infracciones cometidas por los responsables de datos a los principios señalados en el artículo 3°
> y a los derechos y obligaciones establecidos en esta ley se califican, atendida su gravedad, en leves,
> graves y gravísimas. Las responsabilidades [...] se entienden sin perjuicio de las demás
> responsabilidades legales, civiles o penales, que pudieran corresponderle."

**Razonamiento aplicado:** este es el marco, NO la lista — las listas concretas están en 34 bis (leves),
34 ter (graves) y 34 quáter (gravísimas). Corrige un error frecuente de fuentes secundarias que citan
"34 bis/ter/quáter" como si fueran subclasificaciones del mismo nivel: son niveles distintos y
crecientes de gravedad.

### Artículo 34 bis — Infracciones leves
> **TEXTO LITERAL** (Art. 34 bis, líneas 2457-2487)
> "Se consideran infracciones leves, las siguientes: a) Incumplir total o parcialmente el deber de
> información y transparencia, establecido en el artículo 14 ter. b) Carecer de la individualización del
> domicilio postal, correo electrónico o medio electrónico equivalente [...] c) Omitir la respuesta,
> responder en forma incompleta o fuera de plazo, las solicitudes formuladas por el titular [...] d)
> Omitir el envío a la Agencia de las comunicaciones previstas obligatoriamente [...] e) Incumplir las
> instrucciones generales impartidas por la Agencia en los casos que no esté sancionado como infracción
> grave o gravísima. f) Cometer cualquier otra infracción [...] que no sea calificada como grave o
> gravísima."

**Razonamiento aplicado:** letra (f) es una cláusula residual — toda infracción no tipificada
expresamente en 34 ter/quáter cae por defecto en "leve", nunca queda sin sanción por falta de tipificación
específica.

### Artículo 34 ter — Infracciones graves
> **TEXTO LITERAL** (Art. 34 ter, líneas 2489-2548)
> "Se consideran infracciones graves, las siguientes: a) Tratar los datos personales sin contar con el
> consentimiento [...] o sin un antecedente o fundamento legal que otorgue licitud [...], o tratarlos con
> una finalidad distinta [...] b) Comunicar o ceder datos personales, sin el consentimiento [...] c)
> Efectuar tratamiento [...] innecesarios en relación con los fines [...] d) Tratar datos [...] inexactos,
> incompletos o desactualizados [...] e) Impedir u obstaculizar el ejercicio legítimo de los derechos [...]
> f) Omitir la respuesta [...] de bloqueo temporal. g) Realizar tratamiento [...] de niños, niñas y
> adolescentes con infracción [...] h) [personas jurídicas sin fines de lucro, requisitos incumplidos] i)
> Vulnerar el deber de secreto o confidencialidad [...] j) Vulnerar o infringir las obligaciones de
> seguridad [...] k) Omitir las comunicaciones o los registros en los casos de vulneración de las medidas
> de seguridad [...] l) Adoptar medidas de calidad y seguridad insuficientes [...] fines históricos [...]
> m) Realizar operaciones de transferencia internacional [...] en contravención [...] n) Incumplir una
> resolución o un requerimiento específico y directo [...]"

**Razonamiento aplicado:** 14 hipótesis graves — las más frecuentes en auditoría real de un SLEP/colegio:
(a) tratar sin base legal clara, (i) vulnerar secreto, (j)/(k) fallar en seguridad o no reportar brecha,
(m) transferencia internacional irregular (proveedor cloud sin DPA ni base de transferencia). Cualquier
hallazgo de auditoría debe mapearse a una letra específica de este artículo para calificar correctamente
el riesgo, no describir el hallazgo en abstracto.

### Artículo 34 quáter — Infracciones gravísimas
> **TEXTO LITERAL** (Art. 34 quáter, líneas 2550-2589)
> "Se consideran infracciones gravísimas, las siguientes: a) Efectuar tratamiento [...] en forma
> fraudulenta. b) Destinar maliciosamente los datos [...] a una finalidad distinta [...] c) Comunicar o
> ceder, a sabiendas, información no veraz [...] d) Vulnerar el deber de secreto [...] sobre datos
> sensibles y datos [...] de infracciones [...] e) Tratar, comunicar o ceder, a sabiendas, datos [...]
> sensibles o [...] de niños, niñas y adolescentes, en contravención [...] f) Omitir en forma deliberada
> la comunicación de las vulneraciones a las medidas de seguridad [...] g) Efectuar tratamiento masivo de
> datos [...] de infracciones penales, civiles, administrativas y disciplinarias [...] sin autorización
> legal [...] h) Realizar, a sabiendas, operaciones de transferencia internacional [...] en contravención
> [...] i) Incumplir una resolución de la Agencia que resuelve la reclamación [...] j) Entregar, a
> sabiendas, información falsa [...] en el proceso de registro o certificación del MPI. k) Incumplir la
> obligación establecida en el artículo 15 ter [EIPD], en los casos que corresponda."

**Razonamiento aplicado:** el elemento común que escala de grave a gravísimo es casi siempre el dolo
("a sabiendas", "maliciosamente", "fraudulenta", "deliberada") — el mismo hecho objetivo (ej. tratar
datos sensibles de un niño sin base legal) puede calificar como grave (34 ter g) o gravísimo (34 quáter e)
según si hubo conocimiento/intención, lo que hace crítico documentar diligencia y buena fe en cualquier
incidente. La letra (k) confirma que **no hacer la EIPD obligatoria del Art. 15 ter es, por sí sola, una
infracción gravísima** — no un mero incumplimiento formal menor.

### Artículo 35 — Sanciones
> **TEXTO LITERAL** (Art. 35, líneas 2591-2631)
> "Las sanciones [...] serán las siguientes: a) Las infracciones leves serán sancionadas con amonestación
> escrita o multa de hasta 5.000 unidades tributarias mensuales. b) Las infracciones graves serán
> sancionadas con multa de hasta 10.000 unidades tributarias mensuales. c) Las infracciones gravísimas
> serán sancionadas con multa de hasta 20.000 unidades tributarias mensuales. En cada caso, la Agencia
> señalará las medidas tendientes a subsanar [...] en un plazo no mayor a sesenta días, de lo contrario se
> impondrá un recargo de 50% [...] En caso de que exista reincidencia [...] la Agencia podrá aplicar una
> multa de hasta tres veces el monto [...] En caso de que el infractor corresponda a una empresa distinta
> de aquéllas definidas como empresas de menor tamaño [...] que reincida [...] la multa podrá alcanzar [...]
> hasta el monto correspondiente al 2% o 4% de los ingresos anuales por ventas y servicios [...] según se
> trate de infracciones graves o gravísimas, respectivamente."

**Razonamiento aplicado:** confirma los 3 topes (5.000/10.000/20.000 UTM) — pero además: recargo
automático de 50% si no se subsanan las causales en 60 días, reincidencia simple hasta 3x el monto, y
reincidencia de empresa grande hasta 2-4% de ingresos anuales (mecanismo tipo RGPD por facturación, no
solo UTM fijas). El régimen de multas para SLEP como órgano público NO es este — ver Art. 44 (multa sobre
remuneración del jefe superior).

### Artículo 36 — Circunstancias atenuantes y agravantes
> **TEXTO LITERAL** (Art. 36, líneas 2633-2665)
> "Se considerarán circunstancias atenuantes: 1. Las acciones unilaterales de reparación [...] 2. La
> colaboración que el infractor preste en la investigación [...] 3. La ausencia de sanciones previas [...]
> 4. La autodenuncia ante la Agencia [...] 5. El haber cumplido diligentemente sus deberes de dirección y
> supervisión [...] lo que se verificará con el certificado expedido de acuerdo a lo dispuesto en el
> artículo 51. Se considerarán circunstancias agravantes: a) La reincidencia. Existe reincidencia cuando
> el responsable ha sido sancionado en dos o más ocasiones, en los últimos treinta meses [...] b) El
> carácter continuado de la infracción. c) El haber puesto en riesgo la seguridad de los derechos y
> libertades [...]"

**Razonamiento aplicado:** el atenuante N°5 es la conexión legal directa entre tener un **MPI
certificado** (Art. 51) y una reducción real de sanción — es el fundamento normativo exacto de por qué
certificar el modelo de prevención "atenúa sanciones" (mencionado en `mapa-articulos-reglamento-mpi.md`).
La autodenuncia (N°4) reduce responsabilidad incluso sin MPI certificado — vale la pena evaluarla ante
cualquier brecha detectada internamente antes de que la descubra la Agencia.

### Artículo 37 — Determinación del monto de las multas
> **TEXTO LITERAL** (Art. 37, líneas 2666-2715)
> "Para la determinación del monto de las multas [...] la Agencia deberá aplicar prudencialmente los
> siguientes criterios: 1. La gravedad de la conducta. 2. Si la conducta fue realizada con falta de
> diligencia o cuidado [...] 3. El perjuicio producido [...] especialmente el número de titulares [...]
> afectados. 4. El beneficio económico obtenido [...] 5. Si el tratamiento realizado incluye datos [...]
> sensibles o [...] de niños, niñas y adolescentes. 6. La capacidad económica del infractor. 7. Las
> sanciones aplicadas con anterioridad [...] 8. Las circunstancias atenuantes y agravantes [...] En caso
> de que una conducta dé origen a dos o más infracciones [...] se impondrá una sola multa, considerando
> siempre la sanción de la infracción más grave. [...] Cuando por unos mismos hechos [...] el infractor
> pudiese ser sancionado con arreglo a esta ley y a otra u otras leyes, [...] se le impondrá la de mayor
> gravedad."

**Razonamiento aplicado:** el criterio 5 (sensibles o NNA) es agravante de facto en la determinación del
monto — cualquier incidente de un SLEP casi siempre involucra datos de NNA, lo que empuja el monto hacia
el tramo alto del rango aplicable a la infracción calificada.

### Artículo 38 — Sanciones accesorias
> **TEXTO LITERAL** (Art. 38, líneas 2717-2750)
> "En caso que se impongan multas por infracciones gravísimas reiteradas, en un período de veinticuatro
> meses, la Agencia podrá disponer la suspensión de las operaciones y actividades de tratamiento de datos
> [...] hasta por un término de treinta días. Esta suspensión no afectará el almacenamiento de datos [...]
> La suspensión [...] podrá ser parcial o total, y no podrá decretarse cuando con ello se afecten los
> derechos de los titulares. [...] Si el responsable no da cumplimiento [...] esta medida se podrá
> prorrogar indefinidamente [...]"

**Razonamiento aplicado:** sanción operativamente severa — suspender el tratamiento de datos de un SLEP
(ej. bloquear el uso del sistema de matrícula/notas) sería catastrófico operativamente; la ley limita esto
a reincidencia gravísima reiterada en 24 meses, no a un hecho aislado.

### Artículo 39 — Registro Nacional de Sanciones y Cumplimiento
> **TEXTO LITERAL** (Art. 39, líneas 2752-2768)
> "Créase el Registro Nacional de Sanciones y Cumplimiento [...] público y su acceso gratuito. [...] En él
> se deberán consignar a los responsables de datos que hayan sido sancionados [...] Deberá distinguirse
> según la gravedad [...] También se deberán consignar los responsables que adopten modelos certificados
> de prevención de infracciones, con carácter vigente. Las anotaciones [...] serán de acceso público por
> el período de cinco años [...]"

**Razonamiento aplicado:** las sanciones son públicas por 5 años, con impacto reputacional además del
económico — un SLEP sancionado queda expuesto públicamente, no solo paga la multa.

### Artículo 40 — Prescripción
> **TEXTO LITERAL** (Art. 40, líneas 2770-2782)
> "Las acciones para perseguir la responsabilidad por las infracciones [...] prescriben en el plazo de
> cuatro años, contado desde la ocurrencia del hecho [...] En caso de infracciones continuadas, el plazo
> [...] se contará desde el día en que la infracción haya cesado. Se interrumpe la prescripción con la
> notificación del inicio del procedimiento [...] Las sanciones [...] prescriben en el plazo de tres años,
> contado desde la fecha en que la resolución [...] quede ejecutoriada."

**Razonamiento aplicado:** dos plazos distintos — 4 años para perseguir la infracción (desde el hecho o
desde que cesa si es continuada) y 3 años para ejecutar la sanción ya impuesta.

### Artículo 41 — Procedimiento administrativo de tutela de derechos
> **TEXTO LITERAL** (Art. 41, líneas 2787-2884, resumen de plazos operativos): "El titular [...] podrá
> reclamar ante la Agencia cuando el responsable le haya denegado una solicitud [...] dentro del plazo de
> treinta días hábiles [...] Recibido el reclamo, la Agencia, dentro de los diez días hábiles siguientes,
> deberá determinar si éste cumple con los requisitos [...] Acogido el reclamo [...] la Agencia notificará
> al responsable [...] quien dispondrá de un plazo de treinta días corridos, prorrogables [...] La
> resolución del reclamo [...] no podrá superar los seis meses. [...] podrán ser impugnadas judicialmente
> dentro del plazo de quince días hábiles [...]"

**Razonamiento aplicado:** cadena de plazos operativa completa: titular reclama en 30 días hábiles desde
denegación → Agencia admite a trámite en 10 días hábiles → responsable contesta en 30 días corridos
(prorrogables) → resolución en máximo 6 meses → impugnación judicial en 15 días hábiles. Útil para
calendarizar la gestión de cualquier reclamo real que reciba el SLEP desde la Agencia.

### Artículo 42 — Procedimiento administrativo por infracción de ley
> **TEXTO LITERAL** (Art. 42, líneas 2886-2974, resumen de plazos operativos): "a) El procedimiento
> sancionatorio será instruido por la Agencia. [...] c) La Agencia deberá presentar una formulación de
> cargos [...] e) El responsable de datos tendrá un plazo de quince días hábiles para presentar sus
> descargos. [...] j) La resolución que ponga fin al procedimiento [...] debe ser fundada [...] l) El
> procedimiento administrativo de infracción de ley no podrá superar los seis meses."

**Razonamiento aplicado:** este es el procedimiento sancionatorio propiamente tal (distinto del 41, que
es de tutela por denegación de derechos) — 15 días hábiles para descargos tras la formulación de cargos,
6 meses de plazo máximo total. Es el procedimiento aplicable, vía Art. 44, cuando se investiga a un
SLEP como órgano público.

### Artículo 43 — Procedimiento de reclamación judicial
> **TEXTO LITERAL** (Art. 43, líneas 2979-3033, resumen): "Las personas [...] que estimen que un acto
> administrativo [...] o una resolución final [...] de la Agencia, sea ilegal, podrán deducir un reclamo
> de ilegalidad ante la Corte de Apelaciones de Santiago o la del lugar donde se encuentre domiciliado el
> reclamante [...] dentro de los quince días hábiles siguientes [...] Tratándose de reclamaciones en
> contra de una resolución que resuelve un procedimiento sancionatorio, la Corte podrá confirmar o
> revocar la resolución impugnada [...]"

**Razonamiento aplicado:** vía judicial de última instancia es la Corte de Apelaciones (no la Corte
Suprema en primera instancia), con opción de foro en el domicilio del reclamante — favorable en términos
de acceso para un SLEP regional que no quiera litigar necesariamente en Santiago.

### Artículo 44 — Responsabilidad administrativa del jefe superior del órgano público
> **TEXTO LITERAL** (Art. 44, líneas 3039-3094)
> "El jefe superior de un órgano público deberá velar por que el órgano respectivo realice sus operaciones
> y actividades de tratamiento de los datos personales con arreglo a los principios, derechos y
> obligaciones establecidos en el Título IV [...] Las infracciones [...] se tipifican en los artículos 34
> bis, 34 ter y 34 quáter y serán sancionadas con multa de veinte por ciento a cincuenta por ciento de la
> remuneración mensual del jefe superior del órgano público infractor. [...] Si el órgano público persiste
> en la infracción, se le aplicará al jefe superior [...] el duplo de la sanción originalmente impuesta y
> la suspensión en el cargo por un lapso de cinco días. Tratándose de datos personales sensibles, la multa
> será del cincuenta por ciento de la remuneración mensual [...] y procederá la suspensión en el cargo de
> hasta treinta días. [...] la Contraloría General de la República, a petición de la Agencia podrá [...]
> incoar los procedimientos administrativos y proponer las sanciones [...] Las sanciones [...] deberán ser
> publicadas en el sitio web de la Agencia y del respectivo órgano o servicio [...]"

**Razonamiento aplicado:** artículo central para SLEP — la multa recae **personalmente sobre la
remuneración del Director(a) Ejecutivo(a)** (20-50% de su remuneración mensual, 50% fijo si son datos
sensibles), no sobre el presupuesto institucional como tal. Persistencia en la infracción duplica la
sanción y agrega suspensión de 5 días; si son sensibles, la suspensión puede llegar a 30 días. La CGR
puede intervenir a petición de la Agencia. Esto fundamenta por qué la responsabilidad de protección de
datos en un SLEP no es "del área de TI" sino que escala legalmente hasta la máxima autoridad ejecutiva.

### Artículo 45 — Responsabilidad del funcionario infractor
> **TEXTO LITERAL** (Art. 45, líneas 3096-3113)
> "Sin perjuicio de lo dispuesto en el artículo anterior, si [...] se determina que existen
> responsabilidades individuales de uno o más funcionarios [...] la Contraloría General de la República,
> a petición de la Agencia, iniciará una investigación sumaria [...] Las sanciones a los funcionarios
> infractores serán determinadas de conformidad a lo dispuesto en el Estatuto Administrativo. En caso de
> que [...] se determine que cualquiera de los funcionarios [...] es responsable de alguna de las
> infracciones gravísimas [...] esta conducta se considerará una contravención grave a la probidad
> administrativa."

**Razonamiento aplicado:** responsabilidad del jefe superior (Art. 44) y del funcionario individual (Art.
45) son acumulativas, no alternativas — un mismo hecho puede generar sanción institucional al Director
Ejecutivo Y sumario administrativo al funcionario que efectivamente cometió la infracción. Una infracción
gravísima se califica automáticamente como contravención grave a la probidad, con las consecuencias
estatutarias que eso conlleva (más allá de la sanción específica de datos personales).

### Artículo 46 — Deber de los funcionarios de reserva y confidencialidad
> **TEXTO LITERAL** (Art. 46, líneas 3115-3145)
> "Los funcionarios de los órganos públicos que traten datos personales [...] deben guardar secreto o
> confidencialidad respecto de la información que tomen conocimiento en el ejercicio de sus cargos y
> abstenerse de usar dicha información con una finalidad distinta [...] o utilizarla en beneficio propio o
> de terceros. [...] se estimará que los hechos que configuren infracciones a esta disposición vulneran
> gravemente el principio de probidad administrativa [...]"

**Razonamiento aplicado:** deber de reserva individual de cada funcionario que trata datos — su
infracción es, por definición legal, una vulneración grave a la probidad (no solo una infracción a la ley
de datos), lo que la vincula directamente con el régimen disciplinario general del Estatuto
Administrativo.

### Artículo 47 — Responsabilidad civil (norma general)
> **TEXTO LITERAL** (Art. 47, líneas 3150-3170)
> "El responsable de datos deberá indemnizar el daño patrimonial y extrapatrimonial que cause al o los
> titulares, cuando en sus operaciones de tratamiento de datos infrinja los principios [...] y les cause
> perjuicio. [...] La acción indemnizatoria [...] podrá interponerse una vez ejecutoriada la resolución
> [...] favorable [...] y se tramitará de conformidad a las normas del procedimiento sumario [...] Las
> acciones civiles [...] prescribirán en el plazo de cinco años, contado desde que se encuentre
> ejecutoriada la resolución administrativa o la sentencia judicial [...]"

**Razonamiento aplicado:** la vía civil indemnizatoria es **posterior y dependiente** de una resolución
administrativa o sentencia firme previa que constate la infracción — no es una acción autónoma paralela;
primero se agota la vía ante la Agencia (o el reclamo de ilegalidad), y solo después se puede demandar el
daño patrimonial/extrapatrimonial.

### Artículo 48 — Prevención de infracciones (norma general)
> **TEXTO LITERAL** (Art. 48, líneas 3172-3176)
> "Los responsables de datos, sean personas naturales o jurídicas, públicas o privadas, deberán adoptar
> acciones destinadas a prevenir la comisión de las infracciones establecidas en los artículos 34 bis, 34
> ter y 34 quáter."

**Razonamiento aplicado:** confirma lo ya validado en esta skill — el Art. 48 es un **deber general de
prevención**, NO un mandato de designar DPO. Cualquier fuente que cite "el DPO es obligatorio por Art.
48" está leyendo mal el texto; la designación voluntaria de DPO está en el Art. 49/50, y su obligatoriedad
condicionada está en el Reglamento MPI Art. 6.

### Artículo 49 — Modelo de Prevención de Infracciones (MPI)
> **TEXTO LITERAL** (Art. 49, líneas 3178-3232)
> "Los responsables de datos podrán voluntariamente adoptar un modelo de prevención de infracciones
> consistente en un programa de cumplimiento. El programa de cumplimiento deberá contener, al menos, los
> siguientes elementos: a) La designación de un delegado de protección de datos personales. b) La
> definición de medios y facultades del delegado [...] c) La identificación del tipo de información que
> la entidad trata [...] d) La identificación de las actividades o procesos [...] de mayor riesgo [...] e)
> El establecimiento de protocolos, reglas y procedimientos específicos [...] f) Los mecanismos de reporte
> interno [...] g) La existencia de sanciones administrativas internas [...]"

**Razonamiento aplicado:** confirma **voluntariedad expresa** ("podrán voluntariamente") del MPI — y que
adoptar un MPI implica automáticamente designar un delegado (letra a), lo que conecta con la
obligatoriedad condicionada del DPO del Reglamento (Art. 6): no se puede tener MPI sin DPO, pero sí se
puede tener DPO sin MPI certificado.

### Artículo 50 — Atribuciones del delegado (DPO)
> **TEXTO LITERAL** (Art. 50, líneas 3234-3323)
> "El responsable de datos podrá designar un delegado de protección de datos personales. El delegado [...]
> deberá ser designado por la máxima autoridad directiva o administrativa [...] deberá contar con
> autonomía respecto de la administración [...] En las micro, pequeñas y medianas empresas, el dueño [...]
> podrán asumir personalmente las tareas [...] Los funcionarios públicos que desempeñen estas funciones e
> infrinjan este deber de secreto [...] serán sancionados de conformidad a lo que se prescribe en los
> artículos 246 a 247 bis del Código Penal. [...] el delegado de protección de datos tendrá las siguientes
> funciones: a) Informar y asesorar [...] b) Promover y participar en la política [...] c) Supervisar el
> cumplimiento [...] d) Preocuparse de la formación permanente [...] e) Asistir [...] en la identificación
> de los riesgos [...] f) Desarrollar un plan anual de trabajo [...] g) Absolver las consultas [...] h)
> Cooperar [...] con la Agencia."

**Razonamiento aplicado:** el DPO en función pública que infringe el secreto queda sujeto al **régimen
penal del Código Penal (Arts. 246-247 bis, delitos funcionarios)**, no solo a sanción administrativa —
consecuencia penal directa que eleva sustancialmente el estándar de cuidado exigible a quien asuma este
rol en un SLEP.

### Artículo 51 — Certificación, registro, supervisión del MPI
> **TEXTO LITERAL** (Art. 51, líneas 3325-3348)
> "La Agencia será la entidad encargada de certificar que el modelo de prevención de infracciones reúna
> los requisitos [...] La Agencia incorporará en el Registro Nacional de Sanciones y Cumplimiento a las
> entidades que posean una certificación vigente. Un reglamento expedido a través del Ministerio de
> Hacienda [...] establecerá los requisitos, modalidades y procedimientos para la implementación,
> certificación, registro y supervisión de los modelos de prevención de infracciones."

**Razonamiento aplicado:** este es el inciso que habilita expresamente el Reglamento DTO 662-25 (ver
`mapa-articulos-reglamento-mpi.md`) — la certificación del MPI y su efecto atenuante (Art. 36 N°5) dependen
enteramente del cumplimiento del reglamento derivado, no solo de este artículo.

### Artículo 52 — Vigencia de los certificados
> **TEXTO LITERAL** (Art. 52, líneas 3350-3365)
> "Los certificados expedidos por la Agencia tendrán una vigencia de tres años. [...] quedarán sin efecto
> en los siguientes casos: a) Por revocación [...] b) Por fallecimiento [...] c) Por disolución de la
> persona jurídica. d) Por resolución judicial ejecutoriada. e) Por cese voluntario de la actividad [...]"

**Razonamiento aplicado:** vigencia fija de 3 años — un MPI certificado necesita renovación periódica, no
es un estado permanente una vez obtenido.

### Artículo 53 — Revocación de la certificación
> **TEXTO LITERAL** (Art. 53, líneas 3367-3384)
> "La Agencia puede revocar la certificación [...] si el responsable no da cumplimiento a lo establecido
> en este Párrafo. [...] Cuando un certificado ha sido revocado [...] para volver a solicitarlo el
> responsable [...] debe acreditar fehacientemente que la causal que dio origen a su revocación ha sido
> subsanada."

**Razonamiento aplicado:** revocación no es definitiva — se puede volver a solicitar la certificación
acreditando que la causal fue subsanada, pero exige prueba fehaciente, no una mera declaración de
intención.

---

## Título VIII — Del tratamiento de datos por el Congreso Nacional, Poder Judicial y organismos con autonomía constitucional (Arts. 54-55)

### Artículo 54 — Regla general del tratamiento de datos personales
> **TEXTO LITERAL** (Art. 54, líneas 3391-3435)
> "Es lícito el tratamiento de los datos personales que efectúan el Congreso Nacional, el Poder Judicial,
> la Contraloría General de la República, el Ministerio Público, el Tribunal Constitucional, el Banco
> Central, el Servicio Electoral y la Justicia Electoral, y los demás tribunales especiales creados por
> ley, cuando se realiza para el cumplimiento de sus funciones legales [...] con excepción de lo dispuesto
> en el artículo 14 quinquies y en los artículos 44 a 46 [...] Los funcionarios de estos organismos
> deberán guardar secreto de tales datos. [...]"

**Razonamiento aplicado:** régimen especial para órganos con autonomía constitucional — **no aplica a
SLEP**, que se rige por el Título IV general (Arts. 20-26) y sí queda sujeto a los Arts. 44-46 (a
diferencia de estos órganos, que están expresamente excluidos de esos artículos). No confundir este
régimen especial con el aplicable a un servicio público ordinario como un SLEP.

### Artículo 55 — Ejercicio de los derechos y reclamaciones
> **TEXTO LITERAL** (Art. 55, líneas 3437-3467)
> "Los titulares de datos ejercerán los derechos que les reconoce esta ley ante el Congreso Nacional, el
> Poder Judicial, la Contraloría General de la República, el Ministerio Público, el Banco Central [...] de
> acuerdo a procedimientos racionales y justos [...] En caso que la Contraloría [...] el Ministerio
> Público, el Banco Central o el Servicio Electoral denieguen injustificada o arbitrariamente el ejercicio
> de un derecho [...] el titular [...] podrá reclamar ante la Corte de Apelaciones, de acuerdo al
> procedimiento dispuesto en el artículo 43 [...]"

**Razonamiento aplicado:** régimen de reclamo especial (directo a Corte de Apelaciones, sin pasar por la
Agencia) — tampoco aplica a SLEP, que sigue el procedimiento general del Art. 41 (tutela ante la Agencia).

---

## Notas de precisión (para no heredar errores de fuentes secundarias)

1. Las sanciones **no** son "Art. 34 bis/ter/quáter" como clasificación general — **son la clasificación
   misma**: 34 (marco), 34 bis (leves), 34 ter (graves), 34 quáter (gravísimas); los **montos** están en
   el Art. 35 (privados) y en el Art. 44 (jefe superior de órgano público — % de su remuneración, no UTM).
2. El deber de reportar brechas (**Art. 14 sexies**) es "sin dilaciones indebidas" — **NO 72 horas**
   (estándar GDPR, no chileno).
3. DPO/MPI es **voluntario** por regla general (Art. 49) — obligatorio solo si se certifica un programa de
   cumplimiento (Reglamento Art. 6, segunda oración). El Art. 48 es deber general de prevención, no mandato
   de designar DPO — error frecuente de fuentes secundarias.
4. **Transferencias internacionales (Arts. 27-29)**: 3 vías generales + 8 excepciones puntuales — no basta
   "mencionarlo en el RAT" sin resolver bajo cuál vía se ampara cada transferencia.
5. **Título III (Arts. 17-19) — deudas educacionales expresamente excluidas** del régimen de boletín
   comercial, en cualquier nivel educativo — confirmado contra el texto íntegro de la Ley 19.628 original.
6. **Responsabilidad en SLEP es dual y acumulativa**: institucional sobre el jefe superior (Art. 44, %
   remuneración) + individual del funcionario infractor (Art. 45, Estatuto Administrativo + probidad).

## Grafo de esta skill (relación con otras)
Ver `## Grafo` en `SKILL.md` — este archivo es puramente de contenido normativo, no de enrutamiento entre
skills.
