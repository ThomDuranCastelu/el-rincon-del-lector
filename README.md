# El Rincón del Lector

Sitio web de una librería, desarrollado como proyecto integrador del curso de Programación Web (Coderhouse).

## 🔗 Links

- **Sitio desplegado (Netlify):** [https://el-rincon-del-lector-coderhouse.netlify.app](https://el-rincon-del-lector-coderhouse.netlify.app)
- **Sitio desplegado (GitHub Pages):** [https://thomdurancastelu.github.io/el-rincon-del-lector/](https://thomdurancastelu.github.io/el-rincon-del-lector/)
- **Repositorio:** [https://github.com/ThomDuranCastelu/el-rincon-del-lector](https://github.com/ThomDuranCastelu/el-rincon-del-lector)

## 📄 Páginas

- `index.html` — Portada de bienvenida
- `pages/inicio.html` — Home con catálogo resumido
- `pages/sobre-nosotros.html` — Historia, misión y visión de la librería
- `pages/catalogo.html` — Catálogo completo de libros por género
- `pages/contacto.html` — Formulario de contacto

## 🛠️ Tecnologías

- HTML5 semántico
- SCSS (variables, mixins con parámetros, nesting, `@extend`, partials) compilado a CSS
- CSS3 (Flexbox, Grid, media queries, `@keyframes`)
- [Bootstrap 5](https://getbootstrap.com/) (navbar responsiva y carousel)
- [AOS](https://michalsnik.github.io/aos/) (Animate On Scroll)
- Google Fonts (Lobster Two + Lora)
- Desplegado en Netlify

## ✨ Funcionalidades

- Diseño mobile-first, 100% responsivo en mobile / tablet / desktop (breakpoint en 1024px)
- Navbar de Bootstrap con menú hamburguesa en mobile, estilada con la paleta propia
- Carousel de imágenes en `index.html` y `catalogo.html`
- Layout con CSS Grid (`grid-template-areas`) en las 5 páginas
- Animaciones nativas con `@keyframes` (aparición del título, logo flotante) y estados interactivos (`:hover`, `:focus`, `:active`) con `transition`
- Animaciones al hacer scroll con la librería AOS
- Arquitectura SCSS modular (variables, mixins con parámetros, `@extend`, partials organizados por `base/`, `layout/` y `components/`)
- SEO on-page: `title`, `meta description` y `meta keywords` únicos por página, `alt` descriptivo en todas las imágenes

## 📁 Estructura del proyecto

```
el-rincon-del-lector/
├── index.html
├── pages/
│   ├── inicio.html
│   ├── sobre-nosotros.html
│   ├── catalogo.html
│   └── contacto.html
├── scss/
│   ├── main.scss          # único punto de entrada (@use)
│   ├── utilities/
│   │   ├── _variables.scss
│   │   └── _mixins.scss
│   ├── base/
│   │   ├── _tipografia.scss
│   │   └── _base.scss
│   ├── layout/
│   │   ├── _header.scss
│   │   ├── _nav.scss
│   │   ├── _footer.scss
│   │   └── _grid.scss
│   └── components/
│       ├── _cards.scss
│       ├── _buttons.scss
│       ├── _forms.scss
│       ├── _carousel.scss
│       └── _misc.scss
├── styles/
│   └── main.css            # generado por la compilación de SCSS
└── assets/
    ├── libros/
    └── (logo e imágenes generales)
```