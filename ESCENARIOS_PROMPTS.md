# Prompts de escenarios (para ChatGPT)
24 fondos: por cada mundo, 1 escena de entrada + 3 salas. Todos van en formato 16:9 y se reducen luego a 480×270 como el hub.
## Cómo usarlos
- Pega el bloque entero de cada escena en ChatGPT y adjunta como referencias el fondo del hub (`Juego/arte/hub/hub_neurona_480x270.png`) y el aula (`Juego/arte/aula/aula_vacia_480x270.png`).
- Guarda cada resultado como `Juego/arte/fuente/escena_<id>_v1.webp` (por ejemplo `escena_n1_v1.webp`), o pásamelo por el chat.
- Los textos, las puertas de salida, las mesas, los personajes y los objetos de pista los sigue dibujando el juego en código encima. Por eso hay zonas que deben quedar libres.
- Orden recomendado: mundo 1, 2, 3, 4, 5 y 6. Con las 4 escenas de un mundo ya las integro juntas.
- Si una imagen sale con texto, con personajes o con la mesa dibujada, pídele que la repita sin eso: es la única corrección que importa.

---
## Mundo 1 · El Pasillo de los Neuromitos
**Ambiente:** Dusky school corridor. Palette: dark violet walls, magenta/pink accents and baseboard line, grey-lilac tiles, cream details; a hint of mischief, like a dream of school.

### 1. `neu` · Pasillo (entrada del mundo 1)
```text
Pixel art game background, 16:9 (1920x1080 with chunky pixels, equivalent to a 480x270 pixel grid), retro point-and-click adventure style (LucasArts / Return to Monkey Island feel). Same visual identity as the reference images (the Neuron Hub background and the Classroom background): real low-resolution pixel art, hard pixel edges, limited palette (max 32 colors), no anti-aliasing, no smooth gradients, no soft glow blur. ABSOLUTELY NO text, letters, numbers, logos, signs with writing, UI, buttons or characters/people anywhere in the image. Straight-on side view of a room (flat 2D, no perspective tilt).

Scene: School corridor with rows of lockers (blue-grey) between the three doorways and warm lights on the ceiling. Here the three doorways are wooden classroom doors with a small window each (frame only, empty glass area dark). FAR-RIGHT FEATURE: a big empty chalkboard in a wooden frame at 85%-100% of the width, 17%-58% of the height (blank, dark green). Black-and-cream checkered floor.

World mood: Dusky school corridor. Palette: dark violet walls, magenta/pink accents and baseboard line, grey-lilac tiles, cream details; a hint of mischief, like a dream of school.

LAYOUT RULES (the game draws sprites and props on top, so obey them exactly):
- The wall meets the floor along a straight horizontal line at about 66% of the image height. Wall above, floor below.
- THREE identical EMPTY doorways/arches, centered at exactly 25%, 50% and 75% of the width, each about 11%-14% of the width wide, from about 22% to 66% of the height (their bottoms touch the wall base line). Dark empty interior, nothing inside, no signs above or below (the game draws the glowing interior and labels by code).
- Far-left strip (0%-10% of the width, 36%-75% of the height): plain wall, no important details (an exit door is drawn there by code).
- Walkable floor strip (76%-93% of the height): completely clear and continuous, no objects. A standing character is drawn at about 36% of the width, so keep the floor around it empty.
- The far-right feature goes where indicated below.
```

### 2. `n1` · Sala de las Definiciones
```text
Pixel art game background, 16:9 (1920x1080 with chunky pixels, equivalent to a 480x270 pixel grid), retro point-and-click adventure style (LucasArts / Return to Monkey Island feel). Same visual identity as the reference images (the Neuron Hub background and the Classroom background): real low-resolution pixel art, hard pixel edges, limited palette (max 32 colors), no anti-aliasing, no smooth gradients, no soft glow blur. ABSOLUTELY NO text, letters, numbers, logos, signs with writing, UI, buttons or characters/people anywhere in the image. Straight-on side view of a room (flat 2D, no perspective tilt).

Scene: Classroom-office, violet wall, pink baseboard. THEMATIC DECORATION: a very large EMPTY whiteboard at 11%-43% of the width and 11%-47% of the height (blank white surface, frame only), with three small EMPTY paper posters pinned in a row just below it at 11%-43% width, 48%-56% height. Dark purple floor tiles.

World mood: Dusky school corridor. Palette: dark violet walls, magenta/pink accents and baseboard line, grey-lilac tiles, cream details; a hint of mischief, like a dream of school.

LAYOUT RULES (the game draws sprites and props on top, so obey them exactly):
- The wall meets the floor along a straight horizontal line at about 66% of the image height. Wall above, floor below.
- Far-left strip (0%-10% of the width, 36%-75% of the height): plain wall, no important details (an exit door is drawn there by code).
- Center-right area (52%-83% of the width, 40%-80% of the height): NO furniture and no important objects, only plain wall and floor (a desk and a character are drawn there by code).
- Upper-right area (62%-76% of the width, 27%-52% of the height): keep calm and uncluttered (a hanging clue object is drawn there by code).
- Walkable floor strip (76%-93% of the height): completely clear, continuous, no objects, same floor pattern from left to right.
- The thematic decoration goes where indicated below.
```

