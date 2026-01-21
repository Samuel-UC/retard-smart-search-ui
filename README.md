# RETARD — Multi-Interface Search & Navigation System

## Overview
**RETARD** is a dual-interface navigation system designed to bridge the gap between desktop functionality and modern web experiences. The project focuses on accessibility, visual clarity, and intuitive UX, providing tools tailored for diverse user demographics.

The system integrates a **Python-based desktop suite** with a **responsive web application**, demonstrating how different technologies can coexist to provide seamless access to web resources.

---

## Project Objectives
* **Universal Accessibility:** Providing simplified interfaces for older users while maintaining a modern aesthetic for younger demographics.
* **Direct Search Experience:** Minimizing friction in accessing global search engines.
* **Multi-Technology Integration:** Demonstrating the interoperability between Python (Tkinter) and vanilla web technologies (HTML/CSS/JS).
* **UI/UX Research:** Focus on visual recognition over heavy text to reduce cognitive load.

---

## Tech Stack

### Desktop Core
* **Language:** Python 3
* **Library:** Tkinter (GUI)
* **Integration:** `webbrowser` module for system-level browser control.

### Web Interface
* **Frontend:** HTML5 & CSS3 (Advanced animations and responsive layouts).
* **Logic:** Vanilla JavaScript (ES6+).
* **Assets:** Google Fonts & Font Awesome.
* **Note:** This project is built **without frameworks** to demonstrate core proficiency in web standards.

---

## System Components

### 1. Desktop Applications (Python)
The `py/` directory contains standalone tools designed for high-contrast visibility and direct interaction.

* **`main.py`**: A high-contrast search utility. Features large text elements and system-level hooks to open queries directly in the default browser.
* **`busca.py`**: An experimental secondary interface (labeled *Astral*) used for testing alternative GUI layouts.

### 2. Web Interface Structure
The web application is modular, sharing a unified design language and a centralized state for the visual theme.

| Page | Description |
| :--- | :--- |
| `index.html` | Landing page featuring an animated title sequence. |
| `Busqueda.html` | Search engine hub (Google, Bing, DuckDuckGo, etc.). |
| `Recomendaciones.html` | Curated discovery space for niche interests (Crafts, Cooking). |
| `Redesociales.html` | Centralized visual hub for social media platforms. |
| `Sesion.html` | A comprehensive Login UI prototype with social integration. |

---

## Key Features

### Navigation & UX
* **Icon-Driven Design:** Uses visual recognition and color-coded actions to improve navigation speed.
* **Interactive Tooltips:** Contextual information on hover to maintain a clean interface.
* **Dark Mode Engine:** A custom JavaScript implementation that toggles themes across the entire DOM without page reloads.

### Styling Architecture
The CSS is decoupled into specialized modules for better maintainability:
* `stylebtn.css`: Handles complex button logic, icons, and tooltip positioning.
* `styledit.css`: Manages keyframe animations and dynamic backgrounds.
* `estilos.css`: Defines the core layout, form factor, and Dark Mode variables.

### Information Modals
A lightweight modal system implemented using **Pure CSS**, demonstrating efficient UI patterns without the overhead of external JavaScript libraries.

---

## Project Structure
```text

RETARD/
├── py/
│   ├── main.py            # Main Python GUI
│   └── busca.py           # Secondary GUI
├── css/
│   └── estilos.css        # Layout & Theme
├── js/
│   └── main.js            # Theme Logic
├── stylebtn.css           # Component Styles
├── styledit.css           # Animation Logic
├── index.html             # Entry Point
└── [Other HTML Modules]

Scope & Limitations
Backend: This is a frontend-focused prototype. There is no active database or server-side authentication.

Independence: The Python tools and the Web interface operate as independent modules within the same ecosystem.

License
This project is licensed under the MIT License.
