# 🏗️ SteelBuild — Landing Page

Landing page de alto impacto para empresa constructora especializada en **Steel Framing** y **aislamientos termoacústicos proyectados**.

![Preview](https://img.shields.io/badge/Estado-Producción%20Ready-brightgreen)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/TailwindCSS-38B2AC?logo=tailwind-css&logoColor=white)
![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-Listo-blue)

---

## 🚀 Demo en vivo

> Publicar en GitHub Pages: `https://tu-usuario.github.io/steelbuild-landing`

---

## 📋 Secciones incluidas

| Sección | Descripción |
|---|---|
| 🦸 **Hero** | Título impactante + estadísticas + CTA principal |
| 🔧 **Proceso Constructivo** | 3 etapas: Estructura → Aislamiento → Acabado EIFS |
| ⚡ **Beneficios Técnicos** | Grilla de 4 + 3 beneficios con iconos SVG |
| 📸 **Galería de Obra** | Mockup de 6 fotos con placeholders reemplazables |
| 🏆 **Nosotros / Trust** | Stats, testimonial, diferenciadores |
| 📊 **Comparativa** | Steel Framing vs. Construcción tradicional |
| 📩 **Formulario de Contacto** | Validado con radio buttons, select y éxito visual |
| 📍 **Footer** | Completo con redes, contacto y links |
| 💬 **WhatsApp flotante** | Botón de contacto rápido siempre visible |

---

## 🎨 Sistema de diseño

### Paleta de colores

| Token | Hex | Uso |
|---|---|---|
| `accent` | `#e85d04` | CTAs, highlights, progreso |
| `sand-400` | `#d4a654` | Textos secundarios cálidos |
| `sand-600` | `#a97530` | Encabezados cálidos |
| `steel-800` | `#37414b` | Texto principal |
| `steel-900` | `#313940` | Fondos oscuros |

### Tipografía
- **Inter** (Google Fonts) — Sans-serif moderna, pesos 300–900

---

## 📁 Estructura del proyecto

```
steelbuild-landing/
│
├── index.html          # Archivo principal (todo-en-uno)
├── README.md           # Este archivo
│
└── img/                # (Crear esta carpeta)
    └── gallery/
        ├── foto-1.jpg  # Acabado exterior final
        ├── foto-2.jpg  # Estructura Steel Framing nocturna
        ├── foto-3.jpg  # Aislamiento proyectado en techo
        ├── foto-4.jpg  # Revoque base (EIFS)
        ├── foto-5.jpg  # Aislamiento proyectado en paredes
        └── foto-6.jpg  # Interior terminado
```

---

## 🖼️ Cómo agregar las fotos reales

Los placeholders de la galería están diseñados para ser reemplazados fácilmente.

### Opción A — Reemplazar los div placeholder con `<img>`:

Encontrá cada bloque de galería y reemplazá el `<div>` interno por:

```html
<img 
  src="img/gallery/foto-1.jpg" 
  alt="Acabado exterior Steel Framing" 
  class="w-full h-full object-cover"
/>
```

### Opción B — Usar como background CSS:

```html
<div class="w-full h-full" style="background-image: url('img/gallery/foto-1.jpg'); background-size: cover; background-position: center;">
```

---

## 📦 Publicar en GitHub Pages

### Paso 1: Crear repositorio
```bash
git init
git add .
git commit -m "feat: landing page steelbuild"
git remote add origin https://github.com/TU-USUARIO/steelbuild-landing.git
git push -u origin main
```

### Paso 2: Activar GitHub Pages
1. Ir a **Settings** del repositorio
2. Sección **Pages** → Source: **Deploy from a branch**
3. Branch: `main` / Folder: `/ (root)`
4. Guardar → en 1–2 minutos estará disponible en:
   `https://TU-USUARIO.github.io/steelbuild-landing`

---

## ✏️ Personalización rápida

### Cambiar nombre de empresa
Buscar y reemplazar `SteelBuild` y `steelbuild` en el HTML.

### Cambiar datos de contacto
Buscar:
```
+54 (387) XXX-XXXX
info@steelbuild.com.ar
https://wa.me/543870000000
```
Y reemplazar por los datos reales del cliente.

### Cambiar zona de operación
Buscar: `Salta, NOA y región` y actualizar.

### Cambiar estadísticas
En la sección Hero, buscar los bloques con clase `stat-number` y actualizar los valores.

### Cambiar color de acento
En el `<script>` de Tailwind config, cambiar:
```js
accent: '#e85d04',  // → color deseado
```

---

## 📬 Integrar el formulario

El formulario actualmente tiene un mock de envío (setTimeout). Para activarlo con envío real:

### Opción 1 — Formspree (gratis hasta 50 envíos/mes)
```html
<form action="https://formspree.io/f/TU-ID" method="POST">
```
Registrarse en [formspree.io](https://formspree.io)

### Opción 2 — EmailJS (JS puro, sin backend)
```html
<script src="https://cdn.jsdelivr.net/npm/@emailjs/browser@4/dist/email.min.js"></script>
```
Registrarse en [emailjs.com](https://www.emailjs.com)

### Opción 3 — Google Forms (embed)
Reemplazar el formulario por el iframe de Google Forms.

---

## ✅ Checklist de lanzamiento

- [ ] Reemplazar fotos de la galería con imágenes reales
- [ ] Actualizar teléfono, email y link de WhatsApp
- [ ] Actualizar nombre real de la empresa
- [ ] Conectar formulario (Formspree / EmailJS)
- [ ] Actualizar estadísticas reales (obras, años, etc.)
- [ ] Agregar el favicon (`<link rel="icon">`)
- [ ] Configurar Google Analytics o similar
- [ ] Probar en móvil (Chrome DevTools)
- [ ] Publicar en GitHub Pages o hosting propio

---

## 🛠️ Tecnologías

- **HTML5** — estructura semántica
- **Tailwind CSS v3** — via CDN, sin build step
- **SVG inline** — iconos sin dependencias
- **JavaScript vanilla** — sin frameworks, ultraliviano
- **Google Fonts** — Inter

---

## 📄 Licencia

Proyecto desarrollado para uso exclusivo del cliente. No redistribuir sin autorización.

---

*Desarrollado por [Tu Nombre / Agencia]* • *Matias — UX/UI & Digital Transformation Consultant*
