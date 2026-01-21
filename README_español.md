# RETARD — Sistema de Navegación y Búsqueda Multi-Interfaz

## Descripción General
**RETARD** es un sistema de navegación dual diseñado para cerrar la brecha entre la funcionalidad de escritorio y las experiencias web modernas. El proyecto se centra en la accesibilidad, la claridad visual y una experiencia de usuario (UX) intuitiva, ofreciendo herramientas adaptadas a diversos perfiles demográficos.

El sistema integra una **suite de escritorio basada en Python** con una **aplicación web responsiva**, demostrando cómo diferentes tecnologías pueden coexistir para facilitar el acceso a recursos digitales.

---

## Objetivos del Proyecto
* **Accesibilidad Universal:** Interfaces simplificadas para usuarios mayores y estéticas modernas para usuarios jóvenes.
* **Experiencia de Búsqueda Directa:** Minimizar la fricción al acceder a motores de búsqueda globales.
* **Integración Multitecnología:** Demostrar la interoperabilidad entre Python (Tkinter) y estándares web (HTML/CSS/JS).
* **Enfoque en UI/UX:** Priorizar el reconocimiento visual sobre el texto denso para reducir la carga cognitiva.

---

## Tecnologías Utilizadas

### Entorno de Escritorio
* **Lenguaje:** Python 3
* **Librería:** Tkinter (GUI)
* **Integración:** Módulo `webbrowser` para control del navegador a nivel de sistema.

### Interfaz Web
* **Frontend:** HTML5 y CSS3 (Animaciones avanzadas y diseño responsivo).
* **Lógica:** JavaScript Vanilla (ES6+).
* **Recursos:** Google Fonts y Font Awesome.
* **Nota:** El proyecto ha sido desarrollado **sin frameworks** para demostrar el dominio de los estándares web fundamentales.

---

## Componentes del Sistema

### 1. Aplicaciones de Escritorio (Python)
Ubicadas en el directorio `py/`, estas herramientas están diseñadas para ofrecer alta visibilidad e interacción directa.

* **`main.py`**: Utilidad de búsqueda de alto contraste. Incluye elementos de texto de gran tamaño y llamadas al sistema para abrir consultas en el navegador predeterminado.
* **`busca.py`**: Interfaz secundaria experimental (denominada *Astral*) utilizada para pruebas de layouts alternativos.

### 2. Interfaz Web
La aplicación web es modular y comparte una identidad visual unificada junto con un motor de estado para el tema visual.

| Página | Descripción |
| :--- | :--- |
| `index.html` | Página de inicio con secuencia de título animada. |
| `Busqueda.html` | Hub de motores de búsqueda (Google, Bing, DuckDuckGo, etc.). |
| `Recomendaciones.html` | Espacio de descubrimiento curado para intereses específicos. |
| `Redesociales.html` | Panel visual centralizado para redes sociales. |
| `Sesion.html` | Prototipo de interfaz de inicio de sesión con integración social. |

---

## Características Clave

### Navegación y UX
* **Diseño Orientado a Iconos:** Uso de reconocimiento visual y acciones codificadas por colores para aumentar la velocidad de navegación.
* **Tooltips Interactivos:** Información contextual al pasar el cursor para mantener la interfaz limpia.
* **Motor de Modo Oscuro:** Implementación personalizada en JavaScript que alterna temas en todo el DOM sin recargar la página.

### Arquitectura de Estilos (CSS)
El CSS está desacoplado en módulos especializados para mejorar la mantenibilidad:
* `stylebtn.css`: Controla la lógica de botones, iconos y posicionamiento de tooltips.
* `styledit.css`: Gestiona animaciones de fotogramas clave (keyframes) y fondos dinámicos.
* `estilos.css`: Define el diseño base, formularios y variables del Modo Oscuro.

### Sistema de Modales
Incluye un sistema de ventanas modales ligeras implementado exclusivamente con **CSS Puro**, demostrando patrones de UI eficientes sin sobrecarga de librerías externas.

---

## Estructura del Proyecto
```text
RETARD/
├── py/
│   ├── main.py            # GUI Principal en Python
│   └── busca.py           # GUI Secundaria
├── css/
│   └── estilos.css        # Layout y Temas
├── js/
│   └── main.js            # Lógica de Temas y UI
├── stylebtn.css           # Estilos de componentes
├── styledit.css           # Lógica de animaciones
├── index.html             # Punto de entrada principal
└── [Otros Módulos HTML]

Alcance y Limitaciones
Backend: Este es un prototipo de frontend. No incluye base de datos activa ni lógica de autenticación en el servidor.

Independencia: Las herramientas de Python y la interfaz Web funcionan como módulos independientes dentro del mismo ecosistema.

Licencia
Este proyecto está bajo la Licencia MIT.