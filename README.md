# Resdat — Landing corporativa

Sitio estático para **soluciones digitales B2B** ([resdat.es](https://www.resdat.es/)). Genera HTML/CSS en el build; ideal para alojamiento estático o CDN.

## Tecnologías

| Área | Tecnología |
|------|------------|
| **Framework** | [Astro](https://astro.build/) 6.x — páginas y componentes en `.astro`, salida estática (`output: static`). |
| **Estilos** | [Tailwind CSS](https://tailwindcss.com/) 4.x integrado con el plugin oficial para Vite: [`@tailwindcss/vite`](https://tailwindcss.com/docs/installation/using-vite). |
| **Bundler / dev server** | [Vite](https://vitejs.dev/) (incluido con Astro). |
| **Entorno de ejecución** | [Node.js](https://nodejs.org/) ≥ 22.12 (según `package.json`). |
| **Gestor de paquetes** | [pnpm](https://pnpm.io/) (hay `pnpm-lock.yaml` en el repo). |
| **Tipografía** | [Montserrat](https://fonts.google.com/specimen/Montserrat) vía Google Fonts. |
| **Formulario de contacto** | [Formspree](https://formspree.io/) (endpoint configurado en la página de contacto). |
| **Control de versiones** | Git — ver `.gitignore` para artefactos locales (`node_modules`, `dist`, `.env`, etc.). |

## Scripts

```bash
pnpm install    # dependencias
pnpm dev        # servidor de desarrollo
pnpm build      # genera la carpeta dist/
pnpm preview    # vista previa del build de producción
```

## Estructura principal

- `src/pages/` — rutas (p. ej. `index.astro`).
- `src/layouts/` — plantilla HTML base y metadatos.
- `src/styles/global.css` — entrada de Tailwind y tokens de tema (colores de marca).
- `src/assets/` — imágenes, favicon, logo SVG.
- `public/` — archivos servidos tal cual (p. ej. `favicon.svg`).

## Licencia / marca

Contenido y marca **Resdat**. Ajusta enlaces legales y datos de contacto según tu despliegue.
