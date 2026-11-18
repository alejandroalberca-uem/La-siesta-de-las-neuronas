# Biblia de personajes · La Siesta de las Neuronas

Documento para diseñar los personajes con ChatGPT y Gemini. Recoge **todos** los personajes del juego tal y como están ahora, con su papel, su personalidad, una descripción visual lista para pegar en un generador de imágenes y los colores del prototipo.

> Los sprites actuales son **provisionales** (rectángulos). Los colores indicados son los del prototipo: úsalos como punto de partida, no como obligación.

---

## 0. Antes de empezar

### Estilo general del juego
- **Aventura gráfica retro con humor y sarcasmo** (referencia: *Return to Monkey Island*).
- Pixel-art de baja resolución (pantalla de 480×270), con **una paleta cerrada por mundo** y mucha luz.
- Personajes de cuerpo entero de unos **40×44 px** en pantalla, más un **retrato grande** (96×96 o más) para los mentores en los diálogos.
- Siluetas muy legibles: cada personaje debe distinguirse a 32 px por su silueta y su color dominante.

### Plantilla de prompt (pégala delante de cada personaje)
```
Pixel art character sprite, retro point-and-click adventure game style (LucasArts / Return to Monkey Island feel), 
limited color palette, clean 1px dark outline, front-facing 3/4 view, full body, neutral idle pose, 
transparent or flat solid background, no text, no watermark. Humorous but respectful tone.
Character: <PEGA AQUÍ LA DESCRIPCIÓN DEL PERSONAJE>
```
Y, para el retrato de diálogo:
```
Pixel art portrait, bust, 96x96 style, expressive face, same style and palette as above. Character: <...>
Generate 4 expressions: neutral, amused, skeptical, surprised.
```

### Consejos para que salgan coherentes
1. **Genera primero un personaje y úsalo como referencia** (sube la imagen) para el resto: así mantienes el estilo.
2. Pide siempre **hoja de personaje** (frente, tres cuartos, perfil, espalda) y **cuatro expresiones**.
3. Fija una paleta por mundo (hex) y pídesela explícitamente a la IA.
4. Revisa a mano al final: las IA suelen colar detalles que no son pixel-art real. Conviene pasar el resultado por un limpiador de pixel-art o rehacerlo con un artista.

### Precauciones importantes
- **Personas reales:** Cajal, Luria, Goldberg, Darwin y Wechsler son personas reales, y Phineas Gage y H. M. fueron pacientes reales. Pide siempre una **caricatura estilizada**, nunca un parecido fotográfico. Algunos generadores se niegan a dibujar personas reales: describe sus rasgos (barba, gafas, boina…) en vez de usar el nombre.
- **Goldberg** (Elkhonon Goldberg) parece seguir vivo: conviene contar con su visto bueno antes de publicar una caricatura suya.
- **Phineas Gage y H. M.** deben representarse con respeto: **personas, no curiosidades médicas**. Nada de imágenes impactantes ni de la lesión.
- **Casos infantiles y casos clínicos (didácticos):** son ficticios, pero se tratan con respeto. Evita caricaturizar su dificultad (ni estereotipias, ni rasgos que ridiculicen).
- **Conviene evitar rostros reconocibles de personas reales de tu entorno** (compañeros, alumnado) en los diseños.

### Dos cosas a decidir antes de diseñar
1. **Hay dos «Marcos»**: uno es un alumno de la clase del prólogo (dibuja cerebros con patillas) y otro es un niño de 9 años zurdo del mundo 2. **Propuesta:** renombrar a uno (por ejemplo, el de la clase pasaría a llamarse «Mario»).
2. **Varios personajes comparten colores en el prototipo** (Lola, Marta y Sara usan el mismo rosa y el mismo pelo). En el diseño final deberán ser **claramente distintos**.

---

## 1. Resumen: 35 personajes distintos

