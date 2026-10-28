---
name: Casa de la Ribera II
description: Ficha de propiedad leída como tabla de mareas impresa, en dos tintas de marca sobre papel blanco azulado.
colors:
  azul: "#2e3092"
  azul-hondo: "#1d1f66"
  celeste: "#27aae1"
  papel: "#f6f8fd"
  tinta: "#23255f"
  tinta-suave: "#4a4d8a"
  regla: "rgba(46,48,146,.22)"
  papel-foto: "#dfe5f4"
  azul-claro-texto: "#dfe5f7"
  blanco: "#ffffff"
typography:
  display:
    fontFamily: "Montserrat, system-ui, sans-serif"
    fontSize: "clamp(2.1rem, 8.2vw, 3.6rem)"
    fontWeight: 900
    lineHeight: 1.04
    letterSpacing: "-0.025em"
  headline:
    fontFamily: "Montserrat, system-ui, sans-serif"
    fontSize: "clamp(1.6rem, 5vw, 2.4rem)"
    fontWeight: 900
    lineHeight: 1.6
    letterSpacing: "-0.02em"
  figure:
    fontFamily: "Montserrat, system-ui, sans-serif"
    fontSize: "1.25rem"
    fontWeight: 800
    lineHeight: 1.6
  body:
    fontFamily: "Montserrat, system-ui, sans-serif"
    fontSize: "clamp(16px, 1.05vw + 12px, 18px)"
    fontWeight: 300
    lineHeight: 1.6
  label:
    fontFamily: "Montserrat, system-ui, sans-serif"
    fontSize: "0.9rem"
    fontWeight: 500
    lineHeight: 1.6
    letterSpacing: "0.02em"
rounded:
  hairline: "2px"
spacing:
  gutter: "clamp(16px, 5vw, 56px)"
  row: "13px"
  section: "clamp(48px, 9vw, 96px)"
  max: "1180px"
components:
  button-primary:
    backgroundColor: "{colors.azul}"
    textColor: "{colors.blanco}"
    rounded: "{rounded.hairline}"
    padding: "0 28px"
    height: "52px"
    typography: "{typography.figure}"
  button-primary-hover:
    backgroundColor: "{colors.azul-hondo}"
  button-inverse:
    backgroundColor: "{colors.blanco}"
    textColor: "{colors.azul}"
    rounded: "{rounded.hairline}"
    padding: "0 28px"
    height: "52px"
  placeholder-ghost:
    textColor: "{colors.tinta-suave}"
    rounded: "{rounded.hairline}"
    padding: "2px 10px"
    typography: "{typography.label}"
---

# Design System: Casa de la Ribera II

## Overview

**Creative North Star: "La Tabla de Mareas"**

La ficha de la casa se lee como una tabla de mareas impresa: filas finas de datos, cifras tabulares, una regla gruesa arriba y reglas de 1px entre filas. La casa es "la hora" que importa. Solo se toma la gramática de la tabla; no hay datos de mareas ni metáforas náuticas ilustradas.

El sistema es de dos tintas sobre papel: azul Propietas para cifras, títulos, reglas y botones; celeste solo como segunda tinta en guías, contornos y marcas. Sin degradés, sin sombras, sin cards con íconos. Lo que falta se dibuja como casillero fantasma punteado, nunca como dato inventado. Hereda la paleta y la tipografía de la firma; el desarrollo no tiene marca propia.

**Key Characteristics:**
- Dos tintas de marca sobre papel blanco azulado, tintado hacia el azul.
- Cifras tabulares, alineadas a la derecha, con guía punteada celeste desde la etiqueta.
- Reglas finas como única estructura; esquinas casi rectas (2px).
- Fotos grandes a sangre dentro de la rejilla, cada una bajo una regla azul de 2px.
- Un solo gesto de movimiento: las reglas se trazan al entrar en pantalla.

## Colors

Azul de marca y celeste como únicas tintas, sobre un papel frío; los neutros son azules oscuros, nunca grises puros.

