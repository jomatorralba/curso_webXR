# 🥽 WebXR desde cero

**Aprende WebXR paso a paso con mini-retos para Meta Quest. Solo HTML, sin instalar nada.**

> Cada reto enseña una sola cosa. Editas, subes y lo ves en las gafas en minutos.

---

## ¿De qué va esto?

La realidad virtual no tiene por qué ser complicada. Con **A-Frame** y **WebXR** puedes crear escenas 3D usando etiquetas HTML, igual que harías una página web normal. Y lo mejor: se abre directamente desde el **navegador de las Meta Quest**, sin pasar por ninguna tienda de apps.

Este repositorio es el camino que yo seguí para aprenderlo — reto a reto, sin abrumarme.

---

## 🧰 Lo que necesitas

| Qué | Por qué |
|---|---|
| Gafas Meta Quest (2, 3 o Pro) | Para verlo en VR |
| Un editor de texto | TextMate, VS Code, el que uses |
| Un hosting o GitHub Pages | Para publicar el HTML con URL pública |
| Nada más | En serio, nada más |

---

# 🗺️ Ruta de aprendizaje

```
┌─────────────────────────────────────────┐
│           Reto 0 — Arrancar algo        │
│   HTML + A-Frame en el navegador Quest  │
└──────────────────────┬──────────────────┘
                       │
                       ▼
┌─────────────────────────────────────────┐
│     Reto 1 — Poner objetos en escena    │  🟢 Mundo 3D
│     Posición, rotación, color           │
└──────────────────────┬──────────────────┘
                       │
                       ▼
┌─────────────────────────────────────────┐
│     Reto 2 — Hacer que algo se mueva    │  🟢 Mundo 3D
│     Animaciones con animation           │
└──────────────────────┬──────────────────┘
                       │
                       ▼
┌─────────────────────────────────────────┐
│     Reto 3 — Mirar algo para activarlo  │  🟣 Interacción
│     Cursor de gaze y evento click       │
└──────────────────────┬──────────────────┘
                       │
                       ▼
┌─────────────────────────────────────────┐
│     Reto 4 — Usar los controladores     │  🟣 Interacción
│     a-laser-controls, detectar botones  │
└──────────────────────┬──────────────────┘
                       │
                       ▼
┌─────────────────────────────────────────┐
│     Reto 5 — Cargar un modelo 3D        │  🟠 Contenido real
│     GLB/GLTF con a-gltf-model           │
└──────────────────────┬──────────────────┘
                       │
                       ▼
┌─────────────────────────────────────────┐
│     Reto 6 — Mini escena interactiva    │  🟠 Contenido real
│     Galería, puzzle o quiz en VR        │
└─────────────────────────────────────────┘
```

> 🟢 Mundo 3D — 🟣 Interacción — 🟠 Contenido real

Cada reto enseña **una sola cosa**. Completa uno antes de pasar al siguiente.

---

## 🗺️ Los retos

### ✅ Reto 0 — Arrancar algo
El objetivo es únicamente completar el ciclo: escribir HTML → subir → ver en VR. Una caja, un suelo, un cielo. Diez líneas de código.

📁 [`reto-00-arrancar/`](Reto-0)

---

### ✅ Reto 1 — Poner objetos en la escena
Entender el sistema de coordenadas X Y Z y colocar objetos en el espacio. Cajas, esferas, cilindros, texto. Todo con atributos HTML.

