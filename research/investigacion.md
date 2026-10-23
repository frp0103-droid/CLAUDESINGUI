# Fase 1: investigación

**Tema:** Francia, el movimiento lycéen y estudiantil de septiembre y octubre de 2026
**Información al 23/10/2026**
**Estado:** base factual cerrada. La parte de medios (§4 y §5) es **PRELIMINAR**: ver §0.

---

## 0. Limitaciones de acceso (leer primero)

| Qué | Situación | Consecuencia |
|---|---|---|
| Le Monde, Le Figaro, L'Humanité (y casi toda la prensa diaria francesa: Libération, La Croix, Ouest-France, Le Parisien, Les Échos, L'Opinion, 20 Minutes, regionales) | Bloquean el rastreador del buscador y el entorno no tiene salida de red hacia esos dominios | No pude leer ninguna nota completa ni conseguir URL originales. Los titulares que figuran abajo vienen de agregadores (titrespresse.com), de revistas de prensa (Cahiers pédagogiques) o de medios que citan a esos diarios (Acrimed, Le Devoir). |
| fr.wikipedia.org, Wikimedia Commons, franceinfo, etc. | La red del entorno solo permite npm, PyPI y GitHub | No pude abrir ninguna URL para verificarla. Todas aparecen en el buscador, pero ninguna se pudo abrir desde acá: en `fuentes.csv` figuran como `parcial`. |
| edge-tts (Microsoft) | Bloqueado | Para el voice over provisorio voy a usar TTS local. Igual vas a grabar con tu voz. |

**Cómo se destraba:** en la configuración del entorno (menú del entorno en la barra de título → *Edit* → *Network access*) hay que poner "Full", o agregar a *Allowed domains*: `lemonde.fr`, `lefigaro.fr`, `humanite.fr`, `wikipedia.org`, `wikimedia.org`, `titrespresse.com`, `franceinfo.fr`, `speech.platform.bing.com`. La otra opción es que me pases el texto o PDF de las notas.

---

## 1. Eje confirmado y pregunta guía

**Eje (verificado):** un movimiento que nace en un liceo de Créteil por **condiciones de estudio** (faltan profesores, aulas sobrecargadas, edificios deteriorados, horarios, Parcoursup), se vuelve **nacional** en diez días, **escala** a bloqueos con fuerte tensión policial y el **17/10 converge** con los gilets jaunes y los sindicatos contra la **vie chère**, a seis meses de la presidencial de abril de 2027.

Ajuste respecto de las pistas iniciales: el eje se sostiene, pero hay dos datos más recientes que conviene sumar.
- El movimiento ya **pasó a las universidades**: el 13/10, cerca del 90 % de las universidades estaban bloqueadas o cerradas preventivamente, según la Union syndicale (dato sindical).
- Hay **novedades del 22 y 23/10**: Macron recibe hoy, 23/10, a las organizaciones lycéennes; el gobierno presenta las primeras medidas el **lunes 26/10**; mañana, 24/10, hay nueva jornada ("acte II" de los gilets jaunes); los sindicatos convocan al **5/11**.

**Pregunta guía propuesta:** *¿Cómo pasó una protesta por la falta de profesores a convertirse en una crisis nacional, y cómo la cuenta cada diario según su línea?*

---

## 2. Hechos verificados: cronología

Cuando las cifras están en disputa, van las dos versiones. Fuente = id en `fuentes.csv`.

