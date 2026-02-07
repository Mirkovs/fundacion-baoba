# Fundación BAOBAB - Sitio Web

Proyecto Astro mobile-first para la Fundación BAOBAB de cooperación y ayuda al desarrollo.

## 🚀 Inicio rápido

El servidor de desarrollo ya está corriendo en:
- **URL local**: http://localhost:4322/

Abre esta URL en tu navegador para ver el sitio.

## � Características

### Diseño Mobile-First
- Responsive design optimizado para móviles primero
- Menú hamburguesa funcional en dispositivos móviles
- Navegación horizontal en desktop
- Breakpoints: 640px, 768px

### Secciones implementadas

1. **Hero** - Mensaje principal con CTA
2. **Qué hacemos** - 3 bloques de características
3. **Impacto** - Estadísticas de la fundación
4. **Programas** - Becas universitarias y Baobab Junior
5. **Proyectos destacados** - 3 proyectos principales
6. **Noticias** - Últimas actualizaciones
7. **Cómo ayudar** - Voluntariado, cursos y donaciones
8. **Confianza y transparencia** - Historia, valores y recursos
9. **FAQ** - Preguntas frecuentes
10. **CTA final + Contacto** - Información de contacto

### SEO y Accesibilidad
- ✅ Un solo H1 por página
- ✅ HTML semántico
- ✅ Metadatos completos
- ✅ Navegación por teclado
- ✅ ARIA labels en elementos interactivos

## 🎨 Diseño

### Paleta de colores
- **Primary**: #1a8754 (Verde Baobab)
- **Primary Dark**: #156b43
- **Primary Light**: #22a566
- **Text**: #2c3e50
- **Background**: #ffffff

### Tipografía
- Sistema de fuentes nativas para mejor rendimiento
- Escala tipográfica responsive
- Line-height optimizado para legibilidad

## 📁 Estructura del proyecto

```
/
├── public/
│   ├── images/          # Imágenes (actualmente placeholders SVG)
│   └── favicon.svg
├── src/
│   ├── components/
│   │   ├── Header.astro
│   │   ├── Footer.astro
│   │   ├── Button.astro
│   │   ├── FeatureCard.astro
│   │   └── ProjectCard.astro
│   ├── layouts/
│   │   └── BaseLayout.astro
│   └── pages/
│       └── index.astro
└── package.json
```

## 🖼️ Imágenes

**IMPORTANTE**: Actualmente el sitio usa placeholders SVG temporales.

### Imágenes que deben reemplazarse:

Todas las imágenes están en `public/images/` y deben extraerse de la captura original:

1. **baobab-tree.svg** → Árbol Baobab (parte superior izquierda de la captura)
2. **students.svg** → Estudiantes becados (sección "La fundación")
3. **baobab-junior.svg** → Grupo Baobab Junior (foto grupal)
4. **establo.svg** → Construcción del establo (proyectos)
5. **caci.svg** → Placa del centro CACI
6. **community.svg** → Proyectos comunitarios
7. **foundation.svg** → Imagen general de la fundación
8. **news-1.svg** → Imagen de noticias

### Cómo reemplazar las imágenes:

1. Extrae las imágenes de la captura original
2. Guárdalas como JPG o WebP con los mismos nombres (cambiando .svg por .jpg)
3. Actualiza las referencias en `src/pages/index.astro`

Ver `public/images/README.md` para más detalles.

## 🛠️ Comandos disponibles

```bash
# Desarrollo (ya corriendo)
npm run dev

# Build para producción
npm run build

# Preview del build
npm run preview

# Detener el servidor
Ctrl + C
```

## 📝 Contenido

Todo el contenido proviene del texto proporcionado de la página original:

- **Historia**: Fundación creada en septiembre de 2009
- **Experiencia**: Más de 12 años
- **Misión**: Becas universitarias en África subsahariana
- **Baobab Junior**: Asociación de antiguos becarios
- **Donaciones**: 450€/año, desgravables según Ley 49/2002
- **Contacto**: info@fundacionbaobab.com, Calle Andorra 2, Granada

## 🎯 Próximos pasos

1. **Reemplazar imágenes placeholder** con las reales de la captura
2. **Revisar contenido** y ajustar textos si es necesario
3. **Añadir más páginas** (Quiénes somos, Recursos, etc.)
4. **Optimizar imágenes** para web (WebP, lazy loading)
5. **Configurar deployment** (Netlify, Vercel, GitHub Pages)

## 📱 Testing

Prueba el sitio en diferentes dispositivos:
- Móvil: < 640px
- Tablet: 640px - 768px
- Desktop: > 768px

Verifica:
- ✅ Menú hamburguesa funciona en móvil
- ✅ Navegación smooth scroll
- ✅ Todos los enlaces funcionan
- ✅ Formularios de contacto (cuando se implementen)
- ✅ Imágenes cargan correctamente

## 🛠️ Convenciones de Desarrollo

### Enlaces y Assets (IMPORTANTE)
Para asegurar que el sitio funcione en GitHub Pages (específicamente en un subdirectorio como `/fundacion-baoba/`), **todos** los enlaces internos y rutas de recursos deben usar la base dinámica:

- **Enlaces**: `href={`${import.meta.env.BASE_URL}pagina/`}`
- **Imágenes**: `src={`${import.meta.env.BASE_URL}images/foto.jpg`}`
- **Archivos**: `href={`${import.meta.env.BASE_URL}files/doc.pdf`}`

**Nunca usar rutas relativas puras** como `href="proyectos/"` ya que causan errores de anidamiento al navegar desde subpáginas.

## 🌐 Deployment

Para desplegar en producción:

```bash
# Build
npm run build

# El output estará en dist/
# Sube dist/ a tu hosting preferido
```

Opciones recomendadas:
- **Netlify**: Drag & drop de la carpeta dist/
- **Vercel**: Conectar repositorio Git
- **GitHub Pages**: Configurar astro.config.mjs

## 📄 Licencia

Fundación BAOBAB © 2026

---

**Desarrollado con**: Astro + TypeScript
**Diseño**: Mobile-first, responsive
**Estado**: ✅ Home completa, imágenes pendientes