### Primary
- **Azul Propietas** (#2e3092): títulos, cifras, regla gruesa de tabla, botón primario, fondo del cierre, enlace "Escribinos".

### Secondary
- **Celeste Marea** (#27aae1): segunda tinta. Guía punteada de las filas, contorno del casillero fantasma, anillo de foco, hover del enlace del header. Nunca texto chico sobre blanco.

### Neutral
- **Papel Azulado** (#f6f8fd): fondo de página.
- **Azul Hondo** (#1d1f66): hover del botón y fondo del pie legal.
- **Tinta** (#23255f): texto de cuerpo.
- **Tinta Suave** (#4a4d8a): subtítulos, unidades, notas, leyendas secundarias.
- **Regla** (rgba(46,48,146,.22)): reglas de 1px entre filas.
- **Papel de Foto** (#dfe5f4): fondo mientras carga la imagen.
- **Azul Claro de Texto** (#dfe5f7): texto secundario sobre azul y azul hondo, y hover del botón inverso.

### Named Rules
**The Two Inks Rule.** Solo existen azul y celeste como colores de color. Todo lo demás es azul oscuro tintado o blanco.

**The Celeste Is Not Text Rule.** El celeste vive en reglas, contornos, guías y foco; en texto solo si es grande o sobre azul oscuro.

## Typography

**Display / Body Font:** Montserrat (system-ui, sans-serif), pesos 300, 500, 800, 900. Sustituto web de Gotham según el manual de marca.

**Character:** Black para títulos y Light para cuerpo; el contraste de peso hace la jerarquía sin cambiar de familia. Cifras tabulares en todo el documento (`font-variant-numeric: tabular-nums`).

### Hierarchy
- **Display** (900, clamp(2.1rem, 8.2vw, 3.6rem), 1.04, -0.025em): solo el h1 del nombre de la casa.
- **Headline** (900, clamp(1.6rem, 5vw, 2.4rem), -0.02em): títulos de sección, azul (blanco sobre el cierre).
- **Figure** (800, 1.25rem; 1rem en la tabla de condiciones): valores de la tabla y texto del botón.
- **Body** (300, clamp(16px, 1.05vw + 12px, 18px), 1.6): párrafos; bajada limitada a 62ch.
- **Label** (500, 0.9rem, 0.02em): etiquetas de fila, leyendas de foto, subtítulo, enlace del header.

### Named Rules
**The Weight Is The Hierarchy Rule.** Una sola familia; la jerarquía sale de 900/800/500/300 y del tamaño, no de otras fuentes.

## Layout

Columna de hasta 1180px con gutter fluido (clamp(16px, 5vw, 56px)). En celular: logo, foto a sangre en 4:3, título y tabla, botón de ancho completo. Desde 860px el hero pasa a dos columnas (1.25fr / 1fr) con la foto a sangre a la izquierda y la tabla centrada verticalmente a la derecha; la galería es de tres columnas con la primera foto ocupando dos y la segunda estirada; Condiciones se parte en dos columnas con 56px de aire. Ritmo vertical de sección fluido (48 a 96px); filas de tabla con 13px de padding vertical.

## Elevation & Depth

Plano. Sin sombras en ningún estado. La profundidad es tonal y lineal: papel claro, bloques de azul pleno (cierre) y azul hondo (pie), y reglas de 2px que abren cada tabla y cada foto. El único cambio de estado de superficie es el oscurecimiento del botón en hover y un leve hundimiento en `:active` (translateY 1px, scale .99).

### Named Rules
**The Rule, Not The Shadow Rule.** La separación se hace con una regla de 1 o 2px, nunca con sombra ni con card.

## Shapes

Casi rectangular: radio de 2px en botón, casillero fantasma y foco. Las fotos son rectángulos sin radio (4:3, 16:10 en la destacada). El contorno punteado de 1px celeste es la forma de "pendiente". Las reglas gruesas (2px azul) abren; las finas (1px regla) separan.

## Components

### Buttons
- **Shape:** esquinas de 2px, altura mínima 52px, padding 0 28px; ancho completo bajo 520px.
- **Primary:** azul Propietas con texto blanco en Montserrat 800 e ícono SVG de WhatsApp inline a la izquierda.
- **Hover / Focus:** hover a azul hondo en .25s con ease expo-out (cubic-bezier(.16,1,.3,1)); foco con anillo celeste de 3px y 3px de offset.
- **Inverse:** sobre el cierre azul, fondo blanco y texto azul; hover a #dfe7f7.
- **Text link:** "Escribinos" en peso 500 con subrayado de 1px azul que pasa a celeste en hover.

### Tabla de datos (firma)
Lista con regla superior azul de 2px; cada fila alinea al baseline una etiqueta (500), una guía punteada celeste flexible y el valor en 800 azul alineado a la derecha, con la unidad en `small` 500 tinta suave. Filas separadas por 1px de regla. Se usa para los datos de la casa y para las condiciones.

### Casillero fantasma
Marca de lo pendiente: contorno punteado celeste de 1px, 2px de radio, texto 500 tinta suave centrado (ej. "Consultar"). Sustituye a cualquier dato no confirmado.

### Figura de galería
Foto 4:3 bajo regla azul de 2px, con leyenda en una línea (nombre del ambiente a la izquierda, dato secundario a la derecha en tinta suave).

### Cierre y pie
Cierre en azul pleno con título blanco, botón inverso con el teléfono y correo en blanco. Pie en azul hondo con logo blanco, matrícula, aviso legal y enlaces de la firma.

### Movimiento
Un solo gesto: tablas y figuras se "trazan" con clip-path al entrar en pantalla (animation-timeline: view(), solo con soporte y sin reduced-motion). Transiciones desactivadas con reduced-motion.

## Do's and Don'ts

### Do:
- **Do** dar cada dato como fila de tabla: etiqueta, guía punteada celeste, valor azul 800 a la derecha.
- **Do** marcar lo no confirmado con el casillero fantasma en lugar de inventarlo.
- **Do** abrir cada bloque de datos o foto con una regla azul de 2px.
- **Do** usar el logo de color sobre papel y el blanco sobre azul hondo, sin alterarlos.
- **Do** mantener el botón de WhatsApp azul visible en el primer viewport móvil.

### Don't:
- **Don't** usar celeste para texto chico sobre blanco.
- **Don't** agregar sombras, degradés ni cards con íconos.
- **Don't** introducir una tercera tinta ni grises puros.
- **Don't** usar badges ni un hero partido con chips sobre la foto.
- **Don't** afirmar cercanía al mar ni mostrar datos no confirmados.
