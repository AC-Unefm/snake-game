# 🐍 Snake

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

Todo el juego — lógica, estilos, marcado, persistencia y accesibilidad — vive en un único archivo de menos de 500 líneas de código, lo que lo convierte en un recurso ideal y didáctico para estudiantes y desarrolladores que quieran ver cómo se aplican buenas prácticas reales en un proyecto concreto y funcional.

---

## Características y Cómo jugar

- 🎮 **Dificultad progresiva**: La velocidad aumenta cada 5 puntos
- 🏆 **Sistema de sesiones:** Cada partida agrupa 5 intentos con estadísticas detalladas ().
- 💾 **Persistencia:** Mejor puntuación guardada localmente en `localStorage`
- 📊 **Panel de resultados:** Con métricas por intento (puntuación, nivel, duración, recorrido, velocidad máxima y eficiencia).
- 🌑 **Modo Oscuro Nativo:** Adaptable automáticamente según las preferencias del sistema.

## Controles

| Acción | Tecla |
|---|---|
| Iniciar / reiniciar intento | `Enter` o `Espacio` |
| Mover la serpiente | `↑` `↓` `←` `→` |
| Abrir ayuda | `?` o `H` |
| Cerrar ayuda / modal | `Escape` |

**Objetivo:** *Evita las paredes y tu propio cuerpo. Come la comida roja para crecer.*

---

## 🛠️ Enfoque Técnico y Conceptos Demostrados

A pesar de su simplicidad estructural, el código implementa estándares y buenas prácticas de desarrollo moderno:

* **Lógica y Gráficos:** Game loop mediante `setTimeout` recursivo para control dinámico de velocidad y renderizado con Canvas API 2D.
* **Canvas API** — dibujo de primitivas, `save/restore`, `shadowBlur`, `arcTo`
* **Persistencia:** Manejo robusto de `localStorage` mediante bloques `try/catch`.
* **Accesibilidad (Web para todos):** Cumplimiento de **WAI-ARIA 1.2** (`aria-live`, `aria-modal`, roles semánticos , `role`, `aria-describedby`), navegación completa por teclado con *focus trap* en diálogos y respeto por `prefers-reduced-motion`.
* **Documentación:** Código completamente documentado usando sintaxis **JSDoc**.
* **Tecnologías:** HTML5 semántico, estilos CSS3 con variables y `@media`,  JavaScript ES2020 vanilla.

Sin npm. Sin webpack. Sin React. Sin nada más.

---

## 💻 Ejecución Local

No requiere de ningún servidor ni proceso de instalación:

1. Clona el repositorio o descarga el archivo `index.html`.
2. Haz doble clic en `index.html` para abrirlo directamente en cualquier navegador moderno.

*(Opcional para desarrollo)*: Puedes levantar un servidor local rápido con `python -m http.server 8080` o `npx serve .`.

---

## 📄 Licencia

## Licencia

Copyright (c) 2026 Adolfo J. Cardozo S. [<acardozos@correo.unefm.edu.ve>]
Distribuido bajo la licencia **MIT**. Siéntete libre de usar, modificar y distribuir el código con su respectiva atribución. Ver [Licencia MIT](LICENSE) para más detalles.

---

## 👨‍💻 Autor

Desarrollado por **[Adolfo J. Cardozo S.](mailto:acardozos@correo.unefm.edu.ve)**
Profesor Universitario Jubilado e Ingeniero Civil, Consultor especializado en Computación Científica, Computer Vision e IA, e Investigador en Ingeniería Hidráulica y Transporte de Sedimentos (Nivel ScD Candidate)

> *"La simplicidad es el alma de la eficiencia."* — Austin Freeman

---
*Más proyectos y recursos en* **[acscicomp.com](https://acscicomp.com)** *(próximamente)*
