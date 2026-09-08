# página 9 — de aepd-exactitud-calidad-datos-ia-2026.pdf

 
 
 
Página: 9 de 23 
Otros casos podrían ser tratamientos de análisis de tendencias, de correlaciones, 
optimizaciones, asignación de recursos, desarrollo de modelos, toma de decisiones en políticas 
públicas o análisis de riesgos en ámbitos como la logística, la educación, las finanzas, la energía, 
la movilidad, la sanidad, la ciencia, etc. 
En estos casos, en la medida que el conjunto de datos contenga datos personales, el principio 
de exactitud-RGPD debe tener en cuenta características tan importantes como que los datos, 
tomados en su conjunto, no contengan sesgos que comprometan la finalidad del tratamiento. 
Así pues, en sistemas de inteligencia artificial, la calidad del dato debe evaluarse también al 
nivel del conjunto de datos (“dataset”), pues resulta esencial para garantizar el correcto 
funcionamiento del sistema y, por lo tanto, cumplir con la finalidad del tratamiento que supone su 
desarrollo. Ello sin perjuicio de la calidad del dato individual, por cuanto produzca efectos sobre 
las personas.  
El responsable del tratamiento, bajo el principio de exactitud y de responsabilidad proactiva, 
deberá garantizar y documentar la trazabilidad del conjunto de datos utilizado, incluyendo el 
origen de los datos, las transformaciones aplicadas y los criterios de selección y exclusión.  
F. CALIDAD DE LOS DATOS VS VERACIDAD Y ACTUALIDAD 
La calidad del conjunto de datos para una finalidad específica, en cuanto a datos personales, 
puede estar relacionada con la veracidad y actualidad de estos. No obstante, el RGPD es incluso 
explícito en que la actualidad del dato personal es un requisito de exactitud-RGPD sólo cuando sea 
necesario para cumplir con la finalidad del tratamiento. 
La aplicación sobre un conjunto de datos personales de técnicas para la eliminación de sesgos, 
de técnicas de anonimización (no solo para anonimizar, sino para minimizar datos), de técnicas de 
privacidad diferencial o la generación de datos sintéticos puede implicar que algunos valores no 
reflejen directamente la realidad de un individuo o no cumplan determinados criterios técnicos de 
exactitud-ISO. Sin embargo, el conjunto de datos resultante puede tener la calidad suficiente 
como para ser utilizada como entrada en todas o algunas de las fases de desarrollo de un sistema 
de IA basado en ML. Es decir, el conjunto de datos puede considerarse que cumple con el principio 
de exactitud-RGPD en la medida en que resulte adecuado para la finalidad del tratamiento, sin que 
ello suponga prescindir de las exigencias de veracidad cuando estas sean relevantes.  
Es más, existen técnicas para incrementar la calidad del conjunto de datos que pueden implicar 
la utilización de valores que no reflejen directamente la realidad individual. Así, por ejemplo, 
puede considerarse un conjunto de datos formado por registros con múltiples campos en el que 
algunos de ellos están vacíos o incompletos (problemas de completitud). Una técnica para 
aumentar la calidad del conjunto de datos es estimar el posible valor de los campos vacíos 
extrapolándolo de medidas estadísticas obtenidas del resto de registros. Esta es una técnica 
adecuada, pero introduce valores formalmente falsos e inexactos, sacrificando la exactitud-ISO 
por la completitud-ISO. 
 
Figura 5 En la tabla de la izquierda existen campos que no estaban completados en origen. Se puede completar 
la tabla de datos con distintas estrategias. En la tabla del centro se ha elegido introducir la media de los 
sueldos de toda la tabla. En la derecha se han utilizado las medias de los sueldos de la misma provincia. 
COMPLET ADO CON LA MEDIA       COMPLET ADO CON MEDIA POR  PR OVINCIA
ID
PR OVINCIA
SUELDO
EXP.
PR OVINCIA SUELDO
EXP.
PR OVINCIA SUELDO
EXP.
ID1
MAD
57400
Medio
MAD
57400
Medio
MAD
57400
Medio
ID2
VAL
-
Bajo
VAL
65150
Bajo
VAL
22250
Bajo
ID3
GR
90000
Alto
GR
90000
Alto
GR
90000
Alto
ID4
VAL
36900
Bajo
VAL
36900
Bajo
VAL
36900
Bajo
ID5
BCN
-
Medio
BCN
65150
Medio
BCN
45000
Medio
ID6
VAL
7600
Alto
VAL
7600
Alto
VAL
7600
Alto
ID7
VAL
-
Bajo
VAL
65150
Bajo
VAL
22250
Bajo
ID8
BCN
45000
Bajo
BCN
45000
Bajo
BCN
45000
Bajo
CONJ UNT O DE DAT OS OR IG INAL

[1 imágenes en esta página]
