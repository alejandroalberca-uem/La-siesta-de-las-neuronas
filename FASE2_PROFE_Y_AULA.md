# Fase 2 · El Profe y el aula

Objetivo: tener el diseño definitivo del **Profe** (mentor del mundo 1 y profesor de la clase) y del **aula del prólogo**, usando al protagonista (Fase 1) como patrón de estilo y de escala.

## 0. Material de referencia (adjúntalo a ChatGPT/Gemini)

| Archivo | Para qué |
|---|---|
| `arte/protagonista/_hoja_de_contacto.png` | Estilo, escala (40 × 44 px) y paleta del protagonista. **Referencia de estilo obligatoria.** |
| `arte/referencia/aula_actual_480x270.png` | Aula actual a tamaño nativo (con el protagonista ya integrado). |
| `arte/referencia/aula_actual_plano_zonas.png` | La misma aula ×3 con las zonas rotuladas: dónde va cada cosa. |

> El aula actual es **provisional**. La composición (qué hay y dónde) es lo que queremos conservar; el dibujo, no.

---

## 1. El Profe

### Ficha (de la biblia, sin cambios)
- **Rol:** profesor de la clase del prólogo y mentor del Pasillo de los Neuromitos. Cierra el círculo del juego.
- **Personalidad:** entusiasta, algo teatral, pone «exámenes sorpresa con mucha pedagogía». Pasión sincera por enseñar.
- **Visual:** camisa granate, pantalón oscuro, gafas, barba corta oscura, puntero.
- **Colores del prototipo:** camisa `#8a3b3b`, pantalón `#33384f`, pelo y barba `#2b2b2b`.
- **Props:** puntero (en clase) y mando de Kahoot gigante (en el mundo 1).
- **Es una caricatura del propio docente.** Tú decides cómo quieres verte.

### Decisiones que necesito de ti (antes de generar)
1. **Pelo:** corto, rizado, entradas…
2. **Barba:** corta y cuidada (biblia) o más larga.
3. **Gafas:** redondas, rectangulares, montura fina o gruesa.
4. **Ropa:** ¿camisa granate (biblia) o con americana? La IA propuso americana marrón y barba larga en la vista general: **no está en la biblia**, es una propuesta.
5. **Edad aparente:** 35, 45, 55.
6. **Altura y complexión** respecto al protagonista (por escala, mide 44 px como todos, pero puede verse más ancho o más alto de espíritu).

### Sprites y retratos necesarios
| Recurso | Cantidad | Tamaño |
|---|---|---|
| Idle (respira, de pie) | 4 fotogramas | 40 × 44 |
| Señalar con el puntero (a la pizarra) | 4 | 40 × 44 (puede ser más ancho por el puntero) |
| Hablar (gesticula) | 4 | 40 × 44 |
| Escribir en la pizarra (de espaldas/lado) | 4 | 40 × 44 |
| Orgulloso / sorprendido | 2 | 40 × 44 |
| Vistas: frente, 3/4, perfil, espalda | 4 | 40 × 44 |
| Retrato de diálogo | 4 expresiones: neutra, entusiasta, escéptica, «examen sorpresa» | 96 × 96 |

### Prompts (en este orden)

**Paso 1 · Hoja de personaje**
```
Using the attached protagonist sheet as the STYLE, SCALE and PALETTE reference (same pixel art, same 1px dark outline #1a1423, same proportions, 44px tall),
design the university professor of a humorous retro point-and-click adventure game (LucasArts / Return to Monkey Island feel).
He is an enthusiastic, slightly theatrical teacher who gives "surprise exams with lots of pedagogy". Friendly caricature, respectful, NOT photorealistic.
Details: <PEGA AQUÍ TUS DECISIONES: pelo, barba, gafas, camisa granate #8a3b3b, pantalón #33384f, edad aparente>.
Prop: a pointer stick.
Show front, 3/4, side and back views on a flat transparent background, TRUE pixel art on a strict grid, max 20 colors, hard edges, no gradients, no anti-aliasing, no text.
```

**Paso 2 · Retrato con 4 expresiones**
```
Same character and style. Pixel art bust portrait, 96x96, 4 expressions in a row: neutral, enthusiastic (big smile), skeptical (raised eyebrow, looking over the glasses), "surprise exam" (mischievous grin).
Same palette and outline. Flat background.
```

