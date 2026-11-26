---
theme: default
title: Iniciativa Rust
colorSchema: light
canvasWidth: 1920
aspectRatio: 16/9
transition: fade
fonts:
  sans: Inter
  serif: Space Grotesk
  weights: '400,600,700'
layout: declaracion
align: end
logo: top
bar: true
eyebrow: WyeWorks · 2026
---

# Iniciativa Rust

<!--
Apertura (1 min). El objetivo de la charla es generar enganche, mostrar que los proyectos son bien técnicos y copados y convencerlos de que ellos eventualmente pueden trabajar en Rust tambien.
-->

---
layout: contenido
eyebrow: Apertura
tight: true
---

# Un año después

<Compare>
<Side year="2025" headline="2 personas">

- Incertidumbre
- 1 solo proyecto
- Trabajo muy experimental
- Difícil crecer
- Déficit económico
- Inversión incierta
- No mucho entusiasmo

</Side>
<CompareArrow />
<Side year="2026" headline="7 personas" dark>

- 4 proyectos con AWS
- Trabajo valiosísimo
- OSS: dial9, nextest, sccache, etc
- Más posibilidad de crecer
- Guild funcionando, más enganche
- Apuesta seria y fuerte
- Rentable económicamente
- Más leads
- Estrategia y estructura comercial

</Side>
</Compare>

<!--
Apertura (5 min).
2025 (Julián): éramos 2 personas, con mucha incertidumbre y un solo proyecto. El trabajo era muy experimental, hacíamos cosas que no se sabía si se iban a usar, era difícil crecer y la iniciativa estaba en déficit económico. La inversión en Rust de parte de wye era incierta. No había mucho entusiasmo y/o el entusiasmo se apagaba rápido porque no pasaba mucha cosa.
2026 (Pasto): somos 7 personas con 4 proyectos con AWS. El trabajo que hacemos es valiosísimo. El trabajo OSS es mucho más reconocido: dial9, que usa hasta OpenAI, nextest, sccache, rustc, cargo, tenemos mucha más exposición. Hay más posibilidades en general de crecer. Guild está funcionando lindo, hay un grupo de interés en Rust y la gente enganchada. La apuesta pasó a ser seria y fuerte: hoy somos rentables económicamente, hay estrategia y estructura comercial y muchos más leads.
-->

---
layout: contenido
eyebrow: Summit 2025
---

# Plan 2026

<Cards>
<Card eyebrow="Etapa 1" number="1" top>

### Armar equipo

- Rust Guild
- Preparar equipos y onboarding
- Hablar con potenciales clientes

</Card>
<Card eyebrow="Etapa 2" number="2" top>

### Potenciar

- Capacidad de abrir proyectos
- Arrancar un proyecto nuevo
- Mejorar la situación financiera

</Card>
<Card eyebrow="Etapa 3" number="3" top>

### Consolidar

- Al menos 2 equipos estables
- Retorno económico
- Una estrategia consolidada

</Card>
</Cards>

<!--
Plan 2026 (2 min). Esto es lo que nos propusimos hace un año.
-->

---
layout: contenido
eyebrow: Qué pasó
---

# Plan 2026

<Stages>
<Stage eyebrow="Etapa 1" title="Armar equipo" status="completa">

Tenemos equipo y entusiasmo en general. Guild funcionando perfectamente.

</Stage>
<Stage eyebrow="Etapa 2" title="Potenciar" status="completa">

Tenemos capacidad para abrir proyectos, nuevos proyectos con AWS y mejor situación financiera.

</Stage>
<Stage eyebrow="Etapa 3" title="Consolidar" status="casi">

Ya hay retorno económico y equipos bastante estables. Varios proyectos pero la misma fuente de financiamiento. Lo ideal sería un segundo cliente.

</Stage>
</Stages>

<!--
Qué pasó (4 min). Medimos contra nuestro propio plan: Etapa 1 completa, Etapa 2 completa, Etapa 3 casi. Lo único que falta para consolidar es que la plata no venga toda de un solo cliente.
-->

---
layout: contenido
eyebrow: En qué trabajamos
tight: true
---

# Problemas difíciles y copados

