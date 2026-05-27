# 🤾‍♂️ ¡Aprende Balonmano! - Infografía Interactiva (PWA)

Una Aplicación Web Progresiva (PWA) interactiva y completamente autocontenida en un único archivo HTML. Diseñada como una herramienta educativa para niños y niñas de educación primaria (8 a 12 años), explicando los conceptos básicos del balonmano de forma lúdica, accesible y visual.

## 🎯 Propósito Pedagógico

El diseño de esta infografía se basa en los **Principios de Diseño Instruccional de Mayer**:
* **Principio de Coherencia:** Eliminación de elementos visuales que no cumplen una función didáctica directa.
* **Idea Central:** Enfoque en un único objetivo claro ("marcar goles").
* **Carga Cognitiva Reducida:** Presentación de solo 4 datos clave en lenguaje sencillo.
* **Narrativa Guiada:** Uso de una mascota ("Balón", el perrito) que interactúa directamente con el alumno mediante preguntas y retroalimentación.

## ✨ Características Principales

* **Autocontenida (Single-File):** Todo el código (HTML, CSS, JavaScript, Service Worker y Web App Manifest) vive dentro de un único archivo `.html`. No requiere servidor backend ni carpetas de assets.
* **Soporte Offline (PWA):** Gracias a la inyección dinámica del Service Worker, la aplicación puede instalarse en dispositivos móviles y de escritorio, y funcionar sin conexión a internet.
* **Diseño Responsivo:** Interfaz adaptativa (Mobile-first) que se ve perfecta en pantallas pequeñas (desde 375px) hasta monitores de escritorio.
* **Interactividad y Gamificación:** Incluye animaciones CSS suaves (hover, wiggle, bounce) y un quiz interactivo de 8 preguntas con retroalimentación inmediata.
* **Accesibilidad:** Uso de etiquetas semánticas (`<header>`, `<main>`, `<section>`), atributos `aria-live` para lectores de pantalla en el quiz, y respeto por la preferencia de reducción de movimiento (`prefers-reduced-motion`).

## 🛠️ Tecnologías Utilizadas

* **HTML5:** Estructura semántica y SVG embebido para el campo de juego.
* **CSS3:** Variables nativas, CSS Grid/Flexbox, animaciones `@keyframes` y media queries.
* **JavaScript (Vanilla):** Lógica del quiz, generación de Data URIs (Blob) para el Service Worker y el Manifest, y manejo del prompt de instalación PWA.
* **Google Fonts:** Tipografías *Baloo 2* (Títulos) y *Nunito* (Cuerpo de texto).

## 🚀 Cómo usar este proyecto

Dado que es un archivo único, tienes varias formas de ejecutarlo:

1. **Uso básico:** Simplemente haz doble clic en el archivo `balonmano-ninos.html` para abrirlo en tu navegador web predeterminado.
2. **Uso como PWA (Instalable):** Para que el navegador detecte el Service Worker y permita la instalación (botón "Instalar" en el banner), debes servir el archivo a través de un servidor local (localhost) o un entorno seguro (HTTPS). 
   * Si usas VS Code, la extensión **Live Server** es ideal para esto.
   * Una vez abierto en el servidor local, verás el banner animado que te invitará a instalar la app tras unos segundos.

## ✏️ Personalización Importante

Antes de publicar o entregar este archivo, asegúrate de editar el pie de página (footer) en el código HTML con tus datos:

```html
<p>Creado por: <strong>[Ana Cuadros Valeriano]</strong></p>
