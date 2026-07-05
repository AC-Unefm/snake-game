# 🐍 Snake Classic Game

> Un juego clásico de Snake construido exclusivamente con tecnologías web nativas (HTML, CSS y JavaScript vanilla). Sin frameworks, sin dependencias, sin herramientas de compilación. Un único archivo `index.html`

## 🎮 ¡Juega en Línea!

Puedes disfrutar del juego directamente desde el navegador a través de nuestro acceso oficial de alta velocidad:

👉 **[snake-game.acscicomp.com](https://snake-game.acscicomp.com)**

---

### 🌐 Accesos Alternativos y Espejos
Si el acceso principal presenta alguna saturación, puedes utilizar el espejo nativo de GitHub Pages:
* [Espejo Alternativo (GitHub Pages)](https://ac-unefm.github.io/snake-game)

### 🛠️ Código Fuente
Si eres estudiante o investigador y deseas revisar la lógica del juego, puedes clonar este repositorio directamente:
```bash
git clone https://github.com/ac-unefm/snake-game.git
```
&nbsp;&nbsp;
[Reportar un problema acá](https://github.com/ac-unefm/snake-game/issues)

---

## ¿De qué trata este proyecto?

Este proyecto nació como demostración de una idea simple pero poderosa de que, con conocimiento sólido de las herramientas básicas y estandares de la web, se pueden construir experiencias completas, accesibles y bien diseñadas sin necesidad de sobrecargar el proyecto con dependencias externas.

Todo el juego — lógica, estilos, marcado, persistencia y accesibilidad — vive en un único archivo autocontenido, que lo convierte en un recurso ideal y didáctico para estudiantes y desarrolladores que quieran ver cómo se aplican buenas prácticas reales en un proyecto concreto y funcional.

Es un ejemplo práctico que demuestra cómo construir una aplicación web robusta y con características modernas utilizando exclusivamente las APIs nativas del navegador, sin dependencias externas ni herramientas de compilación.

---

## Características y Cómo jugar

- 🎮 **Dificultad progresiva**: La velocidad aumenta cada 5 puntos
- 🏆 **Sistema de sesiones:** Cada partida agrupa 5 intentos con estadísticas detalladas.
- 💾 **Persistencia:** Mejor puntuación guardada localmente en `localStorage`
- 📊 **Panel de resultados:** Con métricas por intento (puntuación, nivel, duración, recorrido, velocidad máxima y eficiencia).
- 📱 **Responsive y táctil** — funciona en móvil, tablet y desktop; controles por swipe y D-pad en pantallas táctiles
- 🌑 **Modo Oscuro Nativo:** Adaptable automáticamente según las preferencias del sistema, nativo, sin configuración.

## Controles

### Teclado

| Acción | Tecla |
|---|---|
| Iniciar / reiniciar intento | `Enter` o `Espacio` |
| Mover la serpiente | `↑` `↓` `←` `→` |
| Abrir ayuda | `?` o `H` |
| Cerrar ayuda / modal | `Escape` |

### Táctil (móvil y tablet)

| Acción | Gesto |
|---|---|
| Mover la serpiente | Deslizar en cualquier dirección sobre el tablero |
| Iniciar / reiniciar | Tocar el tablero |
| Controles direccionales | D-pad visible bajo el tablero en pantallas táctiles |
| Abrir ayuda | Botón `?` en la esquina superior derecha |

**Objetivo:** *Evita las paredes y tu propio cuerpo. Come la comida roja para crecer.*
*Cada sesión tiene 5 intentos. Al completarlos, verás un resumen con tus estadísticas.*

---

## 🛠️ Enfoque Técnico y Conceptos Demostrados

A pesar de su simplicidad estructural en un único archivo, el código implementa estándares rigurosos y buenas prácticas de desarrollo web moderno, sirviendo como un recurso didáctico completo.

### 🎮 Arquitectura del Juego y Gráficos
* **Game Loop Dinámico:** Control del ciclo de actualización y de la dificultad progresiva mediante `setTimeout` recursivo, permitiendo variaciones de velocidad en tiempo real.
* **Canvas API 2D:** Renderizado avanzado de primitivas y optimización gráfica utilizando `save/restore`, efectos de iluminación con `shadowBlur` y trazados fluidos con `arcTo`.

### 🎨 Diseño y Estructura Interactiva
* **Estructura Semántica:** Maquetación limpia basada en HTML5 semántico.
* **Estilos Fluidos y Variables CSS:** Implementación de variables nativas para un *theming* consistente y uso de `clamp()` para lograr un diseño responsive y fluido.
* **Canvas Responsive:** Escalado del canvas mediante CSS y media queries dedicadas para adaptar el layout a escritorio, tablet, móvil y orientación landscape.
* **Modo Oscuro Nativo:** Integración automatizada que respeta las preferencias del sistema operativo mediante media queries (`@media`).

### 📱 Interactividad Avanzada y Accesibilidad
* **Touch Events API:** Soporte completo para dispositivos móviles mediante detección nativa de gestos (*swipe detection*), prevención de scroll accidental con `touch-action: none` y renderizado de un D-pad táctil dinámico.
* **Accesibilidad Web (WAI-ARIA 1.2):** Cumplimiento de estándares de inclusión utilizando atributos dinámicos (`aria-live`, `aria-modal`, `aria-hidden`, roles semánticos y `aria-describedby`).
* **Control por Teclado Completo:** Navegación e interacción total mediante teclado, gestión de *focus visible*, técnica de *focus trap* en diálogos interactivos, atajos para cierre de modales con `Escape` y enlaces de salto rápido (*skip links*).
* **Respeto al Usuario:** Soporte integrado para `prefers-reduced-motion`, desactivando animaciones según la configuración del sistema operativo.

### 🔒 Resiliencia, Seguridad y Documentación
* **Persistencia Segura:** Gestión robusta del almacenamiento local con `localStorage` blindado mediante bloques `try/catch` para el manejo de excepciones.
* **Seguridad del DOM (Anti-XSS):** Construcción segura de elementos utilizando `createElement` sobre la manipulación directa con `innerHTML`, mitigando riesgos de inyección de código.
* **Content Security Policy (CSP):** Configuración de directivas de seguridad básicas directamente en el cliente, operando de forma segura sin necesidad de dependencias del servidor.
* **Documentación Técnica Estándar:** Código fuente 100% autodocumentado utilizando la sintaxis formal de **JSDoc** en todas sus funciones.
* **Stack Minimalista:** JavaScript ES2020 vanilla puro. Sin npm. Sin webpack. Sin React. Sin nada más.

---

## 💻 Ejecución Local

No requiere de ningún servidor ni proceso de instalación:

1. Clona el repositorio o descarga el archivo `index.html`.
2. Haz doble clic en `index.html` para abrirlo directamente en cualquier navegador moderno.

*(Opcional para desarrollo)*: Puedes levantar un servidor local rápido ejecutando:

```bash
python -m http.server 8080
# o
npx serve .
```

---

## 📄 Licencia

Copyright (c) 2026 Adolfo J. Cardozo S. [<acardozos@correo.unefm.edu.ve>]
Distribuido bajo la licencia **MIT**. Siéntete libre de usar, modificar y distribuir el código con su respectiva atribución. Ver [Licencia MIT](LICENSE) para más detalles.

---

## 👨‍💻 Autor

Desarrollado por **[Adolfo J. Cardozo S.](mailto:acardozos@correo.unefm.edu.ve)**
Profesor Universitario Jubilado e Ingeniero Civil, Consultor especializado en Computación Científica, Computer Vision e IA, e Investigador en Ingeniería Hidráulica y Transporte de Sedimentos (Nivel ScD Candidate)

> *"La simplicidad es el alma de la eficiencia."* — Austin Freeman

---
*Más proyectos y recursos en* **[acscicomp.com](https://acscicomp.com)** *(próximamente)*