| Grupo | Personajes |
|---|---|
| Protagonista | Tú (el alumno o la alumna) |
| Mentores (6) | Cajal, Luria, Goldberg, Darwin, Wechsler, el Profe |
| Clase del prólogo (6) | Lucas, Carla, Dani, Irene, Sofía (dibuja cerebros), Lucía (escucha con los ojos cerrados) |
| Mundo 1 · Neuromitos (3) | Phineas Gage, Pablo, Iván |
| Mundo 2 · Neuronas (3) | Nerea, Teodoro, Marcos (mundo 2) |
| Mundo 3 · Percepción, praxias y lenguaje (3) | Tomás, Nico, Julián |
| Mundo 4 · Atención, memoria y FE (3) | Lola, H. M., Quique |
| Mundo 5 · Emoción y cognición social (7) | Álvaro, Marta, Raúl, Leo, Nora y las marionetas Sally y Anne (Phineas Gage reaparece aquí, ya contado en el mundo 1) |
| Mundo 6 · Evaluación (3) | Sara, Nacho, Álex |

(El Profe es el mentor del mundo 1 y también el profesor de la clase. Phineas Gage aparece en los mundos 1 y 5.)

---

## 2. Protagonista

### Tú (el alumno o la alumna)
- **Rol:** protagonista. Se duerme en clase y viaja por los seis mundos.
- **Personalidad:** sarcástico, escéptico, con humor seco. Comenta todo con ironía («mi vida social está en un punto muy bajo», «ojeras de nivel segundo parcial»).
- **Género:** **decidido: es un chico.** (El texto del juego sigue siendo neutro: «Tú».)
- **Visual:** estudiante universitario/a en 4º de Grado, ojeras, cara de «¿esto entra en el examen?». Sudadera/camiseta azul, pantalón oscuro.
- **Colores del prototipo:** camiseta `#3d6fb5`, pantalón `#2b2f4a`, pelo `#4a2c2a`.
- **Extras:** una versión «dormido» (cabeza apoyada sobre una sudadera verde) y una versión «sorprendido» al despertar.

---

## 3. Mentores (6)

### Santiago Ramón y Cajal · mentor del hub y del mundo 2
- **Rol:** anfitrión de la neurona gigante y guía del Bosque de las Neuronas.
- **Personalidad:** orgulloso, sarcástico con cariño; hace chistes sobre sus dibujos y sobre el temario.
- **Visual (caricatura):** hombre mayor con barba y bigote blancos, boina negra, abrigo oscuro, lápiz en la mano. Mirada penetrante.
- **Colores:** abrigo `#2a2733`, pelo `#d8d4cc`, barba `#ece7dc`, boina `#15131c`, piel `#e0b08c`.
- **Prop:** un lápiz y un microscopio.
- **Estado (17/11/2026):** hoja aprobada y sprites integrados (hub y mundo 2). Ver `arte/cajal/LEEME.md`. Pendiente: retratos de diálogo, microscopio y lápiz como objetos.

### Aleksandr Románovich Luria · mentor del mundo 3 (Galería de los Espejos)
- **Rol:** observa, pregunta y razona; aparece también dentro de un espejo de mano que da pistas.
- **Personalidad:** serio, exacto, irónico (con una media sonrisa apenas visible). Detesta que se etiquete antes de descartar.
- **Visual (CANON aprobado 17/11/2026, según la hoja `arte/fuente/luria_hoja_v1.webp`):** hombre de mediana edad con gafas, pelo rizado gris oscuro, chaqueta marrón, camisa blanca y corbata, pantalón gris; gesto sereno con media sonrisa irónica. (Sustituye a la descripción inicial: chaqueta de tweed y pelo oscuro peinado.)
- **Colores:** los de los sprites (`arte/luria/`): chaqueta marrón, pantalón gris, pelo gris oscuro, piel `#e5b995`.
- **Retrato extra:** busto pequeño dentro de un **espejo de mano** dorado.
- **Objetos de la hoja:** libros, cerebro, cubos de Kohs, portapapeles, matrioska (el espejo de mano dorado sigue pendiente).

