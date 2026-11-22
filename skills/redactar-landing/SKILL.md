---
name: redactar-landing
description: Redacta y revisa los textos de la web para los campos reales de Sanity Studio (Portada, Servicios, Quiénes somos, Reseñas reales, FAQs y Contacto) a partir de MEMORIA.md, sin inventar cifras ni usar clichés de IA. Use when el alumnado prepara los textos de su web en Sesión 2 o revisa el copy en Sesión 4.
---

# Redactar la landing para el kit (`kit-negocio-web`)

Objetivo: pasar de las hipótesis de `MEMORIA.md` a **textos claros, honestos y orientados a conversión** listos para copiar en los campos exactos de Sanity Studio.

## Antes de empezar

1. Lee `MEMORIA.md` (oferta en una frase, cliente ideal, alternativa actual, diferencia propuesta, recursos y si es proyecto real o caso ficticio). Si falta, sugiere usar antes `aterrizar-idea`.
2. Revisa que no vas a prometer nada sin respaldo en `MEMORIA.md`.

## Estructura y campos exactos de Sanity Studio

Entrega los borradores organizados exactamente según el panel del kit:

1. **Portada (`1. Mi negocio y portada → Portada`):**
   - **Titular** *(máx. 10–12 palabras)*: qué problema resuelves, para quién y dónde (si aplica). Evita frases vacías como *«Llevamos tu negocio al siguiente nivel»*.
   - **Presentación** *(2–3 frases)*: explica cómo trabajas, cuál es la diferencia concreta frente a la alternativa habitual y qué gana el cliente.
   - **Texto del botón** *(2–4 palabras)*: acción concreta (p. ej. *«Pide presupuesto»*, *«Reserva valoración»*, *«Consultar por WhatsApp»*). Evita *«Enviar»* o *«Más información»*.
2. **Servicios (`Servicios`, 3–4 bloques ordenados por beneficio):**
   - Por cada servicio: **Nombre** (claro, no jerga interna), **Descripción** (qué incluye y para quién sirve, 1–2 frases) y **Precio orientativo o criterio** (si está confirmado en `MEMORIA.md`; si no, marcar `[PRECIO O RANGO PENDIENTE]`).
3. **Quiénes somos (`Quiénes somos`):**
   - **Título**, **Texto** (2–3 frases en lenguaje directo sobre quién está detrás y cómo trabaja) y **3 puntos destacados** solo con hechos verificables (titulación, zona, presupuesto por escrito). *Si es un caso ficticio, márcalo expresamente.*
4. **Reseñas y perfiles verificados *(solo si ya existen valoraciones públicas reales)*:**
   - Si no hay reseñas reales todavía, indica **«Dejar desactivado hasta tener las primeras reseñas verificables»** y sugiere el texto del botón para pedirlas (*Google Maps, ProvenExpert, Trustpilot o LinkedIn*).
5. **Preguntas frecuentes de la portada (`4. Contacto… → Preguntas frecuentes`, 4–5 FAQs):**
   - Responde a las **objeciones reales** del cliente (precio/forma de pago, plazos, zona de cobertura, qué incluye la primera toma de contacto, qué pasa si no encaja). Respuestas directas de 2–3 líneas (ideales también para `/llms.txt` y Google).
6. **Contacto / Reserva / WhatsApp:**
   - **Texto de invitación:** explica exactamente qué ocurre después de escribir y en cuánto tiempo respondes.

## Reglas anti-invención y filtro anti-AI-slop

- **Cero datos inventados:** nunca añadas testimonios ficticios, años de experiencia no declarados, premios, sellos ni garantías absolutas (*«100 % garantizado»*). Si falta un dato concreto, escribe `[COMPLETAR CON DATO REAL]`.
- **Pasa el filtro de `humanizar-textos` antes de entregar:** elimina aperturas cliché (*«En el mundo actual…»*), adjetivos vacíos (*«solución integral, innovadora y personalizada»*), rayas largas excesivas y frases en tono de folleto corporativo.
- **Un único objetivo por bloque:** el lector debe entender en **5 segundos** qué ofreces, para quién es y qué botón pulsar.

## Salida

Presenta todos los bloques listos para copiar y pegar en Sanity Studio, más una lista breve al final con los `[DATOS PENDIENTES]` que la persona debe confirmar antes de pulsar **Publish**.
