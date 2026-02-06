# Guía Visual para Extraer Imágenes de la Captura

Esta guía te ayudará a identificar y extraer cada imagen de la captura original de la página de Fundación Baobab.

## 📸 Mapa de Imágenes en la Captura

### 1. baobab-tree.svg → baobab-tree.jpg
**Ubicación**: Parte superior izquierda de la captura
**Descripción**: Árbol Baobab solitario en paisaje africano con cielo azul
**Tamaño recomendado**: 800x600px
**Uso**: Imagen principal del Hero
**Características visuales**:
- Árbol grande con tronco grueso
- Paisaje de sabana con hierba dorada
- Cielo azul claro
- Fotografía horizontal

---

### 2. students.svg → students.jpg
**Ubicación**: Sección "La fundación" - imagen izquierda
**Descripción**: Estudiantes en un aula o espacio educativo
**Tamaño recomendado**: 600x400px
**Uso**: Sección de Programas - Becas universitarias
**Características visuales**:
- Personas en interior
- Ambiente educativo
- Posiblemente con computadoras o materiales de estudio

---

### 3. baobab-junior.svg → baobab-junior.jpg
**Ubicación**: Sección "Asociación Baobab Junior"
**Descripción**: Foto grupal de miembros de Baobab Junior
**Tamaño recomendado**: 600x400px
**Uso**: Sección de Programas - Baobab Junior
**Características visuales**:
- Grupo de personas posando
- Exterior, posiblemente frente a un edificio
- Ambiente formal/semi-formal

---

### 4. establo.svg → establo.jpg
**Ubicación**: Sección "Proyectos desarrollados por la fundación"
**Descripción**: Construcción del establo
**Tamaño recomendado**: 400x300px
**Uso**: Tarjeta de proyecto destacado
**Características visuales**:
- Estructura de madera en construcción
- Posiblemente con techo de paja o similar
- Ambiente rural/agrícola

---

### 5. caci.svg → caci.jpg
**Ubicación**: Sección "La fundación" - imagen derecha
**Descripción**: Placa o letrero del centro CACI / Maison Baobab
**Tamaño recomendado**: 400x300px
**Uso**: Tarjeta de proyecto destacado
**Características visuales**:
- Placa blanca con texto
- Texto "CACI" visible
- Posiblemente "Maison Baobab" también
- Fondo de pared o edificio

---

### 6. community.svg → community.jpg
**Ubicación**: Parte central/inferior de la captura
**Descripción**: Actividades comunitarias o proyectos en terreno
**Tamaño recomendado**: 400x300px
**Uso**: Tarjeta de proyecto destacado
**Características visuales**:
- Personas en actividad comunitaria
- Posiblemente exterior
- Ambiente de trabajo colaborativo

---

### 7. foundation.svg → foundation.jpg
**Ubicación**: Cualquier imagen representativa de la fundación
**Descripción**: Imagen general que represente la fundación
**Tamaño recomendado**: 600x400px
**Uso**: Sección "La fundación" - Confianza y transparencia
**Sugerencia**: Puedes usar cualquiera de las imágenes anteriores o una combinación

---

### 8. news-1.svg → news-1.jpg
**Ubicación**: Sección "Noticias" en la parte inferior
**Descripción**: Imagen relacionada con noticias de la fundación
**Tamaño recomendado**: 600x400px
**Uso**: Sección de Noticias
**Características visuales**:
- Puede ser una imagen de actividades recientes
- Posiblemente relacionada con eventos o logros

---

## 🛠️ Proceso de Extracción

### Opción 1: Usando un editor de imágenes (Photoshop, GIMP, etc.)

1. Abre la captura en el editor
2. Usa la herramienta de selección rectangular
3. Selecciona el área de la imagen que necesitas
4. Copia y pega en un nuevo documento
5. Ajusta el tamaño según las recomendaciones
6. Guarda como JPG (calidad 80-85%) o WebP

### Opción 2: Usando herramientas online

1. **Photopea** (https://www.photopea.com/) - Editor gratuito online
2. **Squoosh** (https://squoosh.app/) - Para optimizar después de extraer

### Opción 3: Captura de pantalla selectiva

1. Abre la captura en un visor de imágenes
2. Usa herramienta de captura (Windows: Win + Shift + S)
3. Selecciona el área específica
4. Guarda con el nombre correcto

---

## 📋 Checklist de Extracción

Marca cada imagen cuando la hayas extraído y guardado:

- [ ] baobab-tree.jpg (Hero - árbol)
- [ ] students.jpg (Estudiantes en clase)
- [ ] baobab-junior.jpg (Foto grupal)
- [ ] establo.jpg (Construcción)
- [ ] caci.jpg (Placa CACI)
- [ ] community.jpg (Actividades comunitarias)
- [ ] foundation.jpg (Imagen general)
- [ ] news-1.jpg (Noticias)

---

## 🎨 Optimización de Imágenes

Después de extraer, optimiza cada imagen:

### Tamaños recomendados:
- **Hero (baobab-tree)**: 1200x800px máximo
- **Programas (students, baobab-junior)**: 800x600px
- **Proyectos (establo, caci, community)**: 600x400px
- **Otras (foundation, news)**: 800x600px

### Formato:
- **Primera opción**: WebP (mejor compresión)
- **Segunda opción**: JPG (compatibilidad universal)
- **Calidad**: 80-85%

### Herramientas de optimización:
- **Squoosh**: https://squoosh.app/
- **TinyPNG**: https://tinypng.com/
- **ImageOptim** (Mac)
- **FileOptimizer** (Windows)

---

## 🔄 Actualizar el Código

Una vez tengas las imágenes:

1. Guárdalas en `public/images/` con los nombres correctos
2. Abre `src/pages/index.astro`
3. Busca y reemplaza:
   - `.svg` → `.jpg` (o `.webp`)
4. Guarda el archivo
5. El navegador se actualizará automáticamente

### Ejemplo de cambio:

```astro
<!-- Antes -->
<img src="/images/baobab-tree.svg" alt="Árbol Baobab en África" />

<!-- Después -->
<img src="/images/baobab-tree.jpg" alt="Árbol Baobab en África" />
```

---

## ✅ Verificación Final

Después de reemplazar todas las imágenes:

1. Abre http://localhost:4322/ en tu navegador
2. Verifica que todas las imágenes cargan correctamente
3. Revisa en diferentes tamaños de pantalla (móvil, tablet, desktop)
4. Comprueba que las imágenes se ven nítidas y bien encuadradas

---

## 💡 Consejos

- **Mantén las proporciones**: No distorsiones las imágenes
- **Calidad sobre tamaño**: Es mejor una imagen un poco más pesada pero nítida
- **Nombres exactos**: Usa exactamente los nombres indicados
- **Backup**: Guarda las imágenes originales antes de optimizar
- **Prueba primero**: Prueba con una imagen antes de procesar todas

---

**¿Necesitas ayuda?**
Si tienes problemas para identificar alguna imagen, puedes:
1. Usar cualquier imagen representativa temporalmente
2. Dejar el placeholder SVG hasta conseguir la imagen real
3. Usar imágenes similares de bancos de imágenes libres (solo temporalmente)

**Recuerda**: Las imágenes reales de la fundación siempre serán mejores que stock photos.
