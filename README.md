# Portal de Microelectrónica y Semiconductores UTEQ

Primera versión (MVP) de un portal informativo construido con Jekyll y preparado para GitHub Pages.

## Secciones
- Inicio
- Noticias y actividades (`_posts/`)
- Convocatorias (`_convocatorias/`)
- Eventos (`_eventos/`)
- Comunidad estudiantil (`_comunidad/`)
- Proyectos y laboratorios (`_proyectos/`)

## Publicar en GitHub Pages
1. Crea un repositorio en GitHub, por ejemplo `portal-microelectronica-uteq`.
2. Sube el contenido de esta carpeta a la rama `main`.
3. En GitHub abre **Settings → Pages**.
4. En **Build and deployment**, selecciona **Deploy from a branch**, rama `main` y carpeta `/ (root)`.
5. Guarda. GitHub Pages construirá el sitio con Jekyll.

Si el repositorio es un proyecto (por ejemplo `usuario/portal-microelectronica-uteq`), configura en `_config.yml`:
```yml
url: "https://usuario.github.io"
baseurl: "/portal-microelectronica-uteq"
```
Si se publica como sitio de usuario/organización, normalmente `baseurl` queda vacío.

## Ejecutar localmente
Requiere Ruby y Bundler:
```bash
bundle install
bundle exec jekyll serve
```
Abre `http://127.0.0.1:4000`.

## Agregar una noticia
Crea un archivo en `_posts/` con el formato `AAAA-MM-DD-titulo.md`:
```yml
---
title: "Título de la noticia"
date: 2026-11-16
category: Formación
excerpt: "Resumen breve para la tarjeta."
---
Contenido de la noticia...
```

## Agregar una convocatoria, evento, proyecto o contenido de comunidad
Crea un archivo Markdown dentro de la carpeta correspondiente (`_convocatorias/`, `_eventos/`, `_proyectos/`, `_comunidad/`) con front matter:
```yml
---
title: "Nombre"
description: "Descripción breve"
category: "Formación"
status: "Abierta"
status_key: "done"
---
Contenido...
```

## Criterios editoriales
Antes de publicar, confirmar fechas, nombres oficiales, organizadores, enlaces, participantes y autorización para usar fotografías/logotipos. Diferenciar actividades realizadas, programadas, convocatorias abiertas y propuestas en desarrollo.

## Pendientes antes de publicación institucional
- Confirmar denominación oficial de la carrera y unidad académica.
- Validar identidad gráfica y uso del logotipo UTEQ.
- Confirmar autorización institucional, dominio y responsable editorial.
- Sustituir textos de ejemplo por notas verificadas.
- Incorporar fotografías propias con autorización.
- Añadir correo o canal institucional de contacto.