<Projects>
<Project name="Metrique">Low overhead wide-event metrics</Project>
<Project name="Dial9">Flight recorder for Tokio and Rust</Project>
<Project name="nextest">Productionize Test Caching</Project>
<Project name="sccache">Remote Execution</Project>
<Project name="Symposium">Making AI write better rust</Project>
<Project name="HR Subtyping">Convert HR Subtyping into a coercion</Project>
<Project name="AFIDT">Async Functions in Dyn Traits</Project>
<Project name="Bench">Investigando Solana</Project>
</Projects>

<!--
En qué trabajamos (unos 20 min). El marco: todos son proyectos con desafíos técnicos re interesantes. Dar una idea de alto nivel de en qué consiste el proyecto y qué desafío técnico tiene.
Hablar también de la primer experiencia en Rust de Facu Luzko, Emi o Germán Botto.
Aprender trabajando de manera autodidacta y con  la IA.
Bajar el miedo a participar en proyectos de Rust.
-->

---
layout: contenido
eyebrow: A dónde vamos
tight: true
---

# Cuál es la idea?

<Bento>
<Card icon="i-carbon-partnership">

### Afianzar relación con AWS

Hoy son 4 proyectos y cada vez trabajamos con más autonomía.

</Card>
<Card icon="i-carbon-search">

### 2do cliente

Hoy todo el ingreso viene de un solo cliente.

</Card>
<Card icon="i-carbon-rocket">

### Bench

Germán aprontandose para atacar nuevos proyectos. Armando ideas concretas para Solana y/o Encore.

</Card>
<Card icon="i-carbon-growth">

### Crecer la iniciativa

Rust sigue creciendo y nuestros proyectos tienen desafíos técnicos que copan.

</Card>
<Card icon="i-carbon-collaborate">

### Estructura comercial

Estamos mucho más armados comercialmente.

</Card>
</Bento>

<!--
Afianzar relación con AWS: hoy son 4 proyectos. Contar cómo fue creciendo el equipo: Juli, Facu x 2, luego Franco, luego Tina y luego Emi. Pasamos de trabajar muy cerca con Russel a tener cierta autonomía. Estamos armando proyect goals para definir trabajo 2027.

2do cliente: vamos por buen camino, pero esto se demuestra con proyectos concretos. Hoy todo el ingreso de la iniciativa viene de un solo cliente.

Bench: Germán está generando capacidad para atacar nuevos proyectos, con la idea de ir directamente por un par de leads que tenemos: Solana o Encore.

Crecer la iniciativa: en el último año un montón más de empresas decidieron adoptar Rust.
Android: Google reporta 1000× menos densidad de vulnerabilidades de memoria en su código Rust que en C/C++ (nov 2025).
Linux: en diciembre de 2025 se decidió que Rust deja de ser experimental en el kernel.
Bun: Jarred Sumner lo portó de Zig a Rust en 11 días con agentes (mergeado el 14 de mayo de 2026).
GitHub: el runtime de Copilot quedó 100% en Rust el 21 de agosto de 2026, con unas 832 mil líneas de Rust, hecho principalmente por una persona con agentes.
HEY: En la keynote de Rails World 2026 (septiembre, Austin), DHH contó que 37signals está reconstruyendo HEY con un servidor de mail en Rust escrito por agentes, y dijo “Agents like Rust. Great!”.
Microsoft tiene un proyecto de investigación con la meta de eliminar C/C++ para 2030 (aclararon que es investigación, no un plan corporativo).

Crecer la iniciativa: tenemos proyectos desafiantes, y a mucha gente lo que la engancha de Rust es justamente eso, problemas difíciles e interesantes. Es difícil pero vamos a crecer a nivel comercial y a nivel equipo.

Estructura comercial: armamos una buena estructura comercial, tenemos la idea de armar un grupo de trabajo alrededor de esto. Estamos en la Rust Commercial Network, que la Foundation lanzó en junio de 2026 como “la voz colectiva de Rust en producción”, con miembros fundadores como AWS, Arm, Google, JetBrains, Microsoft y OpenAI. Y en general estamos bien conectados.
-->

---
layout: declaracion
size: lg
logo: bottom
bar: true
class: ww-big-h2
---

## ¿Preguntas?