### Elkhonon Goldberg · mentor del mundo 4 (Biblioteca sin Fin)
- **Rol:** director de orquesta (metáfora de las funciones ejecutivas); se presenta como alumno de Luria.
- **Personalidad:** elegante, solemne y un poco teatral; «el director no toca nada y sin él se nota».
- **Visual (caricatura):** frac negro, pelo gris, gafas, batuta blanca, gesto de dirigir. (Ver precauciones: persona real, posiblemente viva.)
- **Colores:** frac `#1c1c28`, pelo `#8a8a92`, piel `#e5b995`.
- **Prop:** batuta y un metrónomo con su cara.
- **Estado (17/11/2026):** hoja aprobada tácitamente y sprites integrados en la Biblioteca (ver `arte/goldberg/LEEME.md`). Diseño de la hoja: pelo gris ondulado, gafas, frac negro, chaleco crema, pajarita; metrónomo con un cerebro dibujado en vez de su cara. Pendiente: visto bueno de Goldberg.

### Charles Darwin · mentor del mundo 5 (Carnaval Límbico)
- **Rol:** observa y anota; ahora reconoce con humor que la universalidad de la expresión es discutida (Barrett).
- **Personalidad:** caballero victoriano, educado, curioso, ligeramente anticuado («no, no tengo móvil»).
- **Visual (caricatura):** barba larga y blanca, calva incipiente, levita oscura, lupa. Se mira en un espejo haciendo muecas.
- **Colores:** levita `#2a2a2a`, pantalón `#1c1c20`, pelo `#d8d4cc`, barba `#f0ece0`, piel `#e0b08c`.
- **Prop:** lupa gigante (la que da las pistas).
- **Estado (17/11/2026):** hoja aprobada y sprites integrados en el Carnaval (ver `arte/darwin/LEEME.md`). Diseño de la hoja: calvo con pelo blanco a los lados, barba larga, levita marrón oscuro con chaleco, lupa dorada, cuaderno y espejo de pie.

### David Wechsler · mentor del mundo 6 (Gabinete de Evaluación)
- **Rol:** calibra, mide y pide método. Las escalas llevan su apellido.
- **Personalidad:** sereno, meticuloso, sarcástico en voz baja («una puntuación sin contexto es ruido con decimales»).
- **Visual (caricatura):** bata blanca, gafas, pelo oscuro peinado, aspecto clínico; coloca pesas en una balanza.
- **Colores:** bata `#e8e8f0`, pantalón `#33384f`, pelo `#2a2a2a`, piel `#e0b08c`.
- **Prop:** balanza de latón.
- **Estado (17/11/2026):** hoja aprobada tácitamente y sprites integrados en el Gabinete (ver `arte/wechsler/LEEME.md`). Diseño de la hoja: traje gris-marrón con chaleco burdeos, calvo con entradas, bigote y gafas (sustituye a la bata blanca y al pelo oscuro peinado de la ficha inicial).

### El Profe · mentor del mundo 1 y profesor de la clase
- **Rol:** cierra el círculo: es el profesor de la clase del prólogo y guía el Pasillo de los Neuromitos.
- **Personalidad:** entusiasta, algo teatral, pone exámenes sorpresa «con mucha pedagogía». **Es una caricatura del propio docente:** valida con él cómo quiere verse.
- **Visual (CANON aprobado 17/11/2026):** calvo con entradas, barba corta marrón, gafas negras gruesas, americana marrón, camisa azul claro, pantalón azul oscuro, puntero.
- **Colores:** americana `#8b5634`, camisa `#a8c8ff`, pantalón `#33384f`, barba `#4a2c2a`. Sprites en `arte/profe/`.
- **Prop:** puntero y un mando de Kahoot gigante.

---

## 4. Clase del prólogo (6)

Aparecen sentados en los pupitres de la clase donde empieza el juego. Cada uno tiene una «manía» que lo define. Deben distinguirse a 32 px.

