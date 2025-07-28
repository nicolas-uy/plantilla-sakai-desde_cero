# Proyecto Angular 20 + Sakai PrimeNG

Base funcional con routing standalone, Tailwind y PrimeNG utilizando plantilla Sakai.

## Requisitos Previos

- Node.js y NPM (https://nodejs.org)
- Angular CLI (`npm install -g @angular/cli@20.0.5`)
- IDE recomendado: WebStorm, VS Code

## Instalación y configuración rápida

### 1. Crear nuevo proyecto Angular

```bash
ng new nombre-del-proyecto
```
- Zoneless: No
- Hojas de estilo: SCSS (Sass)
- SSR/SSG: No

### 2. Descargar y adaptar plantilla Sakai

- Descarga desde [https://github.com/primefaces/sakai-ng](https://github.com/primefaces/sakai-ng)
- Copia al nuevo proyecto:
    - `src/assets`
    - `src/app/layout`
- Elimina `.vscode` y `public` si existen.

### 3. Instalar dependencias principales

```bash
npm install @angular/core@^20
npm install @angular/common@^20 @angular/forms@^20
npm install @angular/router@^20 @angular/animations@^20
npm install @angular/compiler@^20 @angular/platform-browser@^20 @angular/platform-browser-dynamic@^20
npm install primeng@^20 primeicons@^7.0.0
npm install chart.js@4.4.2
npm install @primeuix/themes@^1.2.1
npm install -D tailwindcss@^4.1.11 postcss@^8.5.6 autoprefixer
npm install -D @tailwindcss/forms @tailwindcss/typography
npm install tailwindcss-primeui@^0.6.1
npm install @tailwindcss/postcss@^4.1.11
```

### 4. Crear/ajustar los siguientes archivos base

- `src/index.html`
- `src/main.ts`
- `src/app.component.ts`
- `src/app.config.ts`
- `src/app.routes.ts`
- `src/app/pages/pages.routes.ts`
- `postcssrc.json` (en la raíz)

> Usa el contenido proporcionado en la plantilla Sakai y ajusta rutas/componentes según la estructura standalone del proyecto.

### 5. Modificar angular.json

Cambia la ruta en `"styles"` por:
```json
"src/assets/styles.scss"
```
También en la sección de test.

---

## Estructura mínima esperada

```
src/
  app.component.ts
  app.config.ts
  app.routes.ts
  main.ts
  index.html
  app/
    layout/
    pages/
      dashboard/
      notfound/
      empty/
      pages.routes.ts
assets/
  styles.scss
postcssrc.json
```

---

## Tecnologías

- Angular 20, Angular CLI
- PrimeNG, PrimeUIX (Tema Aura)
- Tailwind CSS, PostCSS, Autoprefixer
- Chart.js, PrimeIcons

---

## Palabras clave

Angular 20, PrimeNG, Sakai, Tailwind CSS, Routing Standalone, Tema Aura

---

### Créditos y Licencia

Este proyecto utiliza archivos y estructuras derivadas de la plantilla **Sakai de PrimeNG**, desarrollada por [**PrimeTek Informatics**](https://www.primetek.com.tr/), y distribuida a través de su sitio oficial y repositorio GitHub para clientes con licencia.

🔒 **Importante**:  
Todo el código fuente original de Sakai (estilos, assets, componentes) es propiedad de PrimeTek y está protegido por su licencia comercial.  
Mi autoría se limita exclusivamente a la creación del proyecto base en Angular 20, su configuración estructural con routing standalone, la integración de Tailwind CSS, y documentación de instalación.

Para usar otras plantillas en tus proyectos, debes contar con una licencia válida otorgada por PrimeTek.
