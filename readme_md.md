# HTML Atelier (v1.0)

**HTML Atelier** is a lightweight, single-file educational web application built to introduce beginners to HTML and foundational CSS. Designed with a clean, editorial studio aesthetic, it combines bite-sized lessons, an interactive live code sandbox, and a browser-based student gallery—all without external frameworks or build tools.

> **Note on Version 1.0:** This release represents the initial version of the project. The visual design, interactive functionality, and educational content will be expanded and improved in future updates.

---

## Features in v1.0

### 1. Home (`#home`)
* Editorial hero layout introducing the platform with clear calls to action.
* Animated hanging tag illustration displaying the HTML5 emblem.
* Instant navigation to the Lessons and Sandbox views.

### 2. Lessons (`#lessons`)
* Featured external YouTube tutorial card for learning HTML fundamentals from scratch.
* Six interactive topic cards covering core web concepts:
  * **Page Structure** (`<!DOCTYPE html>`, `<html>`, `<head>`, `<body>`)
  * **Headings & Text** (`<h1>`–`<h6>`, `<p>`)
  * **Links & Images** (`<a>`, `<img>`)
  * **Lists** (`<ul>`, `<ol>`, `<li>`)
  * **CSS Styling** (`<style>`)
  * **Forms** (`<input>`, `<button>`)
* Expandable code snippets on each card and a **"Try it" (`Попробовать`)** button that loads the snippet directly into the Sandbox.

### 3. Live Sandbox (`#sandbox`)
* Split-screen workspace with a monospace code editor on the left and a live preview inside a sandboxed `<iframe>` on the right.
* Debounced automatic preview updates as you type, plus manual **Refresh** and **Reset** controls.
* One-click **"Send to Gallery" (`Отправить в галерею`)** workflow to share creations from the editor.

### 4. Student Gallery (`#gallery`)
* Submission form allowing learners to publish work by URL or raw HTML snippet.
* Built-in starter examples alongside user-submitted cards.
* Modal preview window powered by the native HTML `<dialog>` element.
* Client-side persistence using `localStorage`, with the ability to delete custom entries.

---

## Technical Overview

* **Single-File Architecture:** Entire application—markup, styling, and logic—is self-contained in a single `.html` file (`HTML Atelier — учим вёрстку.html`) using pure HTML5, CSS3, and Vanilla JavaScript.
* **Hash-Based Routing:** Client-side view switching via URL fragments (`#home`, `#lessons`, `#sandbox`, `#gallery`) without page reloads.
* **Color System & Typography:** Styled with a 60–30–10 color palette pairing *Cormorant Garamond* display headings with *Inter* body text.
* **Adaptive & Accessible:** Supports automatic light/dark themes (`prefers-color-scheme`), reduced-motion preferences (`prefers-reduced-motion`), safe-area insets (`env(safe-area-inset-*)`), and responsive mobile layouts.

---

## Getting Started

1. Clone or download the repository.
2. Open `HTML Atelier — учим вёрстку.html` directly in any modern web browser.
3. No local server, package manager, or installation is required.

---

## Future Plans

Version 1.0 establishes the core foundation of **HTML Atelier**. Planned improvements for upcoming releases include:
* **Design:** Refined visual polish, richer UI components, and expanded theme customization.
* **Functionality:** Enhanced sandbox capabilities (such as separate HTML/CSS tabs, error hints, and export options) and improved gallery management.
* **Content:** Additional step-by-step lessons, interactive exercises, and deeper CSS layout modules.