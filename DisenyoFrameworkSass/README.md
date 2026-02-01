## Descripción
MySassFramework es un **framework CSS modular y ligero** desarrollado con **Sass**, diseñado para crear interfaces web coherentes y responsive sin depender de librerías externas.  
Permite construir layouts y componentes reutilizables de manera escalable y mantenible, con un sistema de variables, mixins, funciones y utilidades automatizadas.

## Características principales

- **Sistema de diseño**
  - Paleta de colores semántica (`primary`, `secondary`, `success`, `danger`, `warning`) mediante mapas Sass.
  - Sistema tipográfico con escala modular automatizada (`$font-base-size`, `$font-scale-ratio`).
  - Variables de espaciado (`xs, sm, md, lg, xl`).
  - Bordes, sombras y z-index predefinidos.
  - Mixins para media queries, flexbox, grid, botones y estados (`hover`, `focus`, `disabled`).
  - Funciones para conversión `px → rem`, contraste de colores y escalas tipográficas.

- **Layout responsive**
  - Sistema de grid con clases generadas automáticamente (`col-6-md`, `col-4-lg`).
  - Uso de bucles Sass (`@for`, `@each`) y condicionales (`@if`) para generar clases dinámicas.
  
- **Componentes reutilizables**
  - Botones con variantes y estados.
  - Cards.
  - Formularios.
  - Navbar responsive.
  - Alertas y badges.
  - Todos los componentes usan variables, son responsive y siguen la metodología BEM.

- **Temas**
  - Dos temas: **claro** y **oscuro**.
  - Definidos con variables CSS y mapas Sass, para fácil cambio de apariencia.

- **Utilidades automáticas**
  - Márgenes y paddings (`.m-sm`, `.pt-lg`, `.px-md`).
  - Colores de texto y fondo (`.text-primary`, `.bg-danger`).
  - Display, flexbox y alineación (`.d-flex`, `.justify-center`, `.align-end`).

## Estructura del proyecto
framework/
├─ sass/
│  ├─ abstract/
│  │  ├─ _variables.scss
│  │  ├─ _maps.scss
│  │  ├─ _functions.scss
│  │  └─ _mixins.scss
│  ├─ base/
│  │  ├─ _reset.scss
│  │  └─ _typography.scss
│  ├─ layout/
│  │  ├─ _grid.scss
│  │  ├─ _header.scss
│  │  └─ _footer.scss
│  ├─ components/
│  │  ├─ _buttons.scss
│  │  ├─ _cards.scss
│  │  └─ _forms.scss
│  ├─ themes/
│  │  ├─ _light.scss
│  │  └─ _dark.scss
│  ├─ utilities/
│  │  ├─ _spacing.scss
│  │  ├─ _color.scss
│  │  └─ _layout.scss
│  └─ main.scss
├─ dist/
│  └─ framework.css
└─ README.md