**Paso 3 · Sprites de animación (40×44)**
```
Same character, true pixel art sprites of 40x44 px on a strict grid, transparent background, 1px outline #1a1423, max 20 colors:
idle (4 frames, subtle breathing), pointing at a board with the pointer (4 frames), talking with hand gestures (4 frames),
writing on a board seen from behind (4 frames), proud (2 frames), surprised (2 frames).
Show each animation in a labeled row, frames side by side. No gradients, no anti-aliasing.
```

### Criterios para darlo por bueno
- Se reconoce a 40 × 44 y se distingue del protagonista por silueta y color (camisa granate, barba, gafas).
- Comparte con el protagonista el **mismo estilo, grosor de contorno y paleta**.
- La barba y las gafas se leen como volumen limpio, no como ruido.
- Su cara en el retrato es amable y con humor, **sin parecido fotográfico**.

---

## 2. El aula del prólogo

### Qué hay y dónde (plano de la imagen `aula_actual_plano_zonas.png`)
Coordenadas en píxeles de la pantalla del juego (480 × 270). **Conviene respetar estas posiciones**: el juego tiene zonas de clic en ellas. Si el diseño las cambia, ajusto yo el código.

| Elemento | Posición (x, y, ancho, alto) | Notas |
|---|---|---|
| Ventana (puesta de sol) | 26, 30, 106 × 86 | Luz cálida y diagonal sobre el suelo |
| Pizarra | 170, 28, 162 × 78 | Debe poder tener texto: **pedirla en blanco** (el juego pone el texto) |
| Reloj | 372, 30, 40 × 40 | **Sin agujas** (el juego las anima) |
| Póster «SÉ UNA» (neurona) | 430, 40, 34 × 48 | Guiño al tema |
| Puerta | 0, 60, 18 × 90 | Salida; a la izquierda |
| El Profe (de pie) | cerca de (356, 160) | Junto a la pizarra, con el puntero |
| Mesa del protagonista (grande) | 296, 202, 122 × 30 | Con el termo (386, 190) y la mochila (398, 226) |
| Silla con sudadera verde | 212, 160, 48 × 48 | Elemento del puzle: la sudadera se coge |
| Mesa de Lucas (duerme) | 92, 188, 60 × 52 | A la izquierda, con «zZ» |
| Carla, Dani, Irene | fondo: (49, 176), (281, 180), (441, 180) | Mesas pequeñas de fondo |
| Marcos y Sofía | frente: (191, 240), (251, 246) | Mesas pequeñas más cercanas |
| Línea del suelo | y = 150 | Pared arriba, suelo abajo |

### Reglas de composición
- **Perspectiva suave de cuarto trasero** (como el aula actual): pared de fondo, suelo de madera en diagonal suave.
- **Los personajes miden 44 px**: las puertas y las mesas deben ser coherentes con esa escala.
- **El aula se entrega en capas** (ver abajo): fondo vacío + mobiliario como sprites aparte (para que los personajes puedan quedar delante y detrás de las mesas).
- **Luz:** hora dorada, haz de la ventana en diagonal, polvo en suspensión (el juego añade las partículas).
- **Paleta:** cálida y violeta oscura de pared, madera clara en el suelo; contraste suficiente para que los personajes de 44 px se lean.

### Entregables del aula
| Capa | Contenido |
|---|---|
| 1. Fondo vacío | Pared, ventana, pizarra en blanco, reloj sin agujas, póster, puerta, suelo |
| 2. Mesas de fondo | 3 mesas pequeñas (para Carla, Dani, Irene) |
| 3. Mesas del frente | 2 mesas pequeñas (para Marcos y Sofía) |
| 4. Mesa de Lucas | Mesa mediana |
| 5. Mesa del protagonista | Mesa grande, con hueco para el termo |
| 6. Silla | Silla con la sudadera verde |
| 7. Objetos | Termo rojo, mochila granate, cuaderno |

### Prompts del aula

**Paso 1 · Fondo vacío**
```
Using the attached image "aula_actual_480x270" as a COMPOSITION reference (keep the same layout: window with sunset on the left, blank whiteboard in the center, clock without hands on the right, poster on the far right, door on the far left, wooden floor starting at 55% of the height),
draw an EMPTY university classroom background for a retro point-and-click adventure game (LucasArts / Return to Monkey Island feel).
True pixel art, 480x270 native resolution (also provide a 3x upscale), hard edges, no gradients, no anti-aliasing, max 24 colors.
No characters, no desks, no chairs. Whiteboard completely blank. Clock with no hands. Warm golden-hour light from the window casting a diagonal beam on the floor.
Violet-tinted wall (#4b4570), wooden floor (#7b5443). No text.
```