### 3. `n2` · Sala del Desarrollo
```text
Pixel art game background, 16:9 (1920x1080 with chunky pixels, equivalent to a 480x270 pixel grid), retro point-and-click adventure style (LucasArts / Return to Monkey Island feel). Same visual identity as the reference images (the Neuron Hub background and the Classroom background): real low-resolution pixel art, hard pixel edges, limited palette (max 32 colors), no anti-aliasing, no smooth gradients, no soft glow blur. ABSOLUTELY NO text, letters, numbers, logos, signs with writing, UI, buttons or characters/people anywhere in the image. Straight-on side view of a room (flat 2D, no perspective tilt).

Scene: Children's classroom, teal-green wall, pale wood baseboard. THEMATIC DECORATION: a tall wall height-measuring chart (a vertical ruler strip with tick marks and no numbers) at 11%-17% of the width, 11%-60% of the height; a wide shelf with colorful toy blocks and a small EMPTY whiteboard at 22%-42% width, 25%-45% height. Dark teal floor.

World mood: Dusky school corridor. Palette: dark violet walls, magenta/pink accents and baseboard line, grey-lilac tiles, cream details; a hint of mischief, like a dream of school.

LAYOUT RULES (the game draws sprites and props on top, so obey them exactly):
- The wall meets the floor along a straight horizontal line at about 66% of the image height. Wall above, floor below.
- Far-left strip (0%-10% of the width, 36%-75% of the height): plain wall, no important details (an exit door is drawn there by code).
- Center-right area (52%-83% of the width, 40%-80% of the height): NO furniture and no important objects, only plain wall and floor (a desk and a character are drawn there by code).
- Upper-right area (62%-76% of the width, 27%-52% of the height): keep calm and uncluttered (a hanging clue object is drawn there by code).
- Walkable floor strip (76%-93% of the height): completely clear, continuous, no objects, same floor pattern from left to right.
- The thematic decoration goes where indicated below.
```

### 4. `n3` · Sala del Informe
```text
Pixel art game background, 16:9 (1920x1080 with chunky pixels, equivalent to a 480x270 pixel grid), retro point-and-click adventure style (LucasArts / Return to Monkey Island feel). Same visual identity as the reference images (the Neuron Hub background and the Classroom background): real low-resolution pixel art, hard pixel edges, limited palette (max 32 colors), no anti-aliasing, no smooth gradients, no soft glow blur. ABSOLUTELY NO text, letters, numbers, logos, signs with writing, UI, buttons or characters/people anywhere in the image. Straight-on side view of a room (flat 2D, no perspective tilt).

Scene: Psychologist's office, slate-blue wall, lilac baseboard. THEMATIC DECORATION: a tall bookshelf full of colorful binders and books at 11%-27% of the width, 11%-49% of the height; next to it a framed bar-chart poster (bars of different heights, no numbers or letters) at 29%-45% width, 20%-50% height, and a crooked diploma frame at 47%-52% width, 18%-26% height. Dark navy floor.

World mood: Dusky school corridor. Palette: dark violet walls, magenta/pink accents and baseboard line, grey-lilac tiles, cream details; a hint of mischief, like a dream of school.

LAYOUT RULES (the game draws sprites and props on top, so obey them exactly):
- The wall meets the floor along a straight horizontal line at about 66% of the image height. Wall above, floor below.
- Far-left strip (0%-10% of the width, 36%-75% of the height): plain wall, no important details (an exit door is drawn there by code).
- Center-right area (52%-83% of the width, 40%-80% of the height): NO furniture and no important objects, only plain wall and floor (a desk and a character are drawn there by code).
- Upper-right area (62%-76% of the width, 27%-52% of the height): keep calm and uncluttered (a hanging clue object is drawn there by code).
- Walkable floor strip (76%-93% of the height): completely clear, continuous, no objects, same floor pattern from left to right.
- The thematic decoration goes where indicated below.
```

---
## Mundo 2 · El Bosque de las Neuronas
**Ambiente:** Magical night forest that is secretly a neuron. Palette: deep green and teal, bioluminescent mint and warm gold glow, bark browns, tiny fireflies.

### 5. `bos` · Claro del bosque (entrada del mundo 2)
```text
Pixel art game background, 16:9 (1920x1080 with chunky pixels, equivalent to a 480x270 pixel grid), retro point-and-click adventure style (LucasArts / Return to Monkey Island feel). Same visual identity as the reference images (the Neuron Hub background and the Classroom background): real low-resolution pixel art, hard pixel edges, limited palette (max 32 colors), no anti-aliasing, no smooth gradients, no soft glow blur. ABSOLUTELY NO text, letters, numbers, logos, signs with writing, UI, buttons or characters/people anywhere in the image. Straight-on side view of a room (flat 2D, no perspective tilt).

Scene: Night forest. The three doorways are arched openings carved into the trunks of three giant glowing trees (frames only; interior dark). A dirt clearing in the center-left floor, mossy ground elsewhere. FAR-RIGHT FEATURE: a clear space at 85%-98% of the width, 52%-83% of the height (a microscope is drawn there by code). Wooden desk-sized flat clearing at 31%-42% width, 74%-82% height must stay empty.

World mood: Magical night forest that is secretly a neuron. Palette: deep green and teal, bioluminescent mint and warm gold glow, bark browns, tiny fireflies.

LAYOUT RULES (the game draws sprites and props on top, so obey them exactly):
- The wall meets the floor along a straight horizontal line at about 66% of the image height. Wall above, floor below.
- THREE identical EMPTY doorways/arches, centered at exactly 25%, 50% and 75% of the width, each about 11%-14% of the width wide, from about 22% to 66% of the height (their bottoms touch the wall base line). Dark empty interior, nothing inside, no signs above or below (the game draws the glowing interior and labels by code).
- Far-left strip (0%-10% of the width, 36%-75% of the height): plain wall, no important details (an exit door is drawn there by code).
- Walkable floor strip (76%-93% of the height): completely clear and continuous, no objects. A standing character is drawn at about 36% of the width, so keep the floor around it empty.
- The far-right feature goes where indicated below.
```

