# Student Utility Web App — Proyecto "RETARD"

[![Licencia: MIT](https://img.shields.io/badge/Licencia-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python: 3.x](https://img.shields.io/badge/Python-3.x-blue.svg)](https://www.python.org/)
[![JavaScript: Vanilla](https://img.shields.io/badge/JS-Vanilla-orange.svg)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)

## 📌 Descripción General
**Student Utility Web App (RETARD)** es un ecosistema de interfaz múltiple diseñado para optimizar el flujo de trabajo digital de un estudiante. El proyecto conecta una aplicación web moderna y responsiva con utilidades de escritorio ligeras, centralizando motores de búsqueda, recursos académicos y navegación social en una experiencia cohesiva.

Este repositorio es una demostración integral de **integración multi-stack**, combinando estándares web (HTML5/CSS3/JS) con desarrollo de interfaces gráficas en Python.

---

## 🚀 Características Clave

* **Arquitectura Web Modular:** Sistema de múltiples páginas diseñado para una navegación escalable.
* **Motor de Interfaz Adaptativo:** Implementación personalizada de Modo Oscuro mediante lógica de estado persistente.
* **Utilidades Multiplataforma:** Herramientas de escritorio independientes en Python para consultas web instantáneas.
* **Frontend "Zero-Framework":** Construido totalmente con Vanilla JS y CSS Puro para demostrar el dominio de los fundamentos básicos.
* **Enfoque en Accesibilidad:** Elementos de alto contraste, iconografía intuitiva y navegación asistida por tooltips.
* **Experiencia de Usuario Dinámica:** Animaciones basadas en keyframes y estados interactivos (*hover*) para mejorar el engagement.

---

## 🛠️ Stack Tecnológico

### Core de Frontend
* **HTML5 y CSS3:** Layouts avanzados, arquitectura Flexbox/Grid y variables CSS.
* **JavaScript (ES6+):** Manipulación del DOM, delegación de eventos y gestión de temas.
* **Tipografía e Iconos:** Integración de Google Fonts y Font Awesome.

### Integración de Escritorio
* **Python 3:** Lógica de backend para interacciones de escritorio.
* **Tkinter:** Framework de GUI para la gestión nativa de ventanas.
* **Webbrowser API:** Enlaces a nivel de sistema para la orquestación del navegador.

---

## 📂 Estructura del Proyecto

```text
student-utility-web-app/
├── index.html              # Hub central y secuencia de inicio
├── Sesion.html             # Prototipo avanzado de interfaz de Login
├── Busqueda.html           # Hub federado de motores de búsqueda
├── Recomendaciones.html    # Recursos académicos y de ocio curados
├── Redesociales.html       # Matriz de navegación de redes sociales
├── css/
│   ├── estilos.css         # Estilos globales, variables y Modo Oscuro
│   ├── stylebtn.css        # Lógica de componentes para iconos y botones
│   └── styledit.css        # Efectos visuales, animaciones y fondos dinámicos
├── js/
│   └── main.js             # Lógica central de UI y gestión de estados
└── py/
    ├── main.py             # Utilidad principal de búsqueda (Tkinter)
    └── busca.py            # Variación experimental de la interfaz
🧠 Aspectos Técnicos Destacados
1. Motor de Temas Unificado
La aplicación utiliza un sistema de alternancia de clases CSS sincronizado mediante JavaScript, permitiendo transiciones fluidas entre el modo claro y oscuro sin parpadeos visuales.

JavaScript
const bntSwitch = document.querySelector('#switch');
bntSwitch.addEventListener('click', () => {
    document.body.classList.toggle('dark');
    bntSwitch.classList.toggle('active');
});
2. Sistema de Modales en CSS Puro
Para optimizar el rendimiento, los modales se gestionan mediante la técnica de Checkbox Hack, eliminando la necesidad de ejecución pesada de JS para capas de interfaz sencillas.

3. Puente Python-Web
La suite de escritorio proporciona una interfaz directa con el navegador predeterminado del sistema operativo, demostrando la capacidad de crear herramientas que interactúan con aplicaciones a nivel de sistema.

Python
def search():
    query = entry_field.get()
    webbrowser.open(query)
🔧 Instalación y Configuración
Interfaz Web
Clona el repositorio:

Bash
git clone [https://github.com/tu-usuario/student-utility-web-app.git](https://github.com/tu-usuario/student-utility-web-app.git)
Abre index.html en cualquier navegador web moderno.

Herramientas de Escritorio
Asegúrate de tener instalado Python 3.x.

Navega al directorio py/ y ejecuta:

Bash
python main.py
📈 Hoja de Ruta (Future Roadmap)
[ ] Estado Persistente: Implementación de localStorage para guardar preferencias de tema.

[ ] Integración de API: Sugerencias de búsqueda en tiempo real mediante Fetch API.

[ ] Autenticación: Integración de backend con Firebase o Node.js.

[ ] Optimización Móvil: Soporte completo para PWA (Progressive Web App).

🎓 Contexto Educativo
Este proyecto fue desarrollado como pieza de portafolio para demostrar competencia en:

Arquitectura Frontend: Organización de estructuras complejas de CSS y HTML.

Implementación de Lógica: Uso de JavaScript para resolver problemas de UI del mundo real.

Herramientas de Productividad: Creación de accesos directos de escritorio para mejorar el flujo de trabajo.

📄 Licencia
Este proyecto está bajo la Licencia MIT. Consulta el archivo LICENSE para más detalles.

Desarrollado con 💡 y ☕ para la comunidad estudiantil.