📁 [`reto-01-objetos/`](Reto-1)
🌏 (https://josemariatorralba.com/vr/Reto-1.html)

---

### ✅ Reto 2 — Hacer que algo se mueva
Animar objetos con el componente `animation`. Girar, flotar, pulsar. Sin una sola línea de JavaScript.

📁 [`reto-02-animaciones/`](Reto-2)
🌏 (https://josemariatorralba.com/vr/Reto-2.html)
---

### ✅ Reto 3 — Mirar algo para activarlo
Interacción por mirada (gaze). Detectar que el usuario mira un objeto y usarlo como disparador.

📁 [`reto-03-gaze/`](Reto-3)
🌏 (https://josemariatorralba.com/vr/Reto-3.html)

---

### ✅ Reto 4 — Usar los controladores
Laser pointer y detección de botones con los mandos de las Quest.

📁 [`reto-04-controladores/`](Reto-4)
🌏 (https://josemariatorralba.com/vr/reto4.html)

---

### ✅ Reto 5 — Cargar un modelo 3D
Importar modelos GLB/GLTF en la escena. Dónde encontrarlos gratis y cómo ajustarlos.

### ⚠️ Antes de empezar — servidor local

Descarga los modelos en la misma carpeta donde tengas el .html
y renombralo por modelo.glb
-> modelos gratis (https://poly.pizza/)

A partir del **Reto 5** necesitas arrancar un servidor local
para probar los archivos en tu ordenador.

El navegador bloquea la carga de archivos 3D (GLB) cuando
abres el HTML directamente desde tu carpeta. Es una restricción
de seguridad de todos los navegadores modernos.

## Cómo arrancar el servidor (Mac y Linux)

1. Abre la Terminal
2. Navega a la carpeta del reto:
   cd ~/Desktop/reto-05 (o la carpeta en que lo tengas)
3. Arranca el servidor:
   python3 -m http.server 8000
4. Abre en el navegador:
   http://localhost:8000

## En Windows

python -m http.server 8000

## Cuando lo subas a un servidor

Esto solo es necesario en local. Cuando subas los
archivos a Hostinger o GitHub Pages el servidor
externo lo gestiona solo y no necesitas hacer nada.

📁 [`reto-05-modelos/`](Reto-5)
🌏 (https://josemariatorralba.com/vr/index.html)

---

### ✅ Reto 6 — Mini escena interactiva de cancelación visual
Este es el reto final del curso. No aprendes una sola cosa nueva — **lo juntas todo**.

Objetos generados con JavaScript, animaciones, interacción por mirada y por controladores, y un objetivo clínico real: una tarea de cancelación visual para entrenar la atención selectiva.

---

## Qué hace esta escena

El paciente aparece rodeado de **24 figuras geométricas** distribuidas en las tres dimensiones. Entre todas hay **8 esferas rojas** — el objetivo. El resto son distractores de distintas formas y colores.

La tarea es sencilla: **encuentra y cancela todas las esferas rojas**. Al activarlas se vuelven grises. Los distractores no responden — hay que ignorarlos.

---

## Cómo se activan los estímulos

Exactamente igual que aprendiste en los retos anteriores:

- **Reto 3** — mira una esfera roja durante 1.5 segundos → se cancela sola
- **Reto 4** — apunta con el láser y pulsa el gatillo → se cancela

Puedes usar cualquiera de las dos formas, o combinarlas.

---

## Qué entrena esta tarea

| Variable cognitiva | Mecanismo |
|---|---|
| Atención selectiva | Buscar el objetivo entre distractores |
| Rastreo visual 3D | Buscar en 360° a tu alrededor |
| Inhibición de respuesta | No activar los distractores |

---

## Cómo graduar la dificultad

Al inicio del script hay cuatro constantes que puedes cambiar sin tocar nada más:

```javascript
const TOTAL_OBJETIVOS  = 8;    // menos objetivos = más difícil encontrarlos
const TOTAL_DISTRACTOR = 16;   // más distractores = más carga atencional
const DISTANCIA_MIN    = 1.5;  // más lejos = más esfuerzo de rastreo
const DISTANCIA_MAX    = 3.5;
```

Para una versión más sencilla, comenta el bloque `animation__flotar` — los estímulos quedarán estáticos en lugar de flotar.

📁 [`reto-06-proyecto/`](Reto-6)
🌏 (https://josemariatorralba.com/vr/reto6.html)

---
## Lo que has aprendido en el curso

Llegando hasta aquí sabes:

- Montar una escena WebXR que funciona directamente en el navegador de las Quest
- Colocar y transformar objetos en el espacio 3D
- Animar propiedades con el componente `animation`
- Detectar la mirada del usuario con un cursor de gaze
- Usar los controladores y el hand tracking para interactuar
- Cargar modelos 3D en formato GLB
- Generar objetos dinámicamente con JavaScript
- Responder a eventos y actualizar la escena en tiempo real

Eso es WebXR desde cero. A partir de aquí, el límite es lo que quieras construir.

---

## 🚀 Cómo empezar

```bash
git clone https://github.com/jomatorralba/webxr-retos.git
```

Abre la carpeta del reto que quieras, edita el `.html`, cortalo, pegalo, haz lo que quieras, todos los retos tienen en código comentado para que lo entendais todo a la perfección, súbelo a tu hosting. Luego abre esa URL desde el **Meta Quest Browser** y pulsa **Enter VR**.

---

## 🛠️ Tecnologías

- [A-Frame](https://aframe.io) — VR con etiquetas HTML
- [WebXR](https://immersiveweb.dev) — estándar web para VR/AR
- [Meta Quest Browser](https://www.meta.com/es-es/experiences/meta-quest-browser/) — soporte WebXR nativo

---

## 📚 Recursos útiles

- [Documentación de A-Frame](https://aframe.io/docs/)
- [Modelos 3D gratis — Poly Pizza](https://poly.pizza)
- [Modelos 3D gratis — Sketchfab](https://sketchfab.com/features/free-3d-models)

---

## 📄 Licencia

APACHE 2.0

---

<p align="center">Hecho con curiosidad y unas Meta Quest 🥽</p>