### 6. `m1` · Sala de la neurona
```text
Pixel art game background, 16:9 (1920x1080 with chunky pixels, equivalent to a 480x270 pixel grid), retro point-and-click adventure style (LucasArts / Return to Monkey Island feel). Same visual identity as the reference images (the Neuron Hub background and the Classroom background): real low-resolution pixel art, hard pixel edges, limited palette (max 32 colors), no anti-aliasing, no smooth gradients, no soft glow blur. ABSOLUTELY NO text, letters, numbers, logos, signs with writing, UI, buttons or characters/people anywhere in the image. Straight-on side view of a room (flat 2D, no perspective tilt).

Scene: Laboratory-classroom set inside the forest, dark green wall, mint baseboard. THEMATIC DECORATION: a huge dark wall screen (empty, dark green glass) at 11%-51% of the width, 11%-47% of the height, with a thin glowing mint frame; ferns and hanging vines at the far edges. Mossy dark floor.

World mood: Magical night forest that is secretly a neuron. Palette: deep green and teal, bioluminescent mint and warm gold glow, bark browns, tiny fireflies.

LAYOUT RULES (the game draws sprites and props on top, so obey them exactly):
- The wall meets the floor along a straight horizontal line at about 66% of the image height. Wall above, floor below.
- Far-left strip (0%-10% of the width, 36%-75% of the height): plain wall, no important details (an exit door is drawn there by code).
- Center-right area (52%-83% of the width, 40%-80% of the height): NO furniture and no important objects, only plain wall and floor (a desk and a character are drawn there by code).
- Upper-right area (62%-76% of the width, 27%-52% of the height): keep calm and uncluttered (a hanging clue object is drawn there by code).
- Walkable floor strip (76%-93% of the height): completely clear, continuous, no objects, same floor pattern from left to right.
- The thematic decoration goes where indicated below.
```

### 7. `m2` · Sala del cartógrafo
```text
Pixel art game background, 16:9 (1920x1080 with chunky pixels, equivalent to a 480x270 pixel grid), retro point-and-click adventure style (LucasArts / Return to Monkey Island feel). Same visual identity as the reference images (the Neuron Hub background and the Classroom background): real low-resolution pixel art, hard pixel edges, limited palette (max 32 colors), no anti-aliasing, no smooth gradients, no soft glow blur. ABSOLUTELY NO text, letters, numbers, logos, signs with writing, UI, buttons or characters/people anywhere in the image. Straight-on side view of a room (flat 2D, no perspective tilt).

Scene: Explorer's study, dark navy-blue wall, bright blue baseboard line. THEMATIC DECORATION: a very large old parchment map pinned to the wall at 11%-42% of the width, 11%-46% of the height (blank aged paper with only a faint round pink shape in the middle and thin grid lines, no letters), and a smaller scroll next to it at 44%-52% width, 18%-26% height. Dark blue floor.

World mood: Magical night forest that is secretly a neuron. Palette: deep green and teal, bioluminescent mint and warm gold glow, bark browns, tiny fireflies.

LAYOUT RULES (the game draws sprites and props on top, so obey them exactly):
- The wall meets the floor along a straight horizontal line at about 66% of the image height. Wall above, floor below.
- Far-left strip (0%-10% of the width, 36%-75% of the height): plain wall, no important details (an exit door is drawn there by code).
- Center-right area (52%-83% of the width, 40%-80% of the height): NO furniture and no important objects, only plain wall and floor (a desk and a character are drawn there by code).
- Upper-right area (62%-76% of the width, 27%-52% of the height): keep calm and uncluttered (a hanging clue object is drawn there by code).
- Walkable floor strip (76%-93% of the height): completely clear, continuous, no objects, same floor pattern from left to right.
- The thematic decoration goes where indicated below.
```

### 8. `m3` · Sala de los hemisferios
```text
Pixel art game background, 16:9 (1920x1080 with chunky pixels, equivalent to a 480x270 pixel grid), retro point-and-click adventure style (LucasArts / Return to Monkey Island feel). Same visual identity as the reference images (the Neuron Hub background and the Classroom background): real low-resolution pixel art, hard pixel edges, limited palette (max 32 colors), no anti-aliasing, no smooth gradients, no soft glow blur. ABSOLUTELY NO text, letters, numbers, logos, signs with writing, UI, buttons or characters/people anywhere in the image. Straight-on side view of a room (flat 2D, no perspective tilt).

Scene: Room split in two halves by color: the left half (0%-50% of the width) warm brown-terracotta, the right half cool blue. THEMATIC DECORATION: a long horizontal golden bridge/beam with small vertical posts hanging under it (like a corpus callosum) crossing the middle of the wall at 31%-69% of the width, 32%-45% of the height. Everything else plain. Dark floor, split in the same two colors.

World mood: Magical night forest that is secretly a neuron. Palette: deep green and teal, bioluminescent mint and warm gold glow, bark browns, tiny fireflies.

LAYOUT RULES (the game draws sprites and props on top, so obey them exactly):
- The wall meets the floor along a straight horizontal line at about 66% of the image height. Wall above, floor below.
- Far-left strip (0%-10% of the width, 36%-75% of the height): plain wall, no important details (an exit door is drawn there by code).
- Center-right area (52%-83% of the width, 40%-80% of the height): NO furniture and no important objects, only plain wall and floor (a desk and a character are drawn there by code).
- Upper-right area (62%-76% of the width, 27%-52% of the height): keep calm and uncluttered (a hanging clue object is drawn there by code).
- Walkable floor strip (76%-93% of the height): completely clear, continuous, no objects, same floor pattern from left to right.
- The thematic decoration goes where indicated below.
```

---
## Mundo 3 · La Galería de los Espejos
**Ambiente:** Elegant moonlit museum gallery of mirrors. Palette: teal and deep blue walls, gold columns and frames, black-and-cream checkerboard marble floor, pale cyan reflections.

### 9. `gal` · Galería (entrada del mundo 3)
```text
Pixel art game background, 16:9 (1920x1080 with chunky pixels, equivalent to a 480x270 pixel grid), retro point-and-click adventure style (LucasArts / Return to Monkey Island feel). Same visual identity as the reference images (the Neuron Hub background and the Classroom background): real low-resolution pixel art, hard pixel edges, limited palette (max 32 colors), no anti-aliasing, no smooth gradients, no soft glow blur. ABSOLUTELY NO text, letters, numbers, logos, signs with writing, UI, buttons or characters/people anywhere in the image. Straight-on side view of a room (flat 2D, no perspective tilt).

Scene: Grand gallery with golden columns between and beside the arches. The three doorways are tall arched windows/mirror frames (gold frames; the glass area is dark and empty). FAR-RIGHT FEATURE: a taller dark arched frame at 86%-100% of the width, 10%-69% of the height (the big cracked mirror, glass dark and empty, gold frame). Black-and-cream checkerboard marble floor.

World mood: Elegant moonlit museum gallery of mirrors. Palette: teal and deep blue walls, gold columns and frames, black-and-cream checkerboard marble floor, pale cyan reflections.

LAYOUT RULES (the game draws sprites and props on top, so obey them exactly):
- The wall meets the floor along a straight horizontal line at about 66% of the image height. Wall above, floor below.
- THREE identical EMPTY doorways/arches, centered at exactly 25%, 50% and 75% of the width, each about 11%-14% of the width wide, from about 22% to 66% of the height (their bottoms touch the wall base line). Dark empty interior, nothing inside, no signs above or below (the game draws the glowing interior and labels by code).
- Far-left strip (0%-10% of the width, 36%-75% of the height): plain wall, no important details (an exit door is drawn there by code).
- Walkable floor strip (76%-93% of the height): completely clear and continuous, no objects. A standing character is drawn at about 36% of the width, so keep the floor around it empty.
- The far-right feature goes where indicated below.
```

