# Instrucciones para el Agente - Proyecto Fundación Baobab

Este archivo contiene las directrices específicas para el desarrollo y mantenimiento del sitio web de la Fundación Baobab.

## 🛠️ Stack Tecnológico
- **Framework**: Astro 5.x
- **Lenguaje**: TypeScript (Modo estricto)
- **Estilos**: CSS puro (vía variables globales en `BaseLayout.astro`)
- **Componentes**: Astro (Server-first)

## 🎨 Principios de Diseño
- **Mobile-first**: Todos los desarrollos deben priorizar la experiencia en móviles.
- **Estética**: Sobria, humana y transparente.
- **Colores**: Uso predominante del Verde Baobab (#1a8754) y tonos tierra.
- **Tipografía**: Fuentes de sistema para máximo rendimiento y legibilidad.

## 📄 Estructura de Contenido
- **Home**: Landing page sintética y puerta de entrada.
- **Transparencia**: Historia, valores y equipo.
- **Proyectos**: Catálogo de impacto e infraestructura.
- **Baobab Junior**: Espacio para la asociación de egresados.
- **Colaborar**: Foco en conversiones (Donaciones, formularios, voluntariado).
- **Noticias/Recursos**: Actualidad y documentos técnicos.

## ⚖️ Normas del Agente
1. **Fidelidad al texto**: Usar siempre el contenido proporcionado por el usuario (no inventar datos).
2. **Transparencia**: Mantener siempre visibles las políticas de cookies y privacidad.
3. **Optimización**: Preferir SVGs para iconos y WebP para imágenes reales.
4. **Accesibilidad**: Mantener un marcado HTML semántico y atributos ARIA necesarios.
5. **SEO**: Un solo H1 por página y meta-etiquetas descriptivas.

## 📂 Gestión de Archivos y Rutas
- **Rutas Internas**: ABSOLUTAMENTE TODOS los enlaces (`href`) e imágenes (`src`) internos deben usar `${import.meta.env.BASE_URL}` para asegurar compatibilidad con subdirectorios de GitHub Pages.
  - Ejemplo: `<a href={`${import.meta.env.BASE_URL}proyectos/`}>`
- **Imágenes**: Deben ir en `public/images/`. Referenciarlas siempre como `${import.meta.env.BASE_URL}images/nombre.ext`.
- **Documentos**: Los documentos oficiales en `public/files/`. Referenciarlos como `${import.meta.env.BASE_URL}files/nombre.pdf`.
- **Componentes**: Los componentes reutilizables en `src/components/`.
- **Layout**: El layout global es `src/layouts/BaseLayout.astro`.

## 🔗 Enrutamiento
1. **Trailing Slashes**: Usar siempre el slash final en las URLs (`/página/`) tal como está configurado en `astro.config.mjs`.
2. **Evitar enlaces relativos sucios**: Nunca usar `href="proyectos/"` o `href="./"`. Usar siempre la base dinámica para evitar anidamientos incorrectos (como `/proyectos/recursos/`).
3. **Favicon**: Referenciar el favicon en el layout usando la base: `${import.meta.env.BASE_URL}favicon.svg`.