| Personaje | Manía / personalidad | Colores del prototipo |
|---|---|---|
| **Lucas** | Duerme con los ojos casi abiertos; dibuja gatos; «café y miedo» | camiseta `#c0852c`, pelo `#222` |
| **Carla** | Toma apuntes a toda velocidad, cuaderno con más colores que una paleta | camiseta `#4a8c8c`, pelo `#1a1a1a` |
| **Dani** | Levanta la mano cada tres minutos; pregunta «¿esto entra en el examen?» | camiseta `#9b59b6`, pelo `#7a3a2a` |
| **Irene** | Mira el móvil con cara de culpa elaborada | camiseta `#e67e22`, pelo `#5a3a22` |
| **Sofía (clase; antes «Marcos»)** | Dibuja cerebros con patillas en el margen | camiseta `#2e86c1`, pelo `#222` |
| **Lucía (clase; antes «Sofía»)** | Escucha con los ojos cerrados con mucha dignidad | camiseta `#c0392b`, pelo `#3a2418` |

---

## 5. Mundo 1 · Pasillo de los Neuromitos

### Phineas Gage (también en el mundo 5)
- **Rol:** persona real y caso histórico; aquí, símbolo del origen de la neuropsicología (relación cerebro–conducta). En el mundo 5 es el caso de lesión orbitofrontal.
- **Personalidad:** educado, algo impaciente y directo; pide que lo llamen Phineas.
- **Visual:** hombre del siglo XIX, sombrero, chaleco y camisa de época, aspecto amable y sereno. **Sin ninguna referencia a la lesión.** Tratarlo con respeto.
- **Colores:** camisa `#6a4a3a` (mundo 1) / `#7a4a2a` (mundo 5), pelo `#3a2a1a`/`#4a3a2a`, sombrero `#3a2a1a`.
- **Estado (17/11/2026):** sprites integrados (hoja del mundo 1; ver `arte/gage/LEEME.md`).

### Pablo (12 años, caso didáctico)
- **Rol:** alumno con dislexia diagnosticada tarde.
- **Personalidad:** abierto, algo desconcertado, aliviado al entender («no es que me haya vuelto disléxico»).
- **Visual:** chaval de 12 años con mochila, mirada despierta y un poco cansada.
- **Colores:** camiseta `#4a8c8c`, pelo `#2a1a10`.
- **Estado (17/11/2026):** sprites integrados (hoja del mundo 1; ver `arte/gage/LEEME.md`).

### Iván (10 años, caso didáctico ficticio)
- **Rol:** niño con perfil verbal fuerte y dificultades ejecutivas (caso del informe).
- **Personalidad:** muy hablador sobre sus videojuegos, sincero («me da una pereza enorme… pero vale»).
- **Visual:** niño de 10 años, camiseta de videojuego, piernas inquietas. **Sin estereotipos ni rasgos que ridiculicen.**
- **Colores:** camiseta `#c0852c`, pelo `#3a2418`.
- **Estado (17/11/2026):** sprites integrados (hoja del mundo 1; ver `arte/gage/LEEME.md`).

---

## 6. Mundo 2 · Bosque de las Neuronas

### Nerea (una neurona)
- **Rol:** caso didáctico de histología (conducción, mielina).
- **Personalidad:** enterada, simpática, con humor sobre «sus primas gliales».
- **Visual:** **neurona con cara**: soma redondo lila, núcleo oscuro, dendritas como cabello y un axón con vaina de mielina como cola. Dos ojos grandes y sonrisa pícara.
- **Colores:** soma `#d9a0ff`, núcleo `#a860d0`, dendritas `#c080e8`.
- **Estado (17/11/2026):** sprites integrados (hoja del mundo 2; ver `arte/nerea/LEEME.md`).

### Teodoro (cartógrafo del cerebro, caso didáctico)
- **Rol:** tiene un mapa con errores que hay que corregir.
- **Personalidad:** seguro de sí mismo, «yo no me he perdido, es el mapa».
- **Visual:** sombrero de explorador, gafas, chaleco, mapa enrollado bajo el brazo.
- **Colores:** camisa `#7a5a2a`, sombrero `#6a4a2a`, pelo `#3a2418`.
- **Estado (17/11/2026):** sprites integrados (hoja del mundo 2; ver `arte/nerea/LEEME.md`).