### 10. `w1` · Sala de las Llaves
```text
Pixel art game background, 16:9 (1920x1080 with chunky pixels, equivalent to a 480x270 pixel grid), retro point-and-click adventure style (LucasArts / Return to Monkey Island feel). Same visual identity as the reference images (the Neuron Hub background and the Classroom background): real low-resolution pixel art, hard pixel edges, limited palette (max 32 colors), no anti-aliasing, no smooth gradients, no soft glow blur. ABSOLUTELY NO text, letters, numbers, logos, signs with writing, UI, buttons or characters/people anywhere in the image. Straight-on side view of a room (flat 2D, no perspective tilt).

Scene: Night study, deep indigo-blue wall, violet baseboard. THEMATIC DECORATION: a large window with a crescent moon and stars at 32%-49% of the width, 14%-48% of the height; many small golden keys of different sizes hanging from the ceiling on thin threads across 50%-83% of the width, 0%-22% of the height; keep 21%-29% of the width, 29%-48% of the height empty for a hanging mirror drawn by code. Dark blue checkered floor.

World mood: Elegant moonlit museum gallery of mirrors. Palette: teal and deep blue walls, gold columns and frames, black-and-cream checkerboard marble floor, pale cyan reflections.

LAYOUT RULES (the game draws sprites and props on top, so obey them exactly):
- The wall meets the floor along a straight horizontal line at about 66% of the image height. Wall above, floor below.
- Far-left strip (0%-10% of the width, 36%-75% of the height): plain wall, no important details (an exit door is drawn there by code).
- Center-right area (52%-83% of the width, 40%-80% of the height): NO furniture and no important objects, only plain wall and floor (a desk and a character are drawn there by code).
- Upper-right area (62%-76% of the width, 27%-52% of the height): keep calm and uncluttered (a hanging clue object is drawn there by code).
- Walkable floor strip (76%-93% of the height): completely clear, continuous, no objects, same floor pattern from left to right.
- The thematic decoration goes where indicated below.
```

### 11. `w2` · Sala del Taller
```text
Pixel art game background, 16:9 (1920x1080 with chunky pixels, equivalent to a 480x270 pixel grid), retro point-and-click adventure style (LucasArts / Return to Monkey Island feel). Same visual identity as the reference images (the Neuron Hub background and the Classroom background): real low-resolution pixel art, hard pixel edges, limited palette (max 32 colors), no anti-aliasing, no smooth gradients, no soft glow blur. ABSOLUTELY NO text, letters, numbers, logos, signs with writing, UI, buttons or characters/people anywhere in the image. Straight-on side view of a room (flat 2D, no perspective tilt).

Scene: Wooden workshop, warm brown wall and floor. THEMATIC DECORATION: a big pegboard with hanging hand tools (hammer, saw, wrench, red-handled tool, no text) at 11%-43% of the width, 14%-42% of the height; below it a wide shelf with colorful wooden blocks (red, blue, yellow, green) at 11%-37% width, 43%-50% height.

World mood: Elegant moonlit museum gallery of mirrors. Palette: teal and deep blue walls, gold columns and frames, black-and-cream checkerboard marble floor, pale cyan reflections.

LAYOUT RULES (the game draws sprites and props on top, so obey them exactly):
- The wall meets the floor along a straight horizontal line at about 66% of the image height. Wall above, floor below.
- Far-left strip (0%-10% of the width, 36%-75% of the height): plain wall, no important details (an exit door is drawn there by code).
- Center-right area (52%-83% of the width, 40%-80% of the height): NO furniture and no important objects, only plain wall and floor (a desk and a character are drawn there by code).
- Upper-right area (62%-76% of the width, 27%-52% of the height): keep calm and uncluttered (a hanging clue object is drawn there by code).
- Walkable floor strip (76%-93% of the height): completely clear, continuous, no objects, same floor pattern from left to right.
- The thematic decoration goes where indicated below.
```

### 12. `w3` · Sala de las Palabras
```text
Pixel art game background, 16:9 (1920x1080 with chunky pixels, equivalent to a 480x270 pixel grid), retro point-and-click adventure style (LucasArts / Return to Monkey Island feel). Same visual identity as the reference images (the Neuron Hub background and the Classroom background): real low-resolution pixel art, hard pixel edges, limited palette (max 32 colors), no anti-aliasing, no smooth gradients, no soft glow blur. ABSOLUTELY NO text, letters, numbers, logos, signs with writing, UI, buttons or characters/people anywhere in the image. Straight-on side view of a room (flat 2D, no perspective tilt).

Scene: Calm library-study, teal-green wall, light teal baseboard line. THEMATIC DECORATION: a big bookshelf full of colorful books at 11%-43% of the width, 11%-47% of the height; scattered small abstract letter-like glyphs are NOT allowed (no letters), instead add a few floating pale-teal dots and tiny sparkles around the shelf.

World mood: Elegant moonlit museum gallery of mirrors. Palette: teal and deep blue walls, gold columns and frames, black-and-cream checkerboard marble floor, pale cyan reflections.

LAYOUT RULES (the game draws sprites and props on top, so obey them exactly):
- The wall meets the floor along a straight horizontal line at about 66% of the image height. Wall above, floor below.
- Far-left strip (0%-10% of the width, 36%-75% of the height): plain wall, no important details (an exit door is drawn there by code).
- Center-right area (52%-83% of the width, 40%-80% of the height): NO furniture and no important objects, only plain wall and floor (a desk and a character are drawn there by code).
- Upper-right area (62%-76% of the width, 27%-52% of the height): keep calm and uncluttered (a hanging clue object is drawn there by code).
- Walkable floor strip (76%-93% of the height): completely clear, continuous, no objects, same floor pattern from left to right.
- The thematic decoration goes where indicated below.
```

