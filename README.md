# 🛏️ Nube Nueve — Colchones de Ensueño

Sitio web de una marca de colchones premium, desarrollado con HTML, CSS y JavaScript puro.

🌐 **Despliegue en GitHub Pages:** https://villarod97.github.io/product-lading-page/

---

## 📁 Estructura del proyecto
nube-nueve/
├── index.html
├── precios.html
├── faq.html
├── script.js
├── css/
│   └── styles.css
└── img/
├── imghero.jpg
├── imagen-1.jpg
├── imagen-2.jpg
├── imagen-3.jpg
├── imagen-4.jpg
├── facebook.svg
├── instagram2.svg
├── linkedin.svg
├── youtube.svg
├── tiktok.svg
├── icono-1.svg
├── icono-2.svg
├── icono-3.svg
├── icono-4.svg
├── faq.svg
└── colchon-de-aire.ico

---

## ✨ Funcionalidades

- **Modo oscuro/claro** — toggle con JavaScript que cambia el atributo `data-theme` en `<html>`.
- **Navegación sticky** — el header se mantiene visible al hacer scroll.
- **Galería de imágenes** — con descripciones usando `<figure>` y `<figcaption>`.
- **Sección de Testimonios** — tarjetas en Flexbox responsivo.
- **FAQ interactivo** — usando `<details>` y `<summary>` nativos de HTML, con página dedicada (`faq.html`) en layout de dos columnas.
- **Página de Precios** — cinco planes en CSS Grid responsivo con badge "Más popular".
- **Formulario de contacto** — con validación nativa HTML5 y estilos de feedback visual.
- **Footer con redes sociales** — íconos SVG con filtro de color y enlaces legales.

---

## 🎨 Decisiones de diseño

- **Tipografía:** Georgia (cuerpo) + Helvetica Neue (UI y etiquetas).
- **Paleta:** tonos neutros cálidos con acento púrpura (`#6d4bb5`) en modo claro y azul suave (`#8aaed4`) en modo oscuro.
- **Responsive:** Mobile first con breakpoints en 640px (tablet) y 1024px (escritorio).
- **Microinteracciones:** `transform` + `transition` en hover de tarjetas, galería, botones e iconos sociales.

---

## 🎨 Tokens CSS (Custom Properties)

| Token | Valor (modo claro) | Valor (modo oscuro) | Dónde se usa |
|---|---|---|---|
| `--bg-color` | `#f5f3ee` | `#111214` | Fondo general del `body` |
| `--text-color` | `#1c1c1c` | `#e8e5de` | Texto principal, inputs, labels con checkbox |
| `--surface` | `#ffffff` | `#1e2025` | Fondo de tarjetas, inputs, details, testimonios |
| `--surface-border` | `rgba(0,0,0,0.10)` | `rgba(255,255,255,0.10)` | Bordes de tarjetas, inputs, separadores |
| `--nav-bg` | `#1c1c1c` | `#0a0b0d` | Fondo del `header` y `footer` |
| `--nav-text` | `#f5f3ee` | `#e8e5de` | Texto y links del nav y footer |
| `--accent` | `#6d4bb5` | `#8aaed4` | Botones, íconos ✦, bordes en hover, precios, badge |
| `--accent-hover` | `#4e3282` | `#aecbe8` | Hover del botón submit y botones de planes |
| `--muted` | `#6b6860` | `#9a9790` | Labels, textos secundarios, figcaption, autores |
| `--link-color` | `#5b6e8c` | `#8aaed4` | Enlaces dentro de `<main>` |
| `--link-hover` | `#3d4f68` | `#aecbe8` | Hover de enlaces dentro de `<main>` |
| `--transition` | `0.3s cubic-bezier(0.4,0,0.2,1)` | _(igual)_ | Transición global de tema (bg, color, border) |

---

## ✅ Validaciones del formulario

| Campo | Atributo(s) | Error nativo que muestra el navegador |
|---|---|---|
| Nombre | `required`, `minlength="3"` | "Completa este campo" si está vacío; "Usa al menos 3 caracteres" si es muy corto |
| Correo electrónico | `required`, `type="email"` | "Completa este campo" si está vacío; "Incluye un signo '@'" si el formato es inválido |
| Teléfono | `required`, `type="tel"`, `pattern="^(?:\+51\s?)?9(?:\s?\d){8}$"` | "Completa este campo" si está vacío; "Coincide con el formato solicitado" si no cumple el patrón peruano |
| Motivo del contacto | `required` | "Selecciona un elemento de la lista" si no se elige ninguna opción |
| Mensaje | `required`, `minlength="10"` | "Completa este campo" si está vacío; "Usa al menos 10 caracteres" si es muy corto |
| Términos y condiciones | `required`, `type="checkbox"` | "Marca esta casilla si quieres continuar" si no está marcado |

---

## 🛠️ Tecnologías

- HTML5 semántico
- CSS3 (Flexbox, Grid, Custom Properties, Media Queries)
- JavaScript vanilla

---

## 🚀 Cómo usar

1. Clona o descarga el repositorio.
2. Abre `index.html` en tu navegador (o usa Live Server en VS Code).
3. No requiere instalación ni dependencias.

---

## ✅ Validación y pruebas

- HTML validado en [W3C Validator](https://validator.w3.org/)
- Probado en Chrome, Firefox y Safari
- Revisado en DevTools modo responsive