### Marcos (mundo 2, 9 años, zurdo)
- **Rol:** niño zurdo al que le han dicho que su lateralidad cruzada explica su dificultad lectora (mito).
- **Personalidad:** inquieto y curioso; se alivia al saber la verdad.
- **Visual:** niño de 9 años, escribe con la izquierda; lápiz en la mano izquierda.
- **Colores:** camiseta `#2e86c1`, pelo `#3a2418`.
- **Estado (17/11/2026):** sprites integrados (hoja del mundo 2; ver `arte/nerea/LEEME.md`).

---

## 7. Mundo 3 · Galería de los Espejos

### Tomás (caso didáctico, agnosia)
- **Rol:** copia perfectamente una llave pero no sabe nombrarla; la reconoce al tacto.
- **Personalidad:** cortés, despistado, agradecido («el mundo es un buen sitio si lo tocas»).
- **Visual:** hombre de mediana edad con gafas, chaqueta marrón, una llave dorada en la mano.
- **Colores:** camisa `#8a5a3a`, pelo `#555`.
- **Estado (17/11/2026):** sprites integrados (hoja del mundo 3; ver `arte/tomas/LEEME.md`).

### Nico (8 años, caso didáctico, trastorno del desarrollo de la coordinación)
- **Rol:** niño que construye un molino de bloques con una mano «con opiniones propias».
- **Personalidad:** alegre y con humor («di coordinación en construcción»).
- **Visual:** niño con camiseta roja, bloques de colores, expresión de concentración.
- **Colores:** camiseta `#d9553a`, pantalón `#2b3a5a`, pelo `#3a2418`.
- **Estado (17/11/2026):** sprites integrados (hoja del mundo 3; ver `arte/tomas/LEEME.md`).

### Julián (65 años, caso didáctico, afasia de Broca)
- **Rol:** hombre con afasia tras un ictus; juega al ajedrez y gana.
- **Personalidad:** tranquilo, atento, mirada de ajedrecista. **Es afasia, no torpeza: respetar su ritmo.**
- **Visual:** señor mayor, pelo gris, chaqueta de punto, tablero de ajedrez.
- **Colores:** chaqueta `#7a6a3a`, pelo `#cfcfcf`.
- **Estado (17/11/2026):** sprites integrados (hoja del mundo 3; ver `arte/tomas/LEEME.md`).

---

## 8. Mundo 4 · Biblioteca sin Fin

### Lola (9 años, caso didáctico, heminegligencia)
- **Rol:** niña con hemiplejia izquierda que ignora su lado izquierdo.
- **Personalidad:** concentrada, simpática, ordena fichas con orgullo.
- **Visual:** niña de 9 años con fichas de colores solo a su derecha; una mano apoyada en el regazo.
- **Colores:** camiseta `#c06aa8`, pelo `#4a2c2a`.
- **Estado (17/11/2026):** sprites integrados (hoja del mundo 4; ver `arte/lola/LEEME.md`).

### H. M. (caso histórico real)
- **Rol:** persona real con amnesia anterógrada; símbolo del «eterno presente» (sin hipocampo).
- **Personalidad:** amable, cortés, siempre «encantado de conocerte». **Tratarlo como una persona.**
- **Visual:** hombre de mediana edad, gafas, camisa de cuello, revista en las manos. Mirada dulce.
- **Colores:** camisa `#5a6a7a`, pelo `#2a2a30`.
- **Estado (17/11/2026):** sprites integrados (hoja del mundo 4; ver `arte/lola/LEEME.md`).

### Quique (10 años, caso didáctico, funciones ejecutivas)
- **Rol:** niño con un trabajo sobre el Antiguo Egipto y muchos papeles.
- **Personalidad:** buenas ideas, desorganizado, honesto («ya he empezado cuatro veces»).
- **Visual:** niño rubio rodeado de papeles, camiseta azul.
- **Colores:** camiseta `#3d8fd9`, pelo `#caa23a`.
- **Estado (17/11/2026):** sprites integrados (hoja del mundo 4; ver `arte/lola/LEEME.md`).

---

## 9. Mundo 5 · Carnaval Límbico