---
## Mundo 4 · La Biblioteca sin Fin
**Ambiente:** Infinite library with a touch of concert hall. Palette: warm mahogany and brown, deep red carpet, brass and gold, green reading lamps, dusty light.

### 13. `bib` · Biblioteca (entrada del mundo 4)
```text
Pixel art game background, 16:9 (1920x1080 with chunky pixels, equivalent to a 480x270 pixel grid), retro point-and-click adventure style (LucasArts / Return to Monkey Island feel). Same visual identity as the reference images (the Neuron Hub background and the Classroom background): real low-resolution pixel art, hard pixel edges, limited palette (max 32 colors), no anti-aliasing, no smooth gradients, no soft glow blur. ABSOLUTELY NO text, letters, numbers, logos, signs with writing, UI, buttons or characters/people anywhere in the image. Straight-on side view of a room (flat 2D, no perspective tilt).

Scene: Immense library, shelves full of books from floor to ceiling on the whole back wall, the three doorways are arched openings cut into the shelves (gold frame, dark empty interior). A deep red carpet runner with a gold border on the floor between 10% and 85% of the width, 59%-82% of the height. FAR-RIGHT FEATURE: a clear space at 85%-98% of the width, 52%-83% of the height (a music stand is drawn there by code).

World mood: Infinite library with a touch of concert hall. Palette: warm mahogany and brown, deep red carpet, brass and gold, green reading lamps, dusty light.

LAYOUT RULES (the game draws sprites and props on top, so obey them exactly):
- The wall meets the floor along a straight horizontal line at about 66% of the image height. Wall above, floor below.
- THREE identical EMPTY doorways/arches, centered at exactly 25%, 50% and 75% of the width, each about 11%-14% of the width wide, from about 22% to 66% of the height (their bottoms touch the wall base line). Dark empty interior, nothing inside, no signs above or below (the game draws the glowing interior and labels by code).
- Far-left strip (0%-10% of the width, 36%-75% of the height): plain wall, no important details (an exit door is drawn there by code).
- Walkable floor strip (76%-93% of the height): completely clear and continuous, no objects. A standing character is drawn at about 36% of the width, so keep the floor around it empty.
- The far-right feature goes where indicated below.
```

### 14. `b1` · Sala del Faro
```text
Pixel art game background, 16:9 (1920x1080 with chunky pixels, equivalent to a 480x270 pixel grid), retro point-and-click adventure style (LucasArts / Return to Monkey Island feel). Same visual identity as the reference images (the Neuron Hub background and the Classroom background): real low-resolution pixel art, hard pixel edges, limited palette (max 32 colors), no anti-aliasing, no smooth gradients, no soft glow blur. ABSOLUTELY NO text, letters, numbers, logos, signs with writing, UI, buttons or characters/people anywhere in the image. Straight-on side view of a room (flat 2D, no perspective tilt).

Scene: Dark blue night room, deep navy wall, bright blue baseboard line. THEMATIC DECORATION: a tall floor lamp with a big rectangular glowing panel at 11%-21% of the width, 11%-45% of the height, with a wide soft beam of pale light cast diagonally across the wall and floor toward the right (hard-edged pixel beam, no blur); a framed star-map picture at 26%-38% width, 18%-31% height. Dark blue checkered floor.

World mood: Infinite library with a touch of concert hall. Palette: warm mahogany and brown, deep red carpet, brass and gold, green reading lamps, dusty light.

LAYOUT RULES (the game draws sprites and props on top, so obey them exactly):
- The wall meets the floor along a straight horizontal line at about 66% of the image height. Wall above, floor below.
- Far-left strip (0%-10% of the width, 36%-75% of the height): plain wall, no important details (an exit door is drawn there by code).
- Center-right area (52%-83% of the width, 40%-80% of the height): NO furniture and no important objects, only plain wall and floor (a desk and a character are drawn there by code).
- Upper-right area (62%-76% of the width, 27%-52% of the height): keep calm and uncluttered (a hanging clue object is drawn there by code).
- Walkable floor strip (76%-93% of the height): completely clear, continuous, no objects, same floor pattern from left to right.
- The thematic decoration goes where indicated below.
```

### 15. `b2` · El Archivo
```text
Pixel art game background, 16:9 (1920x1080 with chunky pixels, equivalent to a 480x270 pixel grid), retro point-and-click adventure style (LucasArts / Return to Monkey Island feel). Same visual identity as the reference images (the Neuron Hub background and the Classroom background): real low-resolution pixel art, hard pixel edges, limited palette (max 32 colors), no anti-aliasing, no smooth gradients, no soft glow blur. ABSOLUTELY NO text, letters, numbers, logos, signs with writing, UI, buttons or characters/people anywhere in the image. Straight-on side view of a room (flat 2D, no perspective tilt).

Scene: Old archive, dark green wall, bright green baseboard. THEMATIC DECORATION: a grid of metal filing-cabinet drawers (5 columns x 3 rows, with small label holders left blank) at 11%-43% of the width, 14%-43% of the height; a large round wall clock with the hands stopped at 51%-59% of the width, 16%-31% of the height. Dark green checkered floor.

World mood: Infinite library with a touch of concert hall. Palette: warm mahogany and brown, deep red carpet, brass and gold, green reading lamps, dusty light.

LAYOUT RULES (the game draws sprites and props on top, so obey them exactly):
- The wall meets the floor along a straight horizontal line at about 66% of the image height. Wall above, floor below.
- Far-left strip (0%-10% of the width, 36%-75% of the height): plain wall, no important details (an exit door is drawn there by code).
- Center-right area (52%-83% of the width, 40%-80% of the height): NO furniture and no important objects, only plain wall and floor (a desk and a character are drawn there by code).
- Upper-right area (62%-76% of the width, 27%-52% of the height): keep calm and uncluttered (a hanging clue object is drawn there by code).
- Walkable floor strip (76%-93% of the height): completely clear, continuous, no objects, same floor pattern from left to right.
- The thematic decoration goes where indicated below.
```

