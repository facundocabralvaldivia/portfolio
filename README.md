# Portfolio Académico

Sitio web personal estático construido con HTML + CSS puro. Listo para desplegar en **GitHub Pages**, sin necesidad de build steps ni dependencias.

## Estructura del proyecto

```
portfolio/
├── index.html          # Home (bio, afiliaciones, recent updates)
├── research.html       # Working papers, publicaciones
├── teaching.html       # Cursos, talleres, supervisión
├── cv.html             # Currículum vitae
├── software.html       # Paquetes y proyectos open source
├── posts.html          # Blog posts y notas
├── css/
│   └── styles.css      # Estilos compartidos (paleta azul profesional)
├── assets/
│   ├── profile.svg     # Foto de perfil placeholder
│   ├── favicon.svg     # Favicon
│   └── logos/          # Logos de afiliaciones (SVG placeholder)
└── README.md
```

## Cómo personalizar

Toda la información actualmente es **ficticia**. Reemplaza el contenido en cada archivo:

1. **Datos personales** — busca y reemplaza `Nombre Apellido` en todos los `.html` por tu nombre real.
2. **Foto de perfil** — sustituye `assets/profile.svg` por tu foto (recomendado: imagen cuadrada, 400×400 px o más, formatos `.jpg`, `.png` o `.webp`). Actualiza el `src` en `index.html` si cambias el nombre del archivo.
3. **Enlaces sociales** — en el `<aside class="sidebar">` de `index.html`, actualiza:
   - `mailto:tu.email@ejemplo.com`
   - `https://github.com/tu-usuario`
   - `https://linkedin.com/in/tu-usuario`
   - `https://scholar.google.com/citations?user=ID`
4. **Logos de afiliaciones** — reemplaza los SVG en `assets/logos/` por los logos reales de tus instituciones.
5. **Contenido de cada página** — edita los archivos `.html` reemplazando el texto placeholder. La estructura de tarjetas, listas y secciones está lista para copiar/pegar.
6. **Colores** — para cambiar la paleta, edita las variables CSS al inicio de `css/styles.css`:
   ```css
   --color-accent: #1f5fb3;        /* color principal */
   --color-accent-hover: #154a8f;  /* hover */
   --color-accent-soft: #e6efff;   /* fondo suave */
   ```

## Cómo desplegar en GitHub Pages

1. Crea un repositorio en GitHub (por ejemplo `tu-usuario.github.io` o `portfolio`).
2. Sube todos los archivos de esta carpeta:
   ```bash
   git init
   git add .
   git commit -m "Initial portfolio"
   git branch -M main
   git remote add origin https://github.com/tu-usuario/tu-repo.git
   git push -u origin main
   ```
3. En GitHub: ve a **Settings → Pages → Build and deployment**.
   - Source: **Deploy from a branch**
   - Branch: **main** / carpeta **/ (root)**
4. En unos minutos tu sitio estará disponible en `https://tu-usuario.github.io/tu-repo/` (o `https://tu-usuario.github.io/` si usas el repo especial).

## Cómo previsualizar localmente

Solo necesitas abrir `index.html` en tu navegador. Para servirlo con un servidor local (recomendado para evitar errores de CORS):

```bash
# con Python
python -m http.server 8000

# o con Node
npx serve .
```

Luego visita `http://localhost:8000`.

## Tecnologías

- **HTML5** semántico
- **CSS3** con variables, Grid y Flexbox
- **Sin JavaScript** (excepto si lo añades tú)
- **SVG** para íconos y logos (escala perfectamente)
- **Responsive** — funciona en móvil, tablet y desktop

## Licencia

Eres libre de usar este template como base para tu propio portfolio. Recomendado bajo licencia MIT.
