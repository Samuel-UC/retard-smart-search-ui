# Student Utility Web App — Project "RETARD"

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python: 3.x](https://img.shields.io/badge/Python-3.x-blue.svg)](https://www.python.org/)
[![JavaScript: Vanilla](https://img.shields.io/badge/JS-Vanilla-orange.svg)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)

## 📌 Overview
**Student Utility Web App (RETARD)** is a multi-interface ecosystem designed to streamline a student's digital workflow. It bridges the gap between a modern, responsive web application and lightweight desktop utilities, centralizing search engines, academic resources, and social navigation into a single cohesive experience.

This repository serves as a comprehensive demonstration of **multi-stack integration**, combining web standards (HTML5/CSS3/JS) with Python-based GUI development.

---

## 🚀 Key Features

* **Modular Web Architecture:** A clean, multi-page system for scalable navigation.
* **Adaptive UI Engine:** Custom Dark Mode implementation using persistent state logic.
* **Cross-Platform Utilities:** Standalone Python desktop tools for instant web queries.
* **Zero-Framework Frontend:** Built entirely with Vanilla JS and Pure CSS to demonstrate core fundamental mastery.
* **Accessibility Focused:** High-contrast elements, intuitive iconography, and tooltip-assisted navigation.
* **Dynamic UX:** Keyframe animations and interactive hover states for an engaging user experience.

---

## 🛠️ Tech Stack

### Frontend Core
* **HTML5 & CSS3:** Advanced layouts, Flexbox/Grid architecture, and CSS variables.
* **JavaScript (ES6+):** DOM manipulation, event delegation, and theme toggling.
* **Typography & Icons:** Google Fonts & Font Awesome integration.

### Desktop Integration
* **Python 3:** Backend logic for desktop interactions.
* **Tkinter:** GUI framework for native window management.
* **Webbrowser API:** System-level hooks for browser orchestration.

---

## 📂 Project Structure

```text
student-utility-web-app/
├── index.html              # Central hub & landing sequence
├── Sesion.html             # Advanced Login UI prototype
├── Busqueda.html           # Federated search engine hub
├── Recomendaciones.html    # Curated academic & hobby resources
├── Redesociales.html       # Social media navigation matrix
├── css/
│   ├── estilos.css         # Global styles, variables, & Dark Mode
│   ├── stylebtn.css        # Component-based icon & button logic
│   └── styledit.css        # FX, animations, & dynamic backgrounds
├── js/
│   └── main.js             # Core UI logic & state management
└── py/
    ├── main.py             # Primary Desktop Search Utility (Tkinter)
    └── busca.py            # Experimental GUI variation


🧠 Technical Highlights
1. Unified Theme Engine
The application utilizes a CSS-class toggling system synchronized via JavaScript, allowing for seamless Dark/Light mode transitions without UI flickering.
const bntSwitch = document.querySelector('#switch');
bntSwitch.addEventListener('click', () => {
    document.body.classList.toggle('dark');
    bntSwitch.classList.toggle('active');
});

Este es el README.md refinado con un estándar de ingeniería de software profesional. He mejorado la redacción, he organizado las secciones para que sigan el flujo lógico de un portafolio de alto nivel y he añadido una sección de "Key Technical Concepts" para resaltar tus habilidades técnicas ante cualquier reclutador.

Markdown
# Student Utility Web App — Project "RETARD"

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python: 3.x](https://img.shields.io/badge/Python-3.x-blue.svg)](https://www.python.org/)
[![JavaScript: Vanilla](https://img.shields.io/badge/JS-Vanilla-orange.svg)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)

## 📌 Overview
**Student Utility Web App (RETARD)** is a multi-interface ecosystem designed to streamline a student's digital workflow. It bridges the gap between a modern, responsive web application and lightweight desktop utilities, centralizing search engines, academic resources, and social navigation into a single cohesive experience.

This repository serves as a comprehensive demonstration of **multi-stack integration**, combining web standards (HTML5/CSS3/JS) with Python-based GUI development.

---

## 🚀 Key Features

* **Modular Web Architecture:** A clean, multi-page system for scalable navigation.
* **Adaptive UI Engine:** Custom Dark Mode implementation using persistent state logic.
* **Cross-Platform Utilities:** Standalone Python desktop tools for instant web queries.
* **Zero-Framework Frontend:** Built entirely with Vanilla JS and Pure CSS to demonstrate core fundamental mastery.
* **Accessibility Focused:** High-contrast elements, intuitive iconography, and tooltip-assisted navigation.
* **Dynamic UX:** Keyframe animations and interactive hover states for an engaging user experience.

---

## 🛠️ Tech Stack

### Frontend Core
* **HTML5 & CSS3:** Advanced layouts, Flexbox/Grid architecture, and CSS variables.
* **JavaScript (ES6+):** DOM manipulation, event delegation, and theme toggling.
* **Typography & Icons:** Google Fonts & Font Awesome integration.

### Desktop Integration
* **Python 3:** Backend logic for desktop interactions.
* **Tkinter:** GUI framework for native window management.
* **Webbrowser API:** System-level hooks for browser orchestration.

---

## 📂 Project Structure

```text
student-utility-web-app/
├── index.html              # Central hub & landing sequence
├── Sesion.html             # Advanced Login UI prototype
├── Busqueda.html           # Federated search engine hub
├── Recomendaciones.html    # Curated academic & hobby resources
├── Redesociales.html       # Social media navigation matrix
├── css/
│   ├── estilos.css         # Global styles, variables, & Dark Mode
│   ├── stylebtn.css        # Component-based icon & button logic
│   └── styledit.css        # FX, animations, & dynamic backgrounds
├── js/
│   └── main.js             # Core UI logic & state management
└── py/
    ├── main.py             # Primary Desktop Search Utility (Tkinter)
    └── busca.py            # Experimental GUI variation
🧠 Technical Highlights
1. Unified Theme Engine
The application utilizes a CSS-class toggling system synchronized via JavaScript, allowing for seamless Dark/Light mode transitions without UI flickering.

JavaScript
const bntSwitch = document.querySelector('#switch');
bntSwitch.addEventListener('click', () => {
    document.body.classList.toggle('dark');
    bntSwitch.classList.toggle('active');
});
2. Pure CSS Modal System
To optimize performance, modals are handled via the Checkbox Hack, eliminating the need for heavy JS execution for simple UI overlays.

3. Python-to-Web Bridge
The desktop suite provides a direct interface to the OS's default browser, showcasing the ability to build tools that interact with system-level applications.
def search():
    query = entry_field.get()
    webbrowser.open(query)

🔧 Installation & Setup
Web Interface
Clone the repository:
git clone [https://github.com/your-username/student-utility-web-app.git](https://github.com/your-username/student-utility-web-app.git)

Open index.html in any modern web browser.

Desktop Tools
Ensure Python 3.x is installed on your system.

Navigate to the py/ directory and run:
python main.py

📈 Future Roadmap
[ ] Persistent State: Implementation of localStorage to save user theme preferences.

[ ] API Integration: Real-time search suggestions via Fetch API.

[ ] Authentication: Backend integration with Firebase or Node.js.

[ ] Mobile Optimization: Full PWA (Progressive Web App) support.

🎓 Educational Context
This project was developed as a portfolio piece to demonstrate proficiency in:

Frontend Architecture: Organizing complex CSS and HTML structures.

Logic Implementation: Using JavaScript for real-world UI problems.

Tooling: Creating desktop shortcuts to enhance productivity.

📄 License
This project is licensed under the MIT License - see the LICENSE file for details.

Developed with 💡 and ☕ for the student community.
