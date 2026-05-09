# Portfolio Académico

Sitio web personal estático construido con HTML + CSS puro. Listo para desplegar en **GitHub Pages**, sin necesidad de build steps ni dependencias.

## Estructura del proyecto

```
portfolio/
├── index.html
├── research.html       # In progress
├── teaching.html
├── cv.html
├── software.html       # In progress
├── posts.html          # In progress
├── assets/
│   ├── css/
│   │   └── styles.css
│   ├── images/
│   ├── docs/
│   └── favicon.svg
└── README.md
```

## Cómo previsualizar localmente

Solo necesitas abrir `index.html` en tu navegador. Para servirlo con un servidor local (recomendado para evitar errores de CORS):

```bash
# con Python
python -m http.server 8000

# o con Node
npx serve .
```

Luego visita `http://localhost:8000`.
