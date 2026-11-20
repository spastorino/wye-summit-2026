# Iniciativa Rust — Slidev

```bash
npm install
npm run dev      # presentación en http://localhost:3030 (notas en /presenter)
npm run build    # versión estática en dist/
npm run export   # PDF (requiere: npm i -D playwright-chromium)
```

## Estructura

```
slides.md         contenido de las slides y notas del orador
style.css         colores, tipografías y estilos de todos los layouts y componentes
layouts/          contenido.vue, declaracion.vue
components/       Cards, Card, Compare, Side, CompareArrow, Stages, Stage,
                  Bento, Projects, Project
public/           rust-logo.svg
```

El lienzo es de 1920×1080 (`canvasWidth: 1920`), así que todas las medidas
de `style.css` están en px reales. Los colores están como variables `--ww-*`
al principio de `style.css`.

## Layouts

**`contenido`**: eyebrow + título (`# ...`) + cuerpo.

```yaml
layout: contenido
eyebrow: Qué pasó          # etiqueta chica arriba del título
tight: true                # menos espacio bajo el título
```

**`declaracion`**: fondo oscuro con una frase grande (portada y cierre).
`# ...` es la frase, un párrafo es el subtítulo y `## ...` va en color de acento.

```yaml
layout: declaracion
align: end                 # center (default) | end
size: lg                   # xl (default, 140px) | lg (96px)
logo: top                  # logo de Rust: top | bottom
bar: true                  # barrita de acento arriba
class: ww-big-h2           # `## ...` bien grande (cierre)
```

## Componentes

Dejá una línea en blanco después de abrir y antes de cerrar cada componente,
para que el markdown de adentro se procese.

```md
<Cards>
<Card icon="i-carbon-chat" eyebrow="Etapa 1" top>

### Título

Texto o lista.

</Card>
</Cards>
```

- `Card`: `icon` (cualquier ícono de Carbon: `i-carbon-<nombre>`, ver
  https://icones.js.org/collection/carbon), `eyebrow`, `number` (número grande
  de fondo) y `top` (borde de acento).
- `Compare` + `Side year="2025" headline="2 personas" [dark]` + `CompareArrow`:
  antes/después con viñetas (`- ...`).
- `Stages` + `Stage eyebrow="Etapa 1" title="..." status="completa|casi"`.
- `Bento`: grilla de tarjetas de 2 filas con textos más compactos: 3 arriba y
  3 abajo, o 3 arriba y 2 abajo (más anchas) si hay 5.
- `Projects` + `Project name="Dial9"`: grilla de proyectos de 4 por fila,
  todos con el mismo estilo. El contenido de cada
  `Project` es una descripción opcional.

## Notas del orador

El último comentario `<!-- ... -->` de cada slide.

## Créditos

`public/rust-logo.svg` es el logo oficial de Rust
(https://github.com/rust-lang/rust-artwork), distribuido bajo
CC-BY 4.0 (https://creativecommons.org/licenses/by/4.0/). En las slides se
muestra recoloreado en el color de acento del deck. Rust y su logo son marcas
registradas de la Rust Foundation; ver
https://rustfoundation.org/policy/rust-trademark-policy/.