### 16. `b3` · El Foso de la Orquesta
```text
Pixel art game background, 16:9 (1920x1080 with chunky pixels, equivalent to a 480x270 pixel grid), retro point-and-click adventure style (LucasArts / Return to Monkey Island feel). Same visual identity as the reference images (the Neuron Hub background and the Classroom background): real low-resolution pixel art, hard pixel edges, limited palette (max 32 colors), no anti-aliasing, no smooth gradients, no soft glow blur. ABSOLUTELY NO text, letters, numbers, logos, signs with writing, UI, buttons or characters/people anywhere in the image. Straight-on side view of a room (flat 2D, no perspective tilt).

Scene: Orchestra pit of a theater, burgundy wall, gold baseboard trim. THEMATIC DECORATION: a heavy dark-red velvet curtain with gold fringe at 11%-30% of the width, 10%-49% of the height; a tall vertical traffic light (red, amber, green lights off) at 35%-41% of the width, 13%-42% of the height; two empty music stands (thin gold stands) at 24%-31% width, 40%-55% height. Dark wood floor.

World mood: Infinite library with a touch of concert hall. Palette: warm mahogany and brown, deep red carpet, brass and gold, green reading lamps, dusty light.

LAYOUT RULES (the game draws sprites and props on top, so obey them exactly):
- The wall meets the floor along a straight horizontal line at about 66% of the image height. Wall above, floor below.
- Far-left strip (0%-10% of the width, 36%-75% of the height): plain wall, no important details (an exit door is drawn there by code).
- Center-right area (52%-83% of the width, 40%-80% of the height): NO furniture and no important objects, only plain wall and floor (a desk and a character are drawn there by code).
- Upper-right area (62%-76% of the width, 27%-52% of the height): keep calm and uncluttered (a hanging clue object is drawn there by code).
- Walkable floor strip (76%-93% of the height): completely clear, continuous, no objects, same floor pattern from left to right.
- The thematic decoration goes where indicated below.
```

---
## Mundo 5 · El Carnaval Límbico
**Ambiente:** Surreal night fairground of emotions. Palette: deep purple night sky, saturated magenta, teal and orange accents, candy stripes, string lights.

### 17. `car` · Feria (entrada del mundo 5)
```text
Pixel art game background, 16:9 (1920x1080 with chunky pixels, equivalent to a 480x270 pixel grid), retro point-and-click adventure style (LucasArts / Return to Monkey Island feel). Same visual identity as the reference images (the Neuron Hub background and the Classroom background): real low-resolution pixel art, hard pixel edges, limited palette (max 32 colors), no anti-aliasing, no smooth gradients, no soft glow blur. ABSOLUTELY NO text, letters, numbers, logos, signs with writing, UI, buttons or characters/people anywhere in the image. Straight-on side view of a room (flat 2D, no perspective tilt).

Scene: Fairground at night under a purple sky with a crescent moon and a string of small colored light bulbs across the top. The three doorways are the entrances of three striped carnival tents (red-white, purple-white, blue-white), arched opening with dark empty interior, no signs. Cobbled plaza floor. FAR-RIGHT FEATURE: a small carousel with horses at 85%-100% of the width, 35%-82% of the height.

World mood: Surreal night fairground of emotions. Palette: deep purple night sky, saturated magenta, teal and orange accents, candy stripes, string lights.

LAYOUT RULES (the game draws sprites and props on top, so obey them exactly):
- The wall meets the floor along a straight horizontal line at about 66% of the image height. Wall above, floor below.
- THREE identical EMPTY doorways/arches, centered at exactly 25%, 50% and 75% of the width, each about 11%-14% of the width wide, from about 22% to 66% of the height (their bottoms touch the wall base line). Dark empty interior, nothing inside, no signs above or below (the game draws the glowing interior and labels by code).
- Far-left strip (0%-10% of the width, 36%-75% of the height): plain wall, no important details (an exit door is drawn there by code).
- Walkable floor strip (76%-93% of the height): completely clear and continuous, no objects. A standing character is drawn at about 36% of the width, so keep the floor around it empty.
- The far-right feature goes where indicated below.
```

### 18. `k1` · El Túnel del Miedo
```text
Pixel art game background, 16:9 (1920x1080 with chunky pixels, equivalent to a 480x270 pixel grid), retro point-and-click adventure style (LucasArts / Return to Monkey Island feel). Same visual identity as the reference images (the Neuron Hub background and the Classroom background): real low-resolution pixel art, hard pixel edges, limited palette (max 32 colors), no anti-aliasing, no smooth gradients, no soft glow blur. ABSOLUTELY NO text, letters, numbers, logos, signs with writing, UI, buttons or characters/people anywhere in the image. Straight-on side view of a room (flat 2D, no perspective tilt).

Scene: Dark red haunted tunnel, almost black burgundy wall, crimson baseboard line. THEMATIC DECORATION: a big round red alarm light on the wall at 51%-62% of the width, 6%-24% of the height with a bold red glow made of flat pixel rings; a pair of tiny glowing eyes peeking from dark corners (two or three pairs) across the wall; keep 11%-23% width, 25%-48% height for a pink model drawn by code and 27%-51% width, 12%-23% height for a neon sign drawn by code. Dark checkered red-black floor.

World mood: Surreal night fairground of emotions. Palette: deep purple night sky, saturated magenta, teal and orange accents, candy stripes, string lights.

LAYOUT RULES (the game draws sprites and props on top, so obey them exactly):
- The wall meets the floor along a straight horizontal line at about 66% of the image height. Wall above, floor below.
- Far-left strip (0%-10% of the width, 36%-75% of the height): plain wall, no important details (an exit door is drawn there by code).
- Center-right area (52%-83% of the width, 40%-80% of the height): NO furniture and no important objects, only plain wall and floor (a desk and a character are drawn there by code).
- Upper-right area (62%-76% of the width, 27%-52% of the height): keep calm and uncluttered (a hanging clue object is drawn there by code).
- Walkable floor strip (76%-93% of the height): completely clear, continuous, no objects, same floor pattern from left to right.
- The thematic decoration goes where indicated below.
```

