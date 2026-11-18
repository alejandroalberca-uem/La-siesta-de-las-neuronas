# La Siesta de las Neuronas — Documento de diseño (v0.1)

> Título de trabajo. Aventura gráfica retro de Neuropsicología en PT, con humor y sarcasmo al estilo *Return to Monkey Island*.

## 1. Idea en una frase
Un alumno se queda dormido en la clase de Neuropsicología y despierta dentro de una neurona. Para despertar tiene que cruzar cinco mundos (uno por unidad), resolver casos clínicos famosos y sobrevivir a mentores que lo tratan con una ironía muy cariñosa.

## 2. Tono
- Humor seco y autoconsciente: el protagonista comenta con sarcasmo la propia asignatura («diapositiva 47 de 80»).
- Los mentores son brillantes y un poco insoportables.
- **Los pacientes históricos se tratan con respeto.** Se hace humor *con* ellos y *sobre la situación del alumno*, nunca sobre su enfermedad o su sufrimiento.
- Todo el humor está al servicio de recordar el concepto: el chiste y la regla clínica van en la misma frase.

## 3. Estructura

**Prólogo (en el prototipo).** Clase → puzle para dormirse → sueño → hub (la neurona) con Cajal.

**Hub.** El axón de una neurona gigante, con cinco puertas. Cajal da pistas y comenta el progreso.

### Mundos (propuesta a validar con tus contenidos)

| Unidad | Mundo | Temas (según tus PPT) | Mentor | Caso |
|---|---|---|---|---|
| U1 | El Pasillo de los Neuromitos | Neuropsicología y educación, neuromitos, infanto-juvenil vs. adulto | Cajal (hub) | Phineas Gage |
| U2 | El Bosque de las Neuronas | Histología, organización del SN, lateralización | Cajal | — |
| U3 | La Galería de los Espejos | Percepción y agnosias, praxias, lenguaje | Luria | Tan (Broca), caso de la llave |
| U4 | La Biblioteca sin Fin | Atención, memoria y aprendizaje, funciones ejecutivas | Goldberg | H.M. |
| U5 | El Carnaval Límbico | Emoción y sistema límbico, cognición social, conciencia, teoría de la mente | por decidir | Gage regresa |

Los mentores y casos están **pendientes de tu validación**: son una propuesta, no contenido sacado de tu temario.

**Final.** Un caso integrador que sirve de repaso.

## 4. Mecánicas
- **Verbos:** Mirar, Llevar, Hablar, Usar (y clic en el inventario para combinar).
- **Diálogos con opciones,** al estilo clásico.
- **Puzles de contenido** (la idea es que el puzle *sea* el aprendizaje):
  - Localizar la lesión a partir de los síntomas.
  - Emparejar síntoma con área o función.
  - Descartar causas antes de etiquetar (por ejemplo, agnosia).
  - Ordenar un circuito o modelo funcional.
  - Elegir una adaptación educativa para un alumno concreto.
- **Cuaderno del alumno** (el inventario conceptual): cada concepto resuelto se anota como ficha de repaso, que se puede usar para estudiar.
- **Sin muerte y sin penalización.** Fallar da una pista, no pierde progreso.

## 5. Dirección de arte
- Pixel-art de baja resolución (480×270 escalado), con **una paleta cerrada por mundo**.
- Mucha luz: ventanas, brillos y partículas (sinapsis, polvo en suspensión).
- Parallax en los fondos y animaciones sutiles.
- Retratos grandes y expresivos para los mentores.
- Música propia y sonido ambiente por mundo.

Los sprites del prototipo son **provisionales**. El arte final requiere un proceso aparte (ver siguiente sección).

## 6. Técnica
- Web, HTML5 sin instalación, jugable desde el móvil (igual que Mundafall).
- Prototipo: JavaScript y canvas, un solo archivo.
- Producción: Phaser o Godot (exportación web), con datos de diálogos y puzles en archivos separados para que puedas editar los textos.

## 7. Hoja de ruta
1. **Prólogo** (este prototipo): validar tono y estética.
2. **Mundo U3 «Galería de los Espejos»** (**hecho en el prototipo**, ver sección 9).
3. **Mundo U4 «Biblioteca sin Fin»** (hecho, sección 10) y **mundo U5 «Carnaval Límbico»** (hecho, sección 11). Mundos U2 (sección 12) y U1 «Pasillo de los Neuromitos» (sección 13): hechos. **Los cinco mundos originales están completos y el juego tiene final.** Con el material 2026 se añadió un sexto mundo (U6, sección 14).
4. Sonido, música, pulido y pruebas con alumnos.