**Paso 2 · Mobiliario como sprites**
```
Same style and palette. Separate pixel-art sprites on a transparent background: small school desk (46px wide), medium desk (60px wide), large teacher-style desk (122px wide), chair with a green hoodie hanging on it, red thermos, maroon backpack, open notebook.
Seen from the same camera angle as the classroom. Scale: a student character is 44px tall.
```

**Paso 3 · Prueba de composición**
Superponer el protagonista, el Profe y las mesas sobre el fondo, a tamaño real. Revisar que los personajes se leen, que la luz no se come los contornos y que la pizarra y el reloj siguen siendo editables.

### Criterios para darlo por bueno
- Se lee como **aula**, con calidez y humor, y es **bonita** (prioridad estética del proyecto).
- La composición coincide con el plano: nada importante se mueve de sitio sin avisar.
- Los personajes de 44 px se distinguen del fondo (contraste de silueta).
- Pizarra en blanco y reloj sin agujas, para poder animarlos.

---

## 3. Qué haré yo cuando me pases las imágenes
1. **Extraer** los sprites del Profe (mismo método que con el protagonista) y **recortar** las capas del aula.
2. **Integrarlos** en el juego a tamaño real y probar con el protagonista y los alumnos.
3. Ajustar las **zonas de clic** si cambia algo del plano.
4. Mostrarte capturas a tamaño real para decidir.

## 4. Decisiones pendientes (resumen)
- Rasgos del Profe (pelo, barba, gafas, ropa, edad aparente).
- ¿Hay un **aula real** de la que quieras sacar fotos como referencia (por ejemplo, la de la Universidad Europea)? Si es así, pásamelas para inspirar el aula sin copiarla.
- Si el aula debe ser **fiel** a una real o una versión onírica más libre.


---

## 5. Dirección elegida: «Aula v2» (actualización)

**Decisión:** la imagen `arte/referencia/aula_inspiracion_principal.webp` pasa a ser la **inspiración principal** del aula, con estos cambios acordados:

1. **El protagonista y su mesa se espejan**: ahora **mira hacia la izquierda y hacia arriba** (hacia la pantalla) y su mesa se **extiende hacia la izquierda**, ocupando el centro delantero del cuadro. Así está más en el centro y más cerca de la acción.
2. **Cámara elevada en 3/4**, como la imagen (alumnos de espaldas o de perfil mirando a la pantalla).
3. Se mantiene el **humor y el ambiente**: puesta de sol, persianas, plantas, el alumno que duerme, el cerebro en la pantalla, el póster de neuronas.

### Qué hay que cambiar respecto a la imagen
| De la imagen | En el aula v2 |
|---|---|
| Logo de Universidad Europea (pared, termo y portátil) | **Quitarlo** de momento. Si se quiere usar, hace falta el visto bueno de la universidad. Si no, un logo genérico inventado. |
| Logotipo de Apple en el portátil | **Quitarlo** (portátil genérico) |
| Bocadillo con texto | **Quitarlo**: los diálogos los pone el juego |
| Texto de la pantalla | **Pantalla en blanco** (el juego escribe el texto). Mantener el cerebro rosa como dibujo aparte, opcional |
| Agujas del reloj | **Reloj sin agujas** (el juego las anima) |
| Falta la silla con la sudadera verde | **Añadirla**: es el objeto del puzle de dormirse |
| Alumnos distintos a la biblia | Ajustarlos a la biblia (ver más abajo) |
| Protagonista a la derecha, mirando a la derecha | **Espejado**: centro-derecha, mirando a la izquierda/arriba; mesa a su izquierda |

### Plano de composición
Ver `arte/referencia/aula_v2_plano_composicion.png` (esquema ×3 sobre 480 × 270). Es solo una guía de **dónde va cada cosa**, no de estilo.

### Escala por planos (para mantener el canon sin perder profundidad)
El canon (**44 px** de alto de pie) vale para los personajes del plano medio. Con la cámara elevada, la perspectiva modifica el tamaño según la fila:
| Plano | Qué hay | Altura aproximada (sentado) |
|---|---|---|
| Fondo (fila trasera) | Carla, Lucas, Dani, Irene | ~30 px |
| Medio | Marcos, Sofía, **el Profe de pie (44 px)** | ~34 px sentado |
| Frente | **El protagonista** y su mesa | ~40 px sentado |

> **Aviso:** en la imagen de inspiración, el Profe mediría ~89 px a escala del juego (el doble del canon). Para respetar el canon, el aula hay que dibujarla **más alejada** (más aire alrededor de los personajes) o con personajes más pequeños, con las proporciones de la tabla.