### Álvaro (caso didáctico, lesión de amígdala)
- **Rol:** hombre tranquilísimo ante cualquier amenaza.
- **Personalidad:** curioso, calmado («lo he apuntado en mi lista de cosas por probar»).
- **Visual:** hombre adulto con camisa verde y expresión serena en un túnel del miedo con luces rojas.
- **Colores:** camisa `#6a8a5a`, pelo `#222`.
- **Estado (17/11/2026):** sprites integrados (hojas del mundo 5; ver `arte/alvaro/LEEME.md`).

### Marta (caso didáctico, lesión frontomedial)
- **Rol:** persona con rostro inexpresivo (acinesia).
- **Personalidad:** feliz por dentro, cara de póker por fuera.
- **Visual:** mujer adulta con rostro muy neutro; **no confundir con Sara ni Lola** (ver notas de color).
- **Colores:** camiseta `#c06aa8`, pelo `#4a2c2a`.
- **Estado (17/11/2026):** sprites integrados (hojas del mundo 5; ver `arte/alvaro/LEEME.md`). Marta: camiseta turquesa `#2a9d8f` y moño bajo negro (cambio frente al rosa inicial, para no confundirla con Lola ni Sara).

### Raúl (caso didáctico, lesión dorsolateral)
- **Rol:** persona con apatía y pérdida de motivación.
- **Personalidad:** indiferente («da igual lo que decidáis»).
- **Visual:** hombre adulto encogido de hombros, camisa gris azulada.
- **Colores:** camisa `#7a7a8a`, pelo `#222`.
- **Estado (17/11/2026):** sprites integrados (hojas del mundo 5; ver `arte/alvaro/LEEME.md`).

### Leo (3 años) y Nora (5 años) (casos didácticos, teoría de la mente)
- **Rol:** los dos niños de la prueba de Sally y Anne. Leo señala la caja (realidad); Nora, la cesta.
- **Personalidad:** Leo, entusiasta; Nora, «lo sabía yo desde el principio».
- **Visual:** dos niños pequeños sentados en una alfombra, cada uno con su estilo.
- **Colores:** Leo camiseta `#e6c23a`, pelo `#3a2418`; Nora camiseta `#2ecc71`, pelo `#3a2418`.
- **Estado (17/11/2026):** sprites integrados (hojas del mundo 5; ver `arte/alvaro/LEEME.md`).

### Sally y Anne (marionetas)
- **Rol:** las marionetas del teatrillo de la falsa creencia.
- **Visual:** dos marionetas: Sally, vestido rojo, junto a una cesta; Anne, vestido azul, junto a una caja.

---

## 10. Mundo 6 · Gabinete de Evaluación

### Sara (9 años, caso didáctico)
- **Rol:** niña que rinde bien en pruebas cortas y se distrae en el aula.
- **Personalidad:** observadora, algo cansada de que no la entiendan.
- **Visual:** niña de 9 años, mirada pensativa, jersey rosa. Distinta de Lola y Marta.
- **Colores:** jersey `#c06aa8`, pelo `#4a2c2a`.
- **Estado (17/11/2026):** sprites integrados (hoja del mundo 6; ver `arte/sara/LEEME.md`). Sara: jersey de punto rosa de manga larga y dos trenzas cortas (para distinguirla de Lola y Marta).

### Nacho (8 años, caso didáctico)
- **Rol:** niño que pierde las instrucciones y se mueve mucho.
- **Personalidad:** inquieto, simpático, pregunta cada pocos segundos.
- **Visual:** niño de 8 años, camiseta azul, pelo castaño revuelto.
- **Colores:** camiseta `#5aa0d9`, pelo `#6a3a1a`.
- **Estado (17/11/2026):** sprites integrados (hoja del mundo 6; ver `arte/sara/LEEME.md`).

### Álex (10 años, caso didáctico, epilepsia facilitada por estrés y ruido)
- **Rol:** niño sensible al ruido y al estrés.
- **Personalidad:** bromista con recelo («¿esto es un laboratorio o una discoteca?»).
- **Visual:** niño de 10 años, camiseta verde, mirada atenta; mano cerca de la oreja.
- **Colores:** camiseta `#6aa86a`, pelo `#2a1a10`.
- **Estado (17/11/2026):** sprites integrados (hoja del mundo 6; ver `arte/sara/LEEME.md`).