| Fecha | Hecho | Cifras | Fuente |
|---|---|---|---|
| 17/09 | Paro docente en el lycée Saint-Exupéry (Créteil) por puestos sin cubrir; al día siguiente, primer bloqueo de alumnos. Otras fuentes ubican el inicio el 21/09. | — | F01, F14 |
| 21/09 | Los diputados de LFI Louis Boyard y Clémence Guetté visitan el liceo. | — | F01 |
| 26/09 | Circular conjunta de Interior y Educación: intervención de las fuerzas de seguridad en caso de "bloqueo total". | — | F15 |
| 30/09 | Expansión nacional. | 356 liceos afectados; 625 detenidos en el día | F14 |
| 01/10 | "Acte II". Más de 900 acciones sobre ~3.700 liceos. Le Figaro publica una nota de inteligencia que atribuye la escalada a "LFI et ses proxys de l'ultragauche". LFI lo niega. Geffray anuncia una plataforma de consulta. | **1.949 detenidos** (Interior); 1.027 establecimientos afectados (Educación); 318 heridos (65 del personal, 170 alumnos, 83 policías), según el gobierno | F02, F03, F20, F21 |
| 02/10 | ~400 liceos cerrados preventivamente. Geffray recibe a tres organizaciones lycéennes (USL, Renouveau Lycéen, Lycéens!). Promete 3.000 profesores reemplazantes. | 1.027 concernidos / 560 perturbados / 400 cerrados (Interior) | F01, F04 |
| 04/10 | Carta del PM Lecornu a sus ministros: **5 frentes de trabajo** (asegurar las clases, condiciones dignas incluidas las olas de calor, tiempo escolar y edificios con las regiones, Parcoursup 2027, democracia lycéenne). Primeras decisiones "antes de fin de octubre". | — | F05 |
| 05/10 | Abre la consulta en la plataforma Agora (hasta el 23/10, anónima, open data). | **413 establecimientos perturbados a mediodía** y 589 en el día (Educación), contra ~800 el viernes 2/10 | F06, F07 |
| 06/10 | "Acte III": marcha nacional lycéenne y estudiantil. Lecornu suspende las clases a fin de semana para un "temps démocratique" en cada liceo. | **266.000 (Interior)** vs **450.000 (organizaciones)**. Wikipedia anota 256.000: ver nota ¹ | F08, F01, F22 |
| 07/10 | Geffray ante la Asamblea: 24 liceos incendiados o saqueados. Se suspenden las granadas de aturdimiento contra lycéens. Lecornu habla de "mouvement de violences urbaines". | — | F01, F09 |
| 08/10 | Interior señala un "aumento de las violencias urbanas". | 375 de 3.700 liceos con clases suspendidas a la mañana | F01 |
| 13/10 | "Acte V": jornada lycéenne, estudiantil y sindical. | **161.500 (Interior)** vs **480.000 (intersindical juvenil)** | F10 |
| 16/10 | Balance de reemplazos: 2.000 de los 3.000 profesores prometidos ya asignados. Tercera reunión con Geffray "sin acción concreta", según los lycéens. 165 miembros del personal heridos desde el inicio. | Acumulado de detenciones: 6.059 a 6.629 según la fecha | F11, F12 |
| 17/10 | **Convergencia**: lycéens + estudiantes + gilets jaunes + sindicatos contra la *vie chère*, convocada en redes (TikTok, cuenta "V2"). Empiezan las vacaciones de Toussaint. Violencia en París, Limoges (incendio del Hôtel de Ville), Niza, Lyon, Saint-Étienne. | **550.000 (Interior, Nuñez; 110.000 en París)** vs **800.000 (organizadores)**. Detenidos: **1.200**, balance provisorio de Lecornu (cifras posteriores más altas, sin consolidar). 150 policías y gendarmes heridos (provisorio). **2 muertos "en marge des manifestations"** según la Prefectura de Policía: uno por un malestar cardíaco cerca del cortejo, el otro sin detalles confirmados. | F13, F16, F17, F18 |
| 18/10 | Discurso de Macron (20 h, Élysée): firmeza ("rien ne le justifie…"), posibles prohibiciones de concentraciones, reunión de partidos, sindicatos y organizaciones juveniles bajo Lecornu. Dice que la plataforma ya supera las 100.000 participaciones. El SNES-FSU responde que "no avanzó nada concreto". | — | F19, F23 |
| 20–22/10 | Lecornu admite "défaillances": dispositivo "demasiado estático" y fallas de inteligencia. Toques de queda parciales (París, Lyon). Manifestaciones prohibidas en varias ciudades. Despliegue de la operación Sentinelle para el 24/10. Geffray anuncia ante la Asamblea las primeras decisiones para el **lunes 26/10** (dotación, reemplazos, Parcoursup). | — | F24, F25, F26 |
| 23/10 (hoy) | Cierra la consulta lycéenne. Macron preside un consejo de defensa y **recibe a las organizaciones lycéennes a las 15 h**. Les Lycéens!: "on n'attend pas grand-chose". | — | F27, F06 |
| Próximo | 24/10: nueva jornada ("acte II" gilets jaunes, Coordination nationale lycéenne). 26/10: medidas. 27/10: el Senado debate un proyecto que haría pagar hasta 10.000 € a quienes participen en concentraciones con daños. 5/11: jornada sindical. Abril de 2027: presidencial. | — | F28, F29, F20 |