## 8. Decisiones abiertas
- Mentores y casos concretos por unidad.
- Si el juego cuenta para la nota o es solo repaso voluntario.
- Cómo se produce el arte final (artista, herramientas de IA para generar fondos con revisión manual, etc.).

## 9. Mundo 3 · La Galería de los Espejos (implementado)

Mentor: **Luria** (su modelo sistémico-funcional aparece en U3T3). Aparece dentro de un espejo de mano en cada ala para dar pistas.
Fuentes: `Boveda/Unidad 3/26/` (U3T1 percepción y agnosias, U3T2 praxias, U3T3 lenguaje y Kahoot).

| Ala | Caso didáctico | Puzle | Contenido evaluado |
|---|---|---|---|
| Sala de las Llaves | Tomás (caso de la llave, U3T1 diap. 2) | Explorar 4 pruebas + 4 decisiones | Niveles estímulo → representación → significado, agnosia asociativa, regla de oro «descartar antes de etiquetar», apoyos en el aula |
| Taller de las Manos | Nico, 8 años (TDC) | Clasificar 4 errores + 3 decisiones | Praxias ideatoria, ideomotora, melocinética y constructiva; TDC ≠ apraxia adquirida; neuronas espejo; «integrar reflejos» |
| Salón de las Palabras | Julián, 65 años (afasia de Broca, U3T3 diap. 14) | Explorar 4 pruebas + 6 decisiones | Perfiles Broca/Wernicke/conducción, lenguaje ≠ pensamiento, doble ruta de lectura, dosis de terapia, MIT, TCS vs. TDL |
| Espejo Mayor (final) | — | Ordenar 5 decisiones | Entrada → representación → significado → diferencial → función (U3T1 diap. 24) |

- Cada acierto añade una ficha al **Cuaderno** (15 fichas en total; se guardan en el navegador).
- Los nombres de los pacientes (Tomás, Nico, Julián) y los diálogos son míos: el temario solo describe los casos de forma anónima.
- El caso del doctor P. (U3T1 diap. 20), el caso pediátrico TEA ≠ agnosia auditiva y los casos de TDL y dislexia quedan libres para ampliar el mundo.

## 10. Mundo 4 · La Biblioteca sin Fin (implementado)

Mentor: **Goldberg**, representado como director de orquesta (la metáfora «director de orquesta» de tu U4T3). Se presenta como alumno de Luria. **Tu temario no menciona a Goldberg**: es una elección de diseño tuya, no un contenido de las diapositivas.
Fuentes: `Boveda/Unidad 4/` (U4T01 atención, U4T21 memoria y aprendizaje, U4T3 funciones ejecutivas).
Estructura igual que el mundo 3: tres salas, una hoja de partitura por sala, y puzle final en el atril. Las pistas las da el metrónomo de cada sala.

| Sala | Caso | Puzle | Contenido evaluado |
|---|---|---|---|
| Sala del Faro | Lola, 9 años, hemiplejia izquierda (caso didáctico, U4T01 diap. 12 y 14) | Explorar 4 pruebas + 6 pasos | Heminegligencia y estrategia educativa, redes de Posner (orden alerta → orientación → ejecutiva), tipos de atención de Sohlberg y Mateer, desarrollo de la atención |
| El Archivo | H. M. (caso histórico, U4T21 diap. 33) | Explorar 3 pruebas + 6 pasos | Hipocampo, amígdala y prefrontal, memoria procedimental, aprendizaje clásico, 7 ± 2 y chunking, falsas memorias, dismnesia evolutiva |
| El Foso de la Orquesta | Quique, 10 años (caso didáctico, U4T3 diap. 31) | Explorar 4 pruebas + 8 pasos | Identificación de funciones ejecutivas en el aula, planificación, mito del lóbulo frontal, frías y calientes, semáforo, docente como lóbulo frontal externo |
| Atril (final) | — | Ordenar 5 pasos | Resolución de problemas de Burgess (U4T3 diap. 19) |

- 16 fichas nuevas en el Cuaderno.
- **H. M.** se trata con respeto explícito en el texto. Las pruebas del caso (no reconoce a quien acaba de conocer, mejora una habilidad motora, repite números si es inmediato) son una **síntesis mía** a partir de lo que dice tu diapositiva («sin hipocampo, un eterno presente») y de tu clasificación de la memoria; tu temario no detalla el caso.
- Los nombres Lola y Quique y los diálogos son míos.

