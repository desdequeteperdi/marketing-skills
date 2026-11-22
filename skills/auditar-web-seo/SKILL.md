---
name: auditar-web-seo
description: Audita una web del kit (conversión móvil, prueba social verificable, SEO técnico básico, perfil local físico/SAB/remoto, AEO /llms.txt y privacidad) a partir de la URL publicada, localhost o HTML. Use when se revisa la web en Sesión 4, 6 u 8.
---

# Auditar conversión, SEO local y AEO (`/llms.txt`)

Objetivo: detectar fallos reales de **claridad comercial, confianza, SEO local, respuestas en IA (AEO) y privacidad** sin inventar métricas ni exigir herramientas de pago.

## Antes de empezar

1. Lee `MEMORIA.md` (si existe) para saber qué vende el negocio, cuál es su acción principal y qué perfil local tiene:
   - **Perfil 1 · Local físico** (atención en tienda/estudio/despacho).
   - **Perfil 2 · A domicilio / área de servicio (SAB)** (dirección oculta en Maps).
   - **Perfil 3 · 100 % online / remoto** (sin ficha de Google Maps).
2. Pide o inspecciona la web (si tienes Playwright MCP o acceso local a `web/dist` / `http://localhost:4321`, revísala directamente; si no, pide que peguen el texto visible o la URL).

## Checklist de auditoría en 5 bloques

### 1. Claridad y conversión en móvil (primeros 5 segundos)
- ¿Se entiende qué vendes, para quién y dónde sin hacer scroll?
- ¿El botón principal lleva a una única acción clara y el teléfono/WhatsApp tienen buen tamaño táctil?
- ¿Quedan textos de ejemplo sin sustituir (*«Estudio Almendro»*, *«Negocio ficticio de ejemplo»*)?

### 2. Señales de confianza reales (cero humo)
- ¿Las afirmaciones de *Servicios* y *Quiénes somos* son comprobables?
- Si muestra testimonios o reseñas: ¿usa el bloque **Reseñas y perfiles verificados** con enlaces reales a **Google Maps, ProvenExpert, Trustpilot, LinkedIn o un directorio sectorial**? *(Si hay citas sin fuente ni contexto real en un proyecto real, márcalo como riesgo de credibilidad).*

### 3. SEO básico y datos estructurados
- **Título en Google** (`≤ 70` caracteres): incluye servicio principal + zona/público (evita *«Inicio»* o solo el nombre).
- **Descripción en Google** (`≤ 160` caracteres): explica beneficio y siguiente paso.
- **Imagen al compartir (`og:image`):** `1200 × 630 px` en JPG/PNG/WebP (no SVG).
- **Imágenes:** todas tienen descripción `alt` útil.
- **JSON-LD (`DatosEstructurados.astro`):** subtipo correcto de `LocalBusiness`, `areaServed` sin exponer domicilio privado y `sameAs` con redes y perfiles de reseñas.

### 4. Estrategia local y AEO (`/llms.txt`)
- **Coherencia con el perfil (1, 2 o 3):** si es a domicilio o remoto, verifica que **no** muestra su dirección particular en portada ni pie; si tiene ficha local, comprueba consistencia **NAP** (Nombre, Zona/Dirección, Teléfono).
- **`/llms.txt`:** ¿resume de forma limpia qué hace el negocio, sus servicios, FAQs con respuestas directas y perfiles de reseñas para que ChatGPT/Perplexity/Gemini no alucinen?

### 5. Privacidad y control
- Si está recogiendo datos reales (formulario, WhatsApp + Sheets o Reservas): ¿están rellenos **Datos legales** (titular, NIF, domicilio fiscal, plazo de conservación)?
- Si hay GA4, GTM o Meta Pixel: ¿aparece el banner de cookies y bloquea los scripts antes de aceptar?

## Salida

Entrega un informe breve ordenado por impacto:
1. **3 fallos prioritarios a corregir hoy** (con el cambio exacto sugerido en Sanity Studio o en el kit).
2. **Mejoras recomendadas** para SEO local / AEO / reseñas verificables.
3. **Qué está ya bien resuelto.**