---

## 11. Plan de trabajo en seis fases

(Acordado: mi propuesta inicial, con la modificación de ChatGPT de diseñar al profesor y el aula antes que los mentores.)

| Fase | Qué se hace | Resultado |
|---|---|---|
| 1 | (**hecha**, pendiente de retoques) Definir el **lenguaje gráfico definitivo** con el protagonista | Hoja de personaje, retrato y sprite del protagonista; paleta base y reglas de estilo |
| 2 | Diseñar **al Profe y el aula real** (en curso: ver `FASE2_PROFE_Y_AULA.md`) | Profe (sprite y retrato) y fondo de la clase del prólogo |
| 3 | Diseñar los **seis mentores** | Retratos con 4 expresiones y sprites |
| 4 | Diseñar los **alumnos del prólogo** (6) | Siluetas muy distintas, sentados y de pie |
| 5 | Diseñar los **personajes de los seis mundos** | Casos de cada mundo, con paleta por mundo |
| 6 | Crear **sprites, expresiones y recursos** listos para el juego | Hojas de sprites y retratos con los tamaños finales |

**Regla de oro:** no generar los 35 personajes de golpe. El protagonista es el patrón de referencia de todos los demás: hasta que su identidad visual sea excelente, no se avanza.

### Reglas de colaboración con otras IA
1. Las **descripciones, personalidades y colores** de este documento son la referencia. No se cambian por iniciativa de la IA.
2. Cualquier **propuesta de mejora** se anota **aparte**, en un bloque titulado «PROPUESTAS», sin modificar la ficha del personaje. Así no se alteran decisiones narrativas sin tu aprobación.
3. Antes de la Fase 5 hay que resolver: el nombre repetido de «Marcos», el visto bueno de Goldberg y las diferencias entre Lola, Marta y Sara.

---

## 12. Ficha técnica para el juego

Todo diseño debe pensarse con las dimensiones reales del juego.

| Elemento | Medida | Notas |
|---|---|---|
| Pantalla | **480 × 270** px | Se escala 2× o más; sin suavizado |
| Sprite en escena | **~40 × 44** px | Silueta y color dominante legibles a ese tamaño |
| Retrato de diálogo | **96 × 96** px (o 128 × 128) | 4 expresiones: neutra, divertida, escéptica, sorprendida |
| Sprite del protagonista | **40 × 44** px | Quieto, caminar (4 fotogramas, de frente y de lado), sentado, dormido, sorprendido |
| Contorno | 1 px oscuro | Color `#1a1423` en el prototipo |
| Fondo | Transparente | PNG sin suavizar |

**Nota técnica importante:** los generadores de imágenes (ChatGPT, Gemini) **no producen pixel-art real** a tamaños exactos: suelen dar imágenes grandes que *parecen* pixel-art. El flujo recomendado es: generar a tamaño grande → reducir al tamaño final con interpolación «vecino más cercano» → **retocar a mano** o con un limpiador de pixel-art → limitar la paleta. Para el sprite final conviene que lo repase un artista o una herramienta específica (Aseprite o similar).

### Nombres de archivo sugeridos
- `protagonista_sprite_idle.png`, `protagonista_walk_01..04.png`, `protagonista_retrato_neutra.png`, etc.
- `cajal_retrato_divertida.png`, `luria_sprite_idle.png`, etc.

---

## 13. Fase 1 · Paquete de prompts del protagonista

Pega estos prompts en ChatGPT o Gemini, **en este orden**, y no avances hasta quedar satisfecho.

### Paso 1 · Hoja de personaje (identidad)
```
Pixel art character design sheet for the protagonist of a humorous retro point-and-click adventure game (LucasArts / Return to Monkey Island feel).
A university student in their 4th year, gender-neutral, sarcastic and sleepy: dark circles under the eyes, a "will this be on the exam?" face.
Blue t-shirt (#3d6fb5), dark trousers (#2b2f4a), brown hair (#4a2c2a), clean 1px dark outline (#1a1423).
Show: front view, 3/4 view, side view, back view, on a flat transparent background. Limited palette, no text.
```