¹ **Nota sobre el 6/10:** la cifra de Interior aparece como 266.000 en la nota de Le Monde replicada por titrespresse y en otros medios, y como 256.000 en Wikipedia. Para la pantalla propongo "266.000 según Interior" y dejar la discrepancia anotada en el anexo.

### Reivindicaciones (síntesis, fuentes F01, F11, F27)
1. Profesores y personal: puestos sin cubrir, reemplazos, enfermeras.
2. Aulas menos cargadas.
3. Edificios: renovación y adaptación al calor.
4. Horarios y ritmos escolares.
5. Parcoursup: abolición o reforma profunda; más plazas en la universidad.
6. Después del 17/10: costo de vida y servicios públicos.

### Hecho vs. interpretación (a separar en la presentación)
- **Hecho:** hubo violencia contra personas y edificios (24 liceos incendiados o saqueados, 165 miembros del personal heridos, más de 300 policías heridos al 1/10, según el gobierno). **También hecho:** hubo menores gravemente heridos: un chico de 16 años perdió el uso de un ojo en Tours y uno de 15 perdió una mano en Lens (Amnesty y prensa).
- **Interpretación en disputa:** que la escalada sea una "manœuvre organisée par LFI" (Matignon y nota de inteligencia revelada por Le Figaro) frente a "complotisme" (LFI) o "uso desproporcionado de la fuerza" (Amnesty, LDH).
- **Dato de opinión:** encuesta Odoxa-Backbone para Le Figaro: 62 % considera justificada la movilización y la mayoría desaprueba el rol de LFI (F20).

---

## 3. Contexto histórico: las causas contadas como historia

**a) Una escuela bajo presión (estructural)**
- Falta de profesores: la OCDE (*Regards sur l'éducation 2026*) habla de 2.900 puestos sin cubrir en Francia; los contractuales pasaron del 5 % (2018) al 7,1 % (2025) del cuerpo docente (F30).
- En la rentrée 2026, el ministro sostuvo "tendremos suficientes profesores" (96,1 % de puestos cubiertos en secundaria). La encuesta del SNES-FSU (1.033 establecimientos) encontró al menos un profesor faltante en el 53 % de los collèges y lycées (F31). Son cifras en disputa: hay que mostrar las dos.
- Presupuesto: 1.803 puestos docentes de secundaria suprimidos para la rentrée 2026, según el SNES-FSU (parte interesada) (F32).
- Parcoursup (desde 2018): la plataforma de admisión a la universidad, percibida como opaca y selectiva. Es una reivindicación central desde 2018 (F01, F05).

**b) El costo de vida (coyuntural)**
- Inflación de septiembre de 2026: ~3 % interanual (estimación INSEE del 30/09), la más alta desde febrero de 2024, empujada por la energía (+21,2 % interanual). Gasoil récord: 2,41 €/l el 20/09, ligado al conflicto en Medio Oriente y al estrecho de Ormuz (F33). *Verificar en insee.fr cuando haya red.*
- Eco con 2018: los gilets jaunes nacieron por un aumento del impuesto a los combustibles (TICPE). La sociología los describe como una crisis de los hogares populares periurbanos y una revuelta contra impuestos vividos como injustos (Alexis Spire, CNRS; CEVIPOF/Sciences Po) (F34).

**c) Precedentes**
- **Mayo del 68:** referencia simbólica. Algunos carteles de 2026 dicen "Génération 6/7 refait Mai 68" (Le Figaro, vía titrespresse). El historiador Robi Morder (UVSQ, GERME) participó de los Comités d'action lycéens en el 68 (F35).
- **Diciembre de 2018, Mantes-la-Jolie:** 151 a 153 lycéens detenidos y obligados a arrodillarse con las manos en la nuca, en medio de un movimiento contra Parcoursup y la reforma del bac, en paralelo a los gilets jaunes. La investigación de la IGPN se archivó (F36). Es el antecedente directo de la convergencia lycéens + gilets jaunes.
- Otros momentos lycéens: 1986 (ley Devaquet), 2005 (ley Fillon), 2006 (CPE), 2010 (jubilaciones). Morder: "la jeunesse est une plaque sensible de notre société" (F35).

**d) Lo inédito de 2026** (análisis académico, F37, F38)
- La organización nace en TikTok y Snapchat y se propaga en red (Valérie Becquet, socióloga).
- Hay una "sobrecarga de incertidumbre": deuda, costo de vida, desempleo, clima, guerra.
- Hay un clima de "alegría política", lejos de la imagen de una generación "angustiada" (Libération; Politis, prensa militante).

