# Skills y plantillas de trabajo (`COMM0006` / `IFCT029PO`)

Material de arranque para definir la oferta, investigar el mercado, redactar la web sin clichés de IA, auditar SEO/AEO/CRO/calidad técnica, reutilizar contenidos y decidir el siguiente paso sin planificar en exceso.

> **¿Buscas la plantilla de la web?** El kit web (Astro + Sanity + Netlify) está en su propio repositorio: [`desdequeteperdi/kit-negocio-web`](https://github.com/desdequeteperdi/kit-negocio-web) (e incluye opcionalmente `npm run mcp` para conectar Sanity, Netlify y Playwright sin Google Cloud). En este repositorio viven las **12 skills de IA** y las **plantillas de negocio** para empezar desde el Día 1.

---

## Cómo empezar en 3 minutos (Windows y Mac)

1. **Descarga esta carpeta en tu ordenador:**
   - **Sin comandos:** pulsa el botón verde **`<> Code` → `Download ZIP`** y descomprímelo en **`C:\proyectos\marketing-skills`** (Windows) o en tu carpeta de proyectos en Mac *(evita carpetas sincronizadas con OneDrive/iCloud si luego vas a juntarlo con el kit web)*.
   - **Con Git:**
     ```bash
     git clone https://github.com/desdequeteperdi/marketing-skills.git
     ```
2. **Crea tu documento único de trabajo (`MEMORIA.md`):**
   - Copia `plantillas/memoria-negocio.md` en esta misma carpeta y guárdalo como **`MEMORIA.md`**.
   - Si no tienes un negocio o proyecto propio todavía, elige uno de los **12 modelos reales** en [`plantillas/proyectos-ejemplo.pdf`](plantillas/proyectos-ejemplo.pdf) (o [`plantillas/proyectos-ejemplo.md`](plantillas/proyectos-ejemplo.md)).
3. **Usa las skills en orden:**
   - **Opción A (chat web: ChatGPT, Claude, Gemini…):** pega el contenido del archivo `SKILL.md` correspondiente junto con tu `MEMORIA.md` y pídele que siga esas instrucciones paso a paso (modo manual: te dará los textos listos para copiar y pegar en Sanity Studio).
   - **Opción B (agente de código en VS Code: Claude Code, Antigravity, Codex, Cursor…):** abre la carpeta y escribe, por ejemplo: *«Lee `skills/aterrizar-idea/SKILL.md` y aplícalo sobre mi `MEMORIA.md`»*.
     - **Doble modo con MCP de Sanity:** si además conectas el MCP opcional del kit (`npm run mcp` en `kit-negocio-web`), las skills de redacción, SEO, reutilización y auditoría leen primero tus documentos, te piden confirmación antes de escribir y guardan **solo borradores (`drafts.*`)**, respetando los **13 *singletons*** y sin publicar ni borrar nada sin tu permiso.

> **Regla de privacidad:** nunca introduzcas datos personales reales de clientes en herramientas de IA y no subas tu `MEMORIA.md` a repositorios públicos (está ignorada en `.gitignore`).

---

## Contenido

### 1. Skills (`skills/`)

#### Estrategia y experimentación
| Orden | Skill | Para qué sirve | Archivo |
|---|---|---|---|
| **1** | `aterrizar-idea` | Pasar de una idea general a una oferta en una frase, recursos, límites, hipótesis y encaje inicial en el kit | [`skills/aterrizar-idea/SKILL.md`](skills/aterrizar-idea/SKILL.md) |
| **2** | `investigar-mercado` | Analizar 5–10 alternativas reales con precios, URLs, fechas, pruebas en contra y guion de entrevistas | [`skills/investigar-mercado/SKILL.md`](skills/investigar-mercado/SKILL.md) |
| **2 bis** | `comparar-competidores` | Comparar cara a cara 3–6 alternativas reales con fuentes, fecha, filtro «tener vs. importar» y traducción opcional a Sanity | [`skills/comparar-competidores/SKILL.md`](skills/comparar-competidores/SKILL.md) |
| **Opcional** | `consejo-asesores` | Revisión crítica simulada desde 5 perspectivas (cliente, mensaje, captación, costes/operatividad en el kit y asesor que contradice) | [`skills/consejo-asesores/SKILL.md`](skills/consejo-asesores/SKILL.md) |
| **3** | `disenar-experimento` | Definir la primera prueba pequeña (`E1`) con señal observable, plazo, presupuesto máximo y montaje sin código en el kit | [`skills/disenar-experimento/SKILL.md`](skills/disenar-experimento/SKILL.md) |
| **4** | `interpretar-resultados` | Separar observaciones medibles (excluyendo ensayos `PRUEBA`) de hipótesis y decidir: continuar, modificar o detener | [`skills/interpretar-resultados/SKILL.md`](skills/interpretar-resultados/SKILL.md) |

#### Redacción, auditoría y difusión (`kit-negocio-web`)
| Cuándo | Skill | Para qué sirve | Archivo |
|---|---|---|---|
| **Sesiones 2 y 4** | `redactar-landing` | Redactar textos reales para los 4 grupos de Sanity Studio (portada, páginas/landings `/[slug]`, `/enlaces`, blog, catálogo/Stripe, captación, SEO y legal) sin inventar datos | [`skills/redactar-landing/SKILL.md`](skills/redactar-landing/SKILL.md) |
| **En cualquier texto** | `humanizar-textos` | Filtro **anti-AI-slop** en español: elimina muletillas y tono robótico de IA y lo sustituye por hechos reales de `MEMORIA.md` | [`skills/humanizar-textos/SKILL.md`](skills/humanizar-textos/SKILL.md) |
| **Sesiones 4, 6 y 8** | `auditar-web-seo` | Auditar conversión móvil, reseñas verificables (Google, ProvenExpert, Trustpilot, LinkedIn), SEO global y por página, perfil local (físico/SAB/remoto), AEO (`/llms.txt`), tienda/módulos y privacidad | [`skills/auditar-web-seo/SKILL.md`](skills/auditar-web-seo/SKILL.md) |
| **Sesiones 5, 9 / blog** | `reutilizar-contenido` | Flujo «1 artículo → 3 piezas» (carrusel, publicación breve/GBP, guion vídeo corto o Brevo) + bloque *En resumen* (AEO) + `/enlaces` + UTMs | [`skills/reutilizar-contenido/SKILL.md`](skills/reutilizar-contenido/SKILL.md) |

#### Auditoría técnica y de conversión externa (adaptada al kit)
| Cuándo | Skill | Para qué sirve | Origen y licencia |
|---|---|---|---|
| **Sesiones 4 y 9 / campañas** | `landing-page-conversion-audit` | Revisión enfocada a fugas de conversión en portada, landings `/[slug]`, `/enlaces` o fichas de producto/pago (encaje anuncio-página, primer pantallazo móvil, claridad de oferta, fricción en formulario/WhatsApp/reservas/Stripe y ruta `/gracias`) | Adaptada de [`autonnel/autonnel-skills`](https://github.com/autonnel/autonnel-skills) · Apache-2.0 ([`LICENSE`](skills/landing-page-conversion-audit/LICENSE)) |
| **Sesiones 6 y 8 / lanzamiento** | `web-quality-audit` | Auditoría técnica basada en evidencias sobre la web publicada o compilada (`web/dist`, nunca `studio/`): Core Web Vitals, accesibilidad (WCAG), SEO técnico, buenas prácticas y navegación agéntica (incluye [`scripts/analyze.sh`](skills/web-quality-audit/scripts/analyze.sh) y [`references/MEASUREMENT.md`](skills/web-quality-audit/references/MEASUREMENT.md)) | Adaptada de [`addyosmani/web-quality-skills`](https://github.com/addyosmani/web-quality-skills) · MIT ([`LICENSE`](skills/web-quality-audit/LICENSE)) |

### 2. Plantillas (`plantillas/`)

- [`plantillas/memoria-negocio.md`](plantillas/memoria-negocio.md): plantilla base para crear tu `MEMORIA.md` (separa **declarado**, **evidencia**, **inferencia** e **hipótesis**).
- [`plantillas/proyectos-ejemplo.pdf`](plantillas/proyectos-ejemplo.pdf) *(y [`.md`](plantillas/proyectos-ejemplo.md))*: catálogo de 12 proyectos ejemplo adaptados al kit web.

---

## Licencia

Material docente bajo [Creative Commons Atribución 4.0 Internacional (CC BY 4.0)](LICENSE). Las skills externas incorporadas en `skills/` conservan sus licencias originales (`Apache-2.0` en `landing-page-conversion-audit` y `MIT` en `web-quality-audit`).
