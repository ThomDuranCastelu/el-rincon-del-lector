# El Rincón del Lector

Sitio web de una librería, desarrollado como proyecto integrador del curso de Programación Web (Coderhouse).

## 🔗 Links

- **Sitio desplegado:** [https://thomdurancastelu.github.io/el-rincon-del-lector/](https://thomdurancastelu.github.io/el-rincon-del-lector/)
- **Repositorio:** [https://github.com/ThomDuranCastelu/el-rincon-del-lector](https://github.com/ThomDuranCastelu/el-rincon-del-lector)

## 📄 Páginas

- `index.html` — Portada de bienvenida
- `pages/inicio.html` — Home con catálogo resumido
- `pages/sobre-nosotros.html` — Historia, misión y visión de la librería
- `pages/catalogo.html` — Catálogo completo de libros por género
- `pages/contacto.html` — Formulario de contacto

## 🛠️ Tecnologías

- HTML5 semántico
- SCSS (variables, mixins, nesting, partials) compilado a CSS
- CSS3 (Flexbox, Grid, media queries)
- [Bootstrap 5](https://getbootstrap.com/) (navbar responsiva y carousel)
- Google Fonts (Lobster Two + Lora)

## ✨ Funcionalidades

- Diseño mobile-first, responsivo en mobile / tablet / desktop
- Navbar de Bootstrap con menú hamburguesa en mobile
- Carousel de imágenes en `index.html` y `catalogo.html`
- Layout con CSS Grid (`grid-template-areas`) en las secciones principales
- Estados interactivos (`:hover`, `:focus`, `:active`) en links, botones y tarjetas
- Paleta de colores y tipografía propias, aplicadas sobre los componentes de Bootstrap
- Arquitectura SCSS modular (variables, mixins y partials organizados por `base/`, `layout/` y `components/`)

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