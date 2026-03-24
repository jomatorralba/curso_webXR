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

## 🗺️ Los retos

### ✅ Reto 0 — Arrancar algo
El objetivo es únicamente completar el ciclo: escribir HTML → subir → ver en VR. Una caja, un suelo, un cielo. Diez líneas de código.

📁 [`reto-00-arrancar/`](./reto-0/)

---

### ✅ Reto 1 — Poner objetos en la escena
Entender el sistema de coordenadas X Y Z y colocar objetos en el espacio. Cajas, esferas, cilindros, texto. Todo con atributos HTML.

📁 [`reto-01-objetos/`](./reto-01-objetos/)

---

### ✅ Reto 2 — Hacer que algo se mueva
Animar objetos con el componente `animation`. Girar, flotar, pulsar. Sin una sola línea de JavaScript.

📁 [`reto-02-animaciones/`](./reto-02-animaciones/)

---

### 🔜 Reto 3 — Mirar algo para activarlo
Interacción por mirada (gaze). Detectar que el usuario mira un objeto y usarlo como disparador.

📁 `reto-03-gaze/` *(próximamente)*

---

### 🔜 Reto 4 — Usar los controladores
Laser pointer y detección de botones con los mandos de las Quest.

📁 `reto-04-controladores/` *(próximamente)*

---

### 🔜 Reto 5 — Cargar un modelo 3D
Importar modelos GLB/GLTF en la escena. Dónde encontrarlos gratis y cómo ajustarlos.

📁 `reto-05-modelos/` *(próximamente)*

---

### 🔜 Reto 6 — Mini escena interactiva
Proyecto final. Una galería, un puzzle o un quiz en VR combinando todo lo aprendido.

📁 `reto-06-proyecto/` *(próximamente)*

---

## 🚀 Cómo empezar

```bash
git clone https://github.com/tuusuario/webxr-retos.git
```

Abre la carpeta del reto que quieras, edita el `index.html` y súbelo a tu hosting. Luego abre esa URL desde el **Meta Quest Browser** y pulsa **Enter VR**.

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

MIT — úsalo, modifícalo y compártelo libremente.

---

<p align="center">Hecho con curiosidad y unas Meta Quest 🥽</p>
