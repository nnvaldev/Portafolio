# Portafolio — Alexander Castillo (`@nvaldev`)

Portafolio personal de **Alexander Nataniel Castillo Centellas**, _Fullstack & Cloud Engineer · DevOps · UI/UX Designer_ de La Paz, Bolivia.

Sitio de una sola página construido con **Astro + Tailwind CSS**, con tema claro/oscuro, animaciones al hacer scroll y un diseño responsive pensado para destacar experiencia y proyectos.

## ✨ Características

- 🌗 **Tema claro / oscuro** con persistencia en `localStorage` y sin parpadeo en la carga inicial.
- 🎬 **Hero animado** (grid + blobs, anillo giratorio, efecto _typing_) para captar la atención.
- 📱 **Responsive**: sidebar en desktop y menú overlay en móvil.
- 🧩 Secciones: Proyectos (con modal de detalle), Experiencia, Habilidades, Formación, Sobre mí y Contacto.
- ⚡ Detalles de UX: barra de progreso de scroll, spotlight que sigue el cursor, tilt 3D en las tarjetas y animaciones respetuosas con `prefers-reduced-motion`.

## 🛠️ Stack

- [Astro](https://astro.build) `^5`
- [Tailwind CSS](https://tailwindcss.com) `^3` (`darkMode: 'class'`)
- [JetBrains Mono](https://www.jetbrains.com/lp/mono/) (`@fontsource-variable`)

## 🚀 Estructura del proyecto

```text
/
├── public/                 # Assets estáticos (favicon, capturas, cv_es.pdf)
├── src/
│   ├── assets/             # Imágenes procesadas por Astro (foto de perfil, svg)
│   ├── components/         # Componentes .astro (Header, Project, Experience, …)
│   │   └── icons/          # Íconos SVG como componentes
│   ├── layouts/
│   │   └── Layout.astro    # Layout base: temas, estilos globales, scripts
│   └── pages/
│       └── index.astro     # Página principal
├── astro.config.mjs
├── tailwind.config.mjs
└── package.json
```

## 🧞 Comandos

Todos los comandos se ejecutan desde la raíz del proyecto:

| Comando             | Acción                                            |
| :------------------ | :------------------------------------------------ |
| `npm install`       | Instala las dependencias                          |
| `npm run dev`       | Servidor de desarrollo en `localhost:4321`        |
| `npm run build`     | Compila el sitio de producción en `./dist/`       |
| `npm run preview`   | Previsualiza el build localmente                  |

## 🎨 Personalización rápida

- **Tema y colores**: variables CSS en el `<style is:global>` de `src/layouts/Layout.astro` (`:root` para claro, `html.dark` para oscuro).
- **Experiencia / Proyectos / Formación**: editar los arreglos de datos en `src/components/Experience.astro`, `Project.astro` y `Formation.astro`.
- **Foto de perfil**: `src/assets/profile photo.jpg` (importada en `src/pages/index.astro`).

## 📫 Contacto

- ✉️ [nnvaldev@gmail.com](mailto:nnvaldev@gmail.com)
- 💼 [linkedin.com/in/nvaldev](https://www.linkedin.com/in/nvaldev/)
- 🐙 [github.com/nnvaldev](https://github.com/nnvaldev)