## 11. Mundo 5 · El Carnaval Límbico (implementado)

Mentor: **Darwin** (propuesta mía: tu U5T01 lo cita como pionero y por la universalidad de la expresión). Aparece junto a una lupa en cada carpa para dar pistas.
Fuentes: `Boveda/Unidad 5/` (U5T01 emoción y sistema límbico, U5T23 cerebro social, conciencia y teoría de la mente).
Estructura igual que los mundos 3 y 4: tres carpas, un billete por carpa, puzle final en el carrusel.

| Carpa | Caso | Puzle | Contenido evaluado |
|---|---|---|---|
| El Túnel del Miedo | Álvaro (caso didáctico, lesión de amígdala) | Explorar 4 pruebas + 6 pasos | Amígdala, James-Lange y Cannon-Bard, circuito de Papez (orden), función adaptativa del sobresalto, emociones básicas de Ekman |
| El Teatro de las Máscaras | Phineas Gage (histórico), Marta y Raúl (didácticos) | Explorar 3 pruebas + 6 pasos | Orbitofrontal, frontomedial y dorsolateral, lateralización, paresia facial emocional/volitiva, autismo y mirada |
| La Carpa de las Mentes | Leo (3 años) y Nora (5 años), didácticos | Explorar 4 pruebas + 7 pasos | Falsa creencia (Sally y Anne), hitos de la teoría de la mente (orden), empatía afectiva, neuronas espejo e intención, red del cerebro social, niveles de conciencia, claves sociales |
| Carrusel (final) | — | Ordenar 3 pasos | Niveles de procesamiento emocional (U5T01 diap. 20) |

- 14 fichas nuevas en el Cuaderno.
- Phineas Gage aparece en tu clase de U1 (corregido 17/11/2026); en este mundo su conducta se construye solo a partir de lo que tu U5T01 dice de la lesión orbitofrontal.
- Los nombres Álvaro, Marta, Raúl, Leo y Nora y los diálogos son míos.
- Pendientes: mundos U1 (Neuromitos) y U2 (Bosque de las Neuronas).

## 12. Mundo 2 · El Bosque de las Neuronas (implementado)

Mentor: **Cajal** (el mismo del hub, ahora en su laboratorio al aire libre). Las pistas las da su microscopio.
Fuentes: `Boveda/Unidad 2/` (U2T1 organización del SN, UA2_T_02 sistema neuroendocrino, U2T3 lateralización).
Estructura igual que los mundos 3, 4 y 5: tres claros, una lámina de microscopio por claro y puzle final en el microscopio.

| Claro | Caso | Puzle | Contenido evaluado |
|---|---|---|---|
| El Claro de las Neuronas | Nerea, una neurona (didáctica) | Explorar 4 pruebas + 7 pasos | Neuronas y glía, velocidad y conducción saltatoria, potencial de acción y sinapsis (orden), neurotransmisores, neurogénesis (orden), capas corticales, neuroplasticidad |
| La Torre de Control | Teodoro, cartógrafo (didáctico) | Explorar 4 afirmaciones + 7 pasos | Planos y orientación, jerarquía cortical (orden), prosencéfalo, SNP (31+12), hipófisis, eje del estrés (orden) |
| El Teatro de los Hemisferios | Marcos, 9 años (didáctico) | Explorar 4 pruebas + 7 pasos | Neuromitos de la lateralidad, zurdera y lenguaje, red del lenguaje, qué hacer en educación, índice de lateralización, «dominante» |
| Microscopio (final) | — | Ordenar 4 pasos | Frontera 2024-2026 de la lateralidad (U2T3 diap. 19) |

- 18 fichas nuevas en el Cuaderno.
- Quedan fuera los contenidos que en U2T1 están solo en imágenes.
- Con esto están todos los mundos salvo **U1 (Neuromitos)**.

## 13. Mundo 1 · El Pasillo de los Neuromitos y final del juego (implementado)

Mentor: **el Profe** (propuesta mía: el mismo profesor caricaturizado de la clase del prólogo, para cerrar el círculo). Las pistas las da un mando de Kahoot.
Fuentes: `Boveda/UNidad 1/2026/` (U1T2 y U1T3).
Estructura igual que el resto: tres aulas, una tiza por aula y puzle final en la pizarra.