### 19. `k2` · El Teatro de las Máscaras
```text
Pixel art game background, 16:9 (1920x1080 with chunky pixels, equivalent to a 480x270 pixel grid), retro point-and-click adventure style (LucasArts / Return to Monkey Island feel). Same visual identity as the reference images (the Neuron Hub background and the Classroom background): real low-resolution pixel art, hard pixel edges, limited palette (max 32 colors), no anti-aliasing, no smooth gradients, no soft glow blur. ABSOLUTELY NO text, letters, numbers, logos, signs with writing, UI, buttons or characters/people anywhere in the image. Straight-on side view of a room (flat 2D, no perspective tilt).

Scene: Small theater, purple wall, magenta baseboard. THEMATIC DECORATION: a heavy dark-red curtain strip at the far left edge at 10%-13% of the width, 11%-52% of the height; a row of three round yellow face-masks (smiley, neutral, sad, no text) on the wall at 15%-39% width, 17%-34% height; a spotlight beam coming from the ceiling at 38%-57% of the width onto the floor (hard-edged pixel beam). Dark violet checkered floor.

World mood: Surreal night fairground of emotions. Palette: deep purple night sky, saturated magenta, teal and orange accents, candy stripes, string lights.

LAYOUT RULES (the game draws sprites and props on top, so obey them exactly):
- The wall meets the floor along a straight horizontal line at about 66% of the image height. Wall above, floor below.
- Far-left strip (0%-10% of the width, 36%-75% of the height): plain wall, no important details (an exit door is drawn there by code).
- Center-right area (52%-83% of the width, 40%-80% of the height): NO furniture and no important objects, only plain wall and floor (a desk and a character are drawn there by code).
- Upper-right area (62%-76% of the width, 27%-52% of the height): keep calm and uncluttered (a hanging clue object is drawn there by code).
- Walkable floor strip (76%-93% of the height): completely clear, continuous, no objects, same floor pattern from left to right.
- The thematic decoration goes where indicated below.
```

### 20. `k3` · La Carpa de las Mentes
```text
Pixel art game background, 16:9 (1920x1080 with chunky pixels, equivalent to a 480x270 pixel grid), retro point-and-click adventure style (LucasArts / Return to Monkey Island feel). Same visual identity as the reference images (the Neuron Hub background and the Classroom background): real low-resolution pixel art, hard pixel edges, limited palette (max 32 colors), no anti-aliasing, no smooth gradients, no soft glow blur. ABSOLUTELY NO text, letters, numbers, logos, signs with writing, UI, buttons or characters/people anywhere in the image. Straight-on side view of a room (flat 2D, no perspective tilt).

Scene: Inside a circus tent at night, very dark blue starry wall, bright blue baseboard line. THEMATIC DECORATION: a small wooden puppet theater (empty stage, red-brown frame, dark blue backdrop) at 11%-33% of the width, 16%-47% of the height; a few stars on the wall; a round red-and-gold rug on the floor at 11%-35% width, 80%-90% height. Dark blue floor.

World mood: Surreal night fairground of emotions. Palette: deep purple night sky, saturated magenta, teal and orange accents, candy stripes, string lights.

LAYOUT RULES (the game draws sprites and props on top, so obey them exactly):
- The wall meets the floor along a straight horizontal line at about 66% of the image height. Wall above, floor below.
- Far-left strip (0%-10% of the width, 36%-75% of the height): plain wall, no important details (an exit door is drawn there by code).
- Center-right area (52%-83% of the width, 40%-80% of the height): NO furniture and no important objects, only plain wall and floor (a desk and a character are drawn there by code).
- Upper-right area (62%-76% of the width, 27%-52% of the height): keep calm and uncluttered (a hanging clue object is drawn there by code).
- Walkable floor strip (76%-93% of the height): completely clear, continuous, no objects, same floor pattern from left to right.
- The thematic decoration goes where indicated below.
```

---
## Mundo 6 · El Gabinete de Evaluación
**Ambiente:** Clinical neuropsychology office, calm and precise. Palette: teal and grey-blue walls, frosted glass, brass accents, pale checkered tiles, soft cyan lights.

### 21. `gab` · Gabinete (entrada del mundo 6)
```text
Pixel art game background, 16:9 (1920x1080 with chunky pixels, equivalent to a 480x270 pixel grid), retro point-and-click adventure style (LucasArts / Return to Monkey Island feel). Same visual identity as the reference images (the Neuron Hub background and the Classroom background): real low-resolution pixel art, hard pixel edges, limited palette (max 32 colors), no anti-aliasing, no smooth gradients, no soft glow blur. ABSOLUTELY NO text, letters, numbers, logos, signs with writing, UI, buttons or characters/people anywhere in the image. Straight-on side view of a room (flat 2D, no perspective tilt).

Scene: Reception hall of a clinic, teal wall, frosted-glass doors. The three doorways are glass doors with metal frames (frosted pale-cyan glass, no writing, nothing visible inside). Pale blue-grey checkered tile floor. Do NOT draw a balance scale (it is drawn by code); keep the wall between the 2nd and 3rd doorways (about 55%-70% of the width) plain. FAR-RIGHT FEATURE: a clear space at 86%-100% of the width, 44%-76% of the height (a reception desk is drawn there by code).

World mood: Clinical neuropsychology office, calm and precise. Palette: teal and grey-blue walls, frosted glass, brass accents, pale checkered tiles, soft cyan lights.

LAYOUT RULES (the game draws sprites and props on top, so obey them exactly):
- The wall meets the floor along a straight horizontal line at about 66% of the image height. Wall above, floor below.
- THREE identical EMPTY doorways/arches, centered at exactly 25%, 50% and 75% of the width, each about 11%-14% of the width wide, from about 22% to 66% of the height (their bottoms touch the wall base line). Dark empty interior, nothing inside, no signs above or below (the game draws the glowing interior and labels by code).
- Far-left strip (0%-10% of the width, 36%-75% of the height): plain wall, no important details (an exit door is drawn there by code).
- Walkable floor strip (76%-93% of the height): completely clear and continuous, no objects. A standing character is drawn at about 36% of the width, so keep the floor around it empty.
- The far-right feature goes where indicated below.
```

