# SEO Checklist para Mauricio Belforte

Este documento es una lista de verificación para implementar las mejores prácticas de SEO en la web de tu agencia:
`https://mauricio-belforte.web.app/`.

Cada ítem debe revisarse y marcarse cuando esté completo.

## Estructura y semántica

- [x] Verificar uso de HTML semántico (`<header>`, `<main>`, `<section>`, etc.)
- [x] Asegurar jerarquía lógica de encabezados (`h1` único, h2, h3...)
- [x] Mantener cards de precios y FAQs intactas; cualquier cambio requiere autorización previa.

## Metadatos y etiquetas

- [x] `<title>` con palabra clave principal: "desarrollador web Trelew", "agencia web Trelew".
- [x] `<meta name="description">` con descripción atractiva y <160 caracteres.
- [x] `<meta name="keywords">` orientado a Trelew y desarrollo web.
- [x] Incluir `<meta name="author" content="Mauricio Belforte">`.
- [x] `<meta name="viewport" content="width=device-width, initial-scale=1.0">` presente.
- [x] Añadir `<link rel="canonical" href="https://mauricio-belforte.web.app/">` en todas las páginas.
- [x] Gestionar `<meta name="robots">` según entorno (desarrollo vs producción).

## Indexación y archivos auxiliares

- [x] Crear/actualizar `robots.txt` en la raíz del hosting permitiendo acceso.
- [x] Generar `sitemap.xml` con la URL canónica y subir a Search Console.
- [x] Subir el sitemap a Google Search Console y Bing Webmaster.

## Contenido y palabras clave

- [x] Realizar investigación de palabras clave orientada a clientes en Trelew ("desarrollador web Trelew", "páginas web Trelew", etc.).
- [x] Distribuir palabras clave en títulos, primeras 100 palabras, encabezados y meta description.
- [ ] Mantener densidad natural (1–2%) y variar con sinónimos y LSI.

## Local SEO y directorios

- [x] Añadir datos estructurados `LocalBusiness` o `WebSite` con dirección en Trelew.
- [ ] Registrar la empresa en Google My Business y completar ficha con fotos, horarios y datos.
- [ ] Buscar directorios locales de Trelew y categorías de servicios web para inclusión.

## Redes sociales y compartir

- [x] Añadir etiquetas Open Graph (`og:title`, `og:description`, `og:image`, `og:url`).
- [x] Añadir Twitter Cards (`twitter:card`, `twitter:title`, etc.).
- [ ] Verificar imágenes compartidas y textos en WhatsApp, Facebook y LinkedIn.

## Rendimiento y UX técnico

- [x] Especificar `width` y `height` en `<img>` para evitar CLS.
- [x] Aplicar `loading="lazy"` en imágenes no críticas.
- [x] Definir `@font-face` con `font-display: swap`.
- [ ] Revisar velocidad y optimizar carga con Lighthouse (LCP, FID, CLS). (Este punto es más amplio y requiere herramientas externas)
- [x] Asegurar accesibilidad mínima (`aria-label`, contrastes, nav accesible).

## URLs y enlaces

- [x] Usar URLs limpias y amigables, separadas por guiones, minúsculas.
- [x] Evitar parámetros de consulta innecesarios.
- [ ] Implementar redirecciones 301 si se cambian URLs.

## Monitoreo y mantenimiento

- [x] Configurar Google Search Console y Bing Webmaster.
- [x] Añadir Google Analytics o similar para seguimiento de tráfico.
- [ ] Programar revisiones mensuales de SEO (palabras clave, performance, errores).

---

**Referencia adicional:**

- [x] Implementar la guía SEO adaptada al proyecto (consultar `GUIA_SEO.md`).
