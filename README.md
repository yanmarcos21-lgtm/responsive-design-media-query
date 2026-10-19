# Practical Time – Tarjetas de perfil responsive

Ejercicio práctico: construcción de tarjetas de perfil con diseño responsive, metodología **BEM**, la propiedad CSS **clip-path** y **Font Awesome** por CDN.

**Integrantes (tarjetas):** Antonio Obregon y Nancy Mina

- Repositorio base: <https://github.com/uniajc-gperezm/responsive-design-media-query>
- Demo (GitHub Pages): `https://TU-USUARIO.github.io/NOMBRE-DEL-REPO/`

## Estructura

```
responsive-cards/
├── css/
│   └── styles.css
├── index.html
└── README.md
```

## Tecnologías

- HTML5 semántico (`main`, `section`, `article`, `header`, `footer`)
- CSS3 con variables, Flexbox y media queries (mobile first)
- `clip-path` para el encabezado curvo/inclinado y el pie con muesca/inclinación
- Font Awesome 7.3.1 por CDN:
  `https://cdnjs.cloudflare.com/ajax/libs/font-awesome/7.3.1/css/all.min.css`

## Metodología BEM

BEM (Block, Element, Modifier) nombra las clases según su función para que el CSS sea predecible y reutilizable.

- **Block:** componente independiente → `profile-card`
- **Element:** parte del bloque → `profile-card__header`, `profile-card__avatar`, `profile-card__name`, `profile-card__footer`
- **Modifier:** variación → `profile-card--wave` (curva) y `profile-card--slant` (inclinada)

## Diseño responsive

| Ancho de pantalla | Comportamiento |
|---|---|
| Menos de 640px | Tarjetas apiladas en una columna |
| 640px o más | Tarjetas lado a lado |
| 1024px o más | Tarjetas más grandes y mayor separación |

## Cómo publicar con GitHub Pages

1. Crea un repositorio público en tu cuenta de GitHub y sube `index.html`, `README.md` y la carpeta `css`.
2. Ve a **Settings → Pages**.
3. En **Source**, elige **Deploy from a branch**, rama `main`, carpeta `/ (root)`, y guarda.
4. Espera 1–2 minutos y abre la URL que GitHub te muestre. Pégala en este README y en la entrega de Teams.

## Cómo usar fotos reales

Reemplaza el `div.profile-card__avatar` por una imagen:

```html
<img class="profile-card__photo" src="img/antonio.jpg" alt="Antonio Obregon">
```

## Recursos

- Generador de clip-path: <https://clippy.f8.edu.vn/>
- Guía BEM: <https://getbem.com/introduction/>
