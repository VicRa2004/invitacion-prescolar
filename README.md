# 🎓 Invitación Digital - Ceremonia de Graduación 2023 - 2026

¡Bienvenido al proyecto de la invitación digital interactiva! Esta aplicación ha sido diseñada especialmente para la ceremonia de graduación en coordinación del **Centro Preescolar Indígena "Coronel Gregorio Mendez"** y el **Centro de Educación Inicial "La Flor del maiz"** en Jolochero, Centro, Tabasco.

El proyecto está desarrollado utilizando **[Astro](https://astro.build/)** y estilizado con **[Tailwind CSS v4](https://tailwindcss.com/)** para brindar una experiencia interactiva, rápida y responsiva.

---

## 🛠️ Requisitos Previos

Antes de ejecutar este proyecto, asegúrate de tener instalado en tu computadora:

- [Node.js](https://nodejs.org/) (versión 18 o superior recomendada)
- Un gestor de paquetes. El proyecto incluye un archivo de bloqueo de **pnpm** (`pnpm-lock.yaml`), por lo que te recomendamos usarlo. Si no lo tienes instalado globalmente, puedes habilitarlo con:
  ```bash
  corepack enable
  ```
  *(O usar `npm` como alternativa).*

---

## 🚀 Pasos para Ejecutar el Proyecto

Sigue estos sencillos pasos para levantar el entorno local:

### 1. Clonar o acceder a la carpeta del proyecto
Abre tu terminal favorita y entra al directorio donde se encuentra este proyecto:
```bash
cd invitacion-prescolar
```

### 2. Instalar las dependencias
Instala todas las librerías necesarias del proyecto ejecutando:
```bash
pnpm install
```
*(Si prefieres usar npm, ejecuta: `npm install`)*

### 3. Iniciar el servidor de desarrollo
Para encender el servidor de desarrollo y visualizar el sitio web de forma interactiva y en tiempo real, ejecuta:
```bash
pnpm run dev
```
*(O `npm run dev`)*

Una vez iniciado, abre tu navegador e ingresa a la dirección local que se muestra en la terminal, que típicamente es:
👉 **[http://localhost:4321/](http://localhost:4321/)**

Cualquier cambio que realices en el código se reflejará instantáneamente en el navegador gracias al Hot Module Replacement (HMR).

---

## 📦 Compilación para Producción

Si deseas compilar la web en archivos HTML, CSS y JS estáticos listos para ser distribuidos o subidos a un hosting (como Netlify, Vercel, Cloudflare Pages, etc.):

1. **Construir el sitio:**
   ```bash
   pnpm run build
   ```
   *(O `npm run build`)*
   
   Esto generará una carpeta llamada `dist/` en la raíz del proyecto con todos los archivos optimizados.

2. **Previsualizar la compilación localmente:**
   Para verificar que todo funciona perfectamente tal como se subirá a producción, puedes levantar un servidor local para la carpeta `dist/` ejecutando:
   ```bash
   pnpm run preview
   ```
   *(O `npm run preview`)*

---

## 📁 Estructura del Proyecto

A continuación, se detalla la estructura principal de archivos para facilitar tu navegación:

```text
invitacion-prescolar/
├── public/                 # Archivos públicos estáticos (imágenes como foto.png, iconos, etc.)
├── src/
│   ├── components/         # Componentes Astro reutilizables
│   │   ├── Bienvenida.astro          # Card de bienvenida principal y globos interactivos
│   │   ├── FotoPolaroid.astro        # Contenedor de la foto grupal con estilo polaroid
│   │   ├── TarjetaInformacion.astro  # Tarjetas individuales para fecha, hora, lugar, etc.
│   │   ├── PiePagina.astro           # Footer con créditos del diseñador
│   │   ├── Confeti.astro             # Lógica para lanzar confeti interactivo
│   │   └── SolYNubes.astro           # Ilustraciones animadas en el fondo
│   ├── layouts/            # Plantillas generales de la aplicación
│   │   └── Plantilla.astro           # Estructura HTML base y tipografías (Fredoka/FontAwesome)
│   ├── pages/              # Páginas del sitio (rutas dinámicas basadas en archivos)
│   │   └── index.astro               # Página de inicio principal de la invitación
│   └── styles/             # Hojas de estilo globales
│       └── global.css                # Configuración de Tailwind CSS v4 y animaciones personalizadas
├── package.json            # Scripts de ejecución y dependencias del proyecto
└── README.md               # Este archivo de documentación
```

---

## 🎨 Diseñado y Desarrollado por
- **Victor Raúl García García** — *Desarrollador Web*
- Sitio web personal / Portafolio: [porfolio-dhz.pages.dev](https://porfolio-dhz.pages.dev/)