### Paso 2 · Retrato de diálogo con 4 expresiones
```
Same character as the reference image. Pixel art bust portrait, 96x96 style, 4 expressions in a row: neutral/sleepy, amused, skeptical (raised eyebrow), surprised.
Same palette and outline. Flat background, no text.
```

### Paso 3 · Poses especiales
```
Same character as the reference. Pixel art poses on a flat transparent background: 
(1) sitting at a school desk, head nodding, (2) asleep with the head on a folded green hoodie, (3) startled awake, (4) walking cycle of 4 frames, side view.
```

### Paso 4 · Prueba de tamaño
Reduce el sprite a **40 × 44** y míralo sobre un fondo oscuro a tamaño real. Si la silueta no se reconoce, se repite el paso 1 con más contraste (silueta más marcada, menos detalle).

### Criterios para dar por buena la Fase 1
- Se reconoce a 40 × 44 px en un fondo oscuro y en uno claro.
- Es reconocible por su silueta (sudadera azul + pelo castaño revuelto).
- Funciona en las cuatro vistas y en las cuatro expresiones.
- La paleta tiene **pocos colores** (máx. 16–24) y es fácil de extender a otros personajes.


---

## 14. Estado del protagonista (Fase 1)

**Decisiones tomadas:**
- Es **un chico** (aspecto de estudiante de 4º, pelo castaño revuelto, sudadera azul, mochila roja, zapatillas blancas con detalles rojos).
- El tamaño **canon** de todos los personajes pasa a ser **40 × 44 px**. El juego ya dibuja a todos los personajes provisionales con 44 px de alto.

**Ya integrado en el juego** (extraído de la hoja de sprites v2, ver `arte/protagonista/LEEME.md`):
- Idle (4 fotogramas), caminar (6), mirar (3), coger (3), usar (4), hablar (4).
- Dormido con la sudadera verde (4) y despertar (4; aún sin usar en escena).
- Las 5 vistas (frente, 3/4, perfil, 3/4 espalda y espalda), guardadas pero sin usar todavía.

**Aula v2:** el protagonista se espeja (mira a la izquierda/arriba) y se coloca en el centro delantero. Ver `FASE2_PROFE_Y_AULA.md`, sección 5.

**Pendiente de revisar con la IA:**
1. El **retrato de diálogo** con expresiones (no extraído aún).
2. El pelo cambió de `#4a2c2a` a `#7a4231`: aprobar o revertir.
3. «Usar» enseña un portátil: sustituir por un gesto neutro.
4. Las **ojeras** del retrato grande parecen un ojo morado: suavizar.
5. Las poses «dormir/despertar» incluyen un resto de la silla en el borde: limpiar.


## 15. Escala canon (17/11/2026)
Los sprites miden 40x44 px y se dibujan a **×1,5 (≈66 px)** en todo el juego (`SPR_SC` en `index.html`): protagonista, Profe y marcadores de posición (`person()`). Los sprites definitivos de mentores, alumnos y personajes de mundo deben generarse en el mismo canon 40x44 y se escalan igual.


## 16. Alumnado del aula, versión definitiva (17/11/2026)
Sprites sentados en `arte/alumnos/sentados/` (20 poses: 10 alumnos × 2), hoja fuente `arte/fuente/alumnado_sentados_v1.webp`. En el aula: Carla, Dani, Irene, Lucas, Sofía y Lucía. Se resuelve el nombre repetido «Marcos» (el de la clase pasa a ser Sofía). Sin usar aún: Marta, Álex, y dos alumnos sin nombre (chica con mechas rosas y chico rubio rizado con gafas). Ojo: Marta y Álvaro ya existen como casos de los mundos 4 y 5, así que no usarlos como alumnos.

**Escala de alumnos sentados (17/11/2026):** los alumnos sentados se dibujan a ×1 (≈45 px con su mesa), mientras protagonista, Profe y personajes de pie van a ×1,5. Los sprites sentados llevan ya zapatillas (se añadieron a los PNG de `arte/alumnos/sentados/`).