**e) Calendario político**
- Gobierno Lecornu (PM), Édouard Geffray (Educación), Laurent Nuñez (Interior). Presupuesto 2027 en debate: Lecornu promete enmiendas a partir de la consulta (F39).
- Presidencial: primera vuelta prevista para el 11 o el 18 de abril de 2027 (falta el decreto). En las encuestas de septiembre, Marine Le Pen aparece primera y Édouard Philippe y Jean-Luc Mélenchon empatan en torno al 16-17 % (F40). Los candidatos ya se posicionan sobre Parcoursup: Le Pen, Polony (F41).
- Los lycéens de 16 o 17 años **no votan en 2027** o votan por primera vez. Una de las consignas de la convocatoria del 17/10 apeló a "los jóvenes que no pueden votar" (Sud Radio).

---

## 4. Los tres medios: selección y justificación ⚠ PRELIMINAR

Las clasificaciones se apoyan en fuentes externas: Wikipedia, que remite a la historia y la propiedad de cada diario; la cartografía "Médias français : qui possède quoi" (Acrimed / Le Monde diplomatique); y el Reuters Institute Digital News Report 2026 (Francia).

| | **L'Humanité** | **Le Monde** | **Le Figaro** |
|---|---|---|---|
| Línea | Izquierda (histórica y comunista) | Centro / diario de referencia ("journal de référence") | Centroderecha / derecha |
| Historia | Fundado en 1904 por Jean Jaurès. Órgano del PCF hasta 1994 (F42). | Fundado en 1944 por Hubert Beuve-Méry (F43). | Fundado en 1826, el diario nacional más antiguo todavía publicado (F44). |
| Propiedad | Sociedad editora propia, ligada históricamente al PCF (F42). | Groupe Le Monde. Accionista principal: Xavier Niel (holding Le Monde Libre). La Société des rédacteurs tiene derecho de veto sobre el director (F43, F45). | Groupe Dassault, desde 2004 (F44, F45). |
| Por qué | Da voz a lycéens, sindicatos y docentes. Lectura social del conflicto. | Diario de calidad de mayor alcance digital (más de 600.000 suscriptores digitales) y referencia de confianza (F46). | Segundo diario nacional (315.000 suscriptores digitales). Lectura de orden público. Publicó la nota de inteligencia sobre LFI (F46). |

**Reemplazo posible:** si se habilita la red y algún diario resulta inaccesible por el paywall, el reemplazo natural del polo izquierdo es *Libération*: fundado en 1973 por Sartre y Serge July, hoy en un fondo de dotación tras su salida del grupo Altice.

---

## 5. Notas identificadas por medio ⚠ ANÁLISIS PARCIAL (sin texto completo ni URL original)

Solo se registran titulares que aparecen literalmente en las fuentes intermedias. **Autor y URL original: pendientes.** Ninguna cita es inventada; las expresiones entre comillas son las que reproducen las fuentes intermedias.

### L'Humanité
| # | Titular (tal como aparece) | Fecha aprox. | Momento | Vía |
|---|---|---|---|---|
| H1 | « On ne nous écoute jamais » : les lycéens en lutte racontent leur quotidien | ~15/10 | Causas | titrespresse + video en YouTube de L'Humanité |
| H2 | « La jeunesse continue de se battre, de sourire et de chanter » : lettre… (texto de la lycéenne Maïa Boudeau) | ~23/10 | Actualidad / represión | titrespresse |
| H3 | Pieza de la edición del 24/10 sobre la reacción de Macron ("un nuevo paso en la represión", paráfrasis) | 23-24/10 | Futuro | titrespresse (titular sin confirmar) |

**Lectura preliminar:**
- (a) **Causas:** déficit de medios (aulas sobrecargadas, falta de profesores, liceos vétustes, la vía profesional abandonada), contado por los propios lycéens.
- (b) **Actualidad:** da voz a los alumnos y pone en primer plano la represión policial.
- (c) **Futuro:** responsabiliza al Ejecutivo y su giro hacia la represión.

### Le Monde
| # | Titular | Fecha aprox. | Momento | Vía |
|---|---|---|---|---|
| M1 | Mouvement lycéen : la mobilisation s'amplifie et agrège de nombreux soutiens | 6-7/10 | Origen / expansión | titrespresse (cita "266.000 según Interior vs 450.000") |
| M2 | Tribuna de un colectivo de sociólogos de la Universidad de Tours (encuesta de campo con lycéens) | ~10/10 | Causas | Cahiers pédagogiques, revista de prensa del 11/10 |
| M3 | *pendiente:* nota del 17/10 o posterior (balance y medidas) | — | Pico / futuro | — |