| Aula | Caso | Puzle | Contenido evaluado |
|---|---|---|---|
| Sala de las Definiciones | Phineas Gage (histórico, símbolo) | Explorar 4 preguntas + 7 pasos | Definición de neuropsicología, relación con la educación, neuromitos (estilos, hemisferios, 10 %), mitos de la neuroplasticidad, tipos de plasticidad |
| Sala del Desarrollo | Pablo, 12 años (didáctico) | Explorar 4 revisiones + 6 pasos | Neuropsicología infanto-juvenil frente a adultos, «pequeños adultos», baremos, periodo crítico y sensible, clasificación de los trastornos del neurodesarrollo |
| Sala del Informe | Iván, 10 años (caso didáctico ficticio) | Explorar 4 revisiones + 7 pasos | Lectura de un informe: disparidad de índices, perfil verbal/no verbal, memoria por repetición, funciones ejecutivas, medicación, lenguaje que oculta déficits y neuropsicología escolar |
| Pizarra (final) | — | Ordenar 3 pasos | Autoconocimiento → autogestión → autorregulación (U1T3 diap. 13) |

- 14 fichas nuevas en el Cuaderno (el Cuaderno completo suma 77).
- **Final del juego:** al completar los cinco mundos, Cajal se despide, el protagonista despierta en clase con el Profe, y aparece la pantalla de FIN.
- **Caso ficticio:** el caso real (anonimizado) del Sr. A de tu U1T3 se ha sustituido por Iván, inventado; se conservan los mismos aprendizajes sin datos de ningún paciente real.


## 14. Mundo 6 · El Gabinete de Evaluación (nuevo, material 2026)

La Unidad 6 (evaluación neuropsicológica) llegó en la carpeta `Unidad 6/26`. Es la **puerta 6** del hub, que pasa a tener seis puertas.
Mentor: **Wechsler** (propuesta mía: tus diapositivas citan las escalas Wechsler, no a la persona). Las pistas las da una balanza.
Estructura igual que el resto: tres salas, un sello por sala y puzle final en el informe.

| Sala | Caso | Puzle | Contenido evaluado |
|---|---|---|---|
| Despacho (principios) | Sara, 9 años (didáctico; basado en el caso ficticio de U6T01) | Explorar 4 fuentes + 8 pasos | Definición, entrevista, validez ecológica, estandarizadas y específicas, informe adaptado, qué hace el docente con un informe, las pruebas no bastan |
| Almacén de Pruebas | Nacho, 8 años (basado en el caso ficticio de U6T02) | Explorar 4 revisiones + 8 pasos | d2, BRIEF-2 frente a ENFEN, índices del WISC-V, escalas de inteligencia, Stroop, PROLEC-R, AULA, cómo leer un informe |
| Sala de Registros | Álex, 10 años (basado en el caso ficticio de U6T03) | Explorar 4 pruebas + 8 pasos | Perfil de estrés, EMG frente a MEG, estructural frente a funcional, EEG, qEEG y TDAH, MEG, Marek, medidas de aula |
| Informe (final) | — | Ordenar 6 pasos | Proceso de evaluación (U6T01 diap. 10) |

- 24 fichas nuevas en el Cuaderno (total del juego: unas 100).
- El **final del juego** ahora exige completar los seis mundos.

## 15. Actualización con el material 2026 (U4, U5 y U6)

Resumen completo de las diferencias del material en `Boveda/CAMBIOS_26.md`. Cambios en el juego:

- **U4:** Miller con la nota de Cowan (~4); el desarrollo de la atención ya no se da por completo a los 7 años; estrategia de negligencia reformulada (tus dos diapositivas no coinciden: ver `REVISION_U4.md`); pasos nuevos: Stroop, Cochrane 2021, TDAH (Alati), amnesia infantil (Yates), práctica de recuperación y entrenamiento de FE; DUA 3.0 en las fichas.
- **U5:** Darwin y la universalidad de la expresión ahora discutida; pasos nuevos: Barrett, LeDoux y Pine, Rolls, alexitimia, regulación en el aula, doble empatía y conciencia encubierta; **neuronas espejo reescritas** (Heyes y Catmur, 2022).
- **U6:** mundo nuevo.
- Los documentos `REVISION_U4.md`, `REVISION_U5.md` y `REVISION_U6.md` se han regenerado e incluyen arriba lo que cambió.