### Alumnos (ajustar a la biblia)
Lucas (duerme, camiseta mostaza), Carla (jersey verde azulado, apuntes), Dani (morado, levanta la mano), Irene (naranja, móvil), Marcos (camiseta azul, dibuja un cerebro), Sofía (roja, ojos cerrados). La IA colocó a una chica de coleta morada y a un chico de naranja: hay que **revisar quién es quién** al crear la versión final.

### Profe (de la imagen, pendiente de tu confirmación)
Rizos castaños, barba, gafas, americana marrón, camisa azul, pantalón gris, puntero. **No coincide con la biblia (camisa granate).** Si te gusta así, lo adopto como canon y actualizo la ficha.

### Prompt del aula v2 (fondo vacío, con la composición nueva)
```
Use the attached image "aula_inspiracion_principal" as the MAIN INSPIRATION (art direction, warm lighting, charm, humor, color mood), and the attached "aula_v2_plano_composicion" as the COMPOSITION guide.
Draw an EMPTY university classroom background for a retro point-and-click adventure game, elevated 3/4 camera view (as in the inspiration), 480x270 native pixel grid (also provide a 3x upscale), TRUE pixel art, hard edges, no gradients, no anti-aliasing, max 24 colors.
Changes from the inspiration: NO characters, NO logos or brand names (no Apple, no university logo), NO speech bubble. Whiteboard/screen completely BLANK. Clock with NO hands. Keep: sunset window with blinds, door on the left, neuron poster, plant.
Leave clear floor space for desks in 3 rows. The front-center area must be free for the protagonist's long desk, extending to the left.
```

### Prompt de los sprites de mobiliario (con el protagonista espejado)
```
Same style and palette. Pixel-art sprites on a transparent background, same elevated 3/4 camera: small student desk (46px), medium desk (60px), the protagonist's long desk (130px, extending to the LEFT), chair with a GREEN hoodie hanging, red thermos, maroon backpack, generic laptop (no logo), open notebook.
Also add the protagonist sitting at the long desk, FACING LEFT and slightly up, resting his chin on his hand (same character as the reference sprite sheet).
```

### Qué haré yo con lo que me pases
- Recortar las capas y los sprites, integrarlos a escala real y ajustar las zonas de clic.
- Re-colocar al protagonista (espejado, centro-derecha) y la animación de dormirse.
- Probar la escala por planos antes de cerrar nada.

## 6. Estado: Profe integrado (17/11/2026)
Sprites del Profe extraídos a `arte/profe/` e integrados en `index.html` (aula y mentor de neuromitos). Ver `arte/profe/LEEME.md`. Pendiente: Aula v2 (fondo vacío generado por el usuario), retratos y aprobar el diseño como canon.

## 7. Aula v2 integrada (17/11/2026)
- Fondo vacío recibido (`arte/fuente/aula_vacia_v1.webp`) → `arte/aula/aula_vacia_480x270.png` (96 colores), embebido en `index.html` (`AULA_IMG`, `buildClass`).
- Pizarra digital, manecillas del reloj, alumnos, mesas, silla con sudadera, termo, mochila y apuntes se dibujan encima en código; hotspots recolocados.
- Protagonista espejado (mira a la izquierda), mesa que se extiende a su izquierda; Profe de pie a la derecha de la pizarra.
- Pendiente: sustituir los muebles dibujados en código por los sprites de mobiliario (3 mesas, silla+sudadera, termo, mochila, cuaderno). Nota: el termo lleva el logo «ue».

## 8. Mobiliario y escala (17/11/2026)
- Sprites de mobiliario (`arte/mobiliario/`): mesa pequeña, mediana y grande, silla con sudadera (y `silla_vacia`, derivada quitando la sudadera), termo, mochila y cuaderno; embebidos como `FURN` en `index.html`.
- **Escala:** en el aula, protagonista y Profe se dibujan a ×1,5 (`SPR_SC`, ≈66 px) porque a 44 px quedaban pequeños frente al aula. Decidir si el canon pasa a ×1,5 en todo el juego (mundos, mentores, resto de alumnos).
- Termo con logo «ue» (pendiente decidir si se mantiene).

## 9. Hub v2 (neurona gigante)
Fondo nuevo del hub con el axón como pasarela y seis puertas sobre las vainas de mielina. Ver `arte/hub/LEEME.md`. Cajal (sprites definitivos) se coloca junto al soma. Pendiente: neurona destino al final del axón; probar a mano los retornos desde cada mundo.