### 22. `v1` · Sala de Principios
```text
Pixel art game background, 16:9 (1920x1080 with chunky pixels, equivalent to a 480x270 pixel grid), retro point-and-click adventure style (LucasArts / Return to Monkey Island feel). Same visual identity as the reference images (the Neuron Hub background and the Classroom background): real low-resolution pixel art, hard pixel edges, limited palette (max 32 colors), no anti-aliasing, no smooth gradients, no soft glow blur. ABSOLUTELY NO text, letters, numbers, logos, signs with writing, UI, buttons or characters/people anywhere in the image. Straight-on side view of a room (flat 2D, no perspective tilt).

Scene: Office, dark teal wall, bright cyan baseboard. THEMATIC DECORATION: a tall bookshelf with colored binders and books at 11%-27% of the width, 11%-49% of the height; two framed certificates (blank, no text) at 31%-38% and 40%-47% of the width, 14%-23% of the height. Dark teal checkered floor.

World mood: Clinical neuropsychology office, calm and precise. Palette: teal and grey-blue walls, frosted glass, brass accents, pale checkered tiles, soft cyan lights.

LAYOUT RULES (the game draws sprites and props on top, so obey them exactly):
- The wall meets the floor along a straight horizontal line at about 66% of the image height. Wall above, floor below.
- Far-left strip (0%-10% of the width, 36%-75% of the height): plain wall, no important details (an exit door is drawn there by code).
- Center-right area (52%-83% of the width, 40%-80% of the height): NO furniture and no important objects, only plain wall and floor (a desk and a character are drawn there by code).
- Upper-right area (62%-76% of the width, 27%-52% of the height): keep calm and uncluttered (a hanging clue object is drawn there by code).
- Walkable floor strip (76%-93% of the height): completely clear, continuous, no objects, same floor pattern from left to right.
- The thematic decoration goes where indicated below.
```

### 23. `v2` · Sala de Pruebas
```text
Pixel art game background, 16:9 (1920x1080 with chunky pixels, equivalent to a 480x270 pixel grid), retro point-and-click adventure style (LucasArts / Return to Monkey Island feel). Same visual identity as the reference images (the Neuron Hub background and the Classroom background): real low-resolution pixel art, hard pixel edges, limited palette (max 32 colors), no anti-aliasing, no smooth gradients, no soft glow blur. ABSOLUTELY NO text, letters, numbers, logos, signs with writing, UI, buttons or characters/people anywhere in the image. Straight-on side view of a room (flat 2D, no perspective tilt).

Scene: Test room, dark blue-grey wall, light-blue baseboard. THEMATIC DECORATION: a big pegboard wall with a 3x3 grid of small pastel boxes (mint, cream, light blue, blank, no text), hanging from small hooks, at 11%-52% of the width, 6%-45% of the height. Dark navy checkered floor.

World mood: Clinical neuropsychology office, calm and precise. Palette: teal and grey-blue walls, frosted glass, brass accents, pale checkered tiles, soft cyan lights.

LAYOUT RULES (the game draws sprites and props on top, so obey them exactly):
- The wall meets the floor along a straight horizontal line at about 66% of the image height. Wall above, floor below.
- Far-left strip (0%-10% of the width, 36%-75% of the height): plain wall, no important details (an exit door is drawn there by code).
- Center-right area (52%-83% of the width, 40%-80% of the height): NO furniture and no important objects, only plain wall and floor (a desk and a character are drawn there by code).
- Upper-right area (62%-76% of the width, 27%-52% of the height): keep calm and uncluttered (a hanging clue object is drawn there by code).
- Walkable floor strip (76%-93% of the height): completely clear, continuous, no objects, same floor pattern from left to right.
- The thematic decoration goes where indicated below.
```

### 24. `v3` · Sala de Neuroimagen
```text
Pixel art game background, 16:9 (1920x1080 with chunky pixels, equivalent to a 480x270 pixel grid), retro point-and-click adventure style (LucasArts / Return to Monkey Island feel). Same visual identity as the reference images (the Neuron Hub background and the Classroom background): real low-resolution pixel art, hard pixel edges, limited palette (max 32 colors), no anti-aliasing, no smooth gradients, no soft glow blur. ABSOLUTELY NO text, letters, numbers, logos, signs with writing, UI, buttons or characters/people anywhere in the image. Straight-on side view of a room (flat 2D, no perspective tilt).

Scene: Imaging suite, dark slate wall, green-cyan baseboard line. THEMATIC DECORATION: a white MRI scanner (big round tunnel in a white housing, dark opening, a short sliding bed, no text) at 11%-26% of the width, 35%-52% of the height base; a dark monitor with a green wave line (EEG-like waveform) on the wall at 26%-48% of the width, 15%-30% of the height. Dim blue lighting. Dark navy floor.

World mood: Clinical neuropsychology office, calm and precise. Palette: teal and grey-blue walls, frosted glass, brass accents, pale checkered tiles, soft cyan lights.

LAYOUT RULES (the game draws sprites and props on top, so obey them exactly):
- The wall meets the floor along a straight horizontal line at about 66% of the image height. Wall above, floor below.
- Far-left strip (0%-10% of the width, 36%-75% of the height): plain wall, no important details (an exit door is drawn there by code).
- Center-right area (52%-83% of the width, 40%-80% of the height): NO furniture and no important objects, only plain wall and floor (a desk and a character are drawn there by code).
- Upper-right area (62%-76% of the width, 27%-52% of the height): keep calm and uncluttered (a hanging clue object is drawn there by code).
- Walkable floor strip (76%-93% of the height): completely clear, continuous, no objects, same floor pattern from left to right.
- The thematic decoration goes where indicated below.
```