**Lectura preliminar:**
- (a) **Causas:** degradación de las condiciones de estudio, con fundamento académico.
- (b) **Actualidad:** perfiles diversos, apoyo de adultos (padres, electos, sindicalistas), las dos cifras de asistencia y la aclaración de que la mayoría de las movilizaciones fue sin enfrentamientos.

### Le Figaro
| # | Titular / pieza | Fecha aprox. | Momento | Vía |
|---|---|---|---|---|
| F-a | Revelación de una nota del renseignement parisien: "instrumentalisation" del movimiento por LFI, posible "stratégie d'embrasement" | 01/10 | Origen | Acrimed (7/10), Le Devoir |
| F-b | Encuesta Odoxa-Backbone: 62 % considera justificada la movilización y desaprueba a LFI | ~5/10 | Actualidad | Le Devoir, Acrimed |
| F-c | Colère sociale : conseil de défense et rencontre avec les lycéens au programme d'Emmanuel Macron avant une nouvelle mobilisation le 24 octobre | 23/10 | Futuro | titrespresse |
| (extra) | Les slogans, nouveau terrain de jeu linguistique des lycéens / « On est là pour maintenir la pression », affirme Fabio Lapotre (MNL) | oct. | Color / voz lycéenne | titrespresse |

**Lectura preliminar:**
- (a) **Causas:** reconoce un malestar (la encuesta), pero pone el foco en la instrumentalización política.
- (b) **Actualidad:** orden público, violencia, fuentes policiales y de inteligencia.
- (c) **Futuro:** respuesta securitaria (consejo de defensa) más diálogo.

> ⚠ Estas lecturas son **hipótesis de trabajo**: hay que confirmarlas con el texto completo antes de llevarlas al guion. Lo que sí está documentado por fuentes externas: Acrimed acusa a buena parte de la prensa de priorizar la violencia (en el JT de France 2, 8 % del tiempo a las reivindicaciones y 75 % a la violencia y los daños) y critica a "l'éditocratie" por el relato del complot de LFI. Además, 780 estudiantes de periodismo firmaron una tribuna contra la cobertura (F47, F48). Acrimed es parte interesada (crítica de medios, de izquierda).

---

## 6. Comparativo (borrador, se completa con los textos)

| Eje | L'Humanité | Le Monde | Le Figaro |
|---|---|---|---|
| Encuadre | Lucha social legítima y represión | Movimiento amplio con apoyos transversales | Orden público e instrumentalización política |
| Vocabulario esperado | "lutte", "jeunesse", "répression" | "mobilisation", "soutiens", "lycéens" | "violences", "ultragauche", "blocus" |
| A quién da voz | Lycéens, docentes, sindicatos | Lycéens, académicos, adultos que apoyan | Gobierno, inteligencia, encuestas, algunos lycéens |
| Cifras que prioriza | Heridos y detenidos (represión) | Las dos cifras (Interior y organizadores) | Daños, detenidos, policías heridos, encuesta |
| Responsable | Gobierno | Repartido / estructural | LFI y la ultraizquierda; también el gobierno, por laxitud |
| Tono hacia el gobierno | Crítico | Distante / analítico | De apoyo crítico (firmeza) |
| Tono hacia los manifestantes | Empático | Descriptivo | Separa a los lycéens de los "casseurs" |
| **Coincidencias** | Los tres reconocen reivindicaciones reales sobre la escuela y el peso del 17/10. | | |

---

## 7. Otras fuentes (no periodísticas)
Detalle completo en `fuentes.csv`:
- Institucionales: education.gouv.fr, elysee.fr, Assemblée nationale, INSEE, OCDE, Reuters Institute (Oxford).
- ONG: Amnesty France y Amnesty International, LDH, FCPE.
- Sindicatos: SNES-FSU.
- Académicas: The Conversation, Robi Morder (UVSQ/GERME), Valérie Becquet, Alexis Spire (CNRS), CEVIPOF.
- Observatorio de medios: Acrimed.
- Base factual: franceinfo (servicio público) y AFP vía Bourse Direct.

Cada fuente lleva marcado su tipo y si es **parte interesada**.
