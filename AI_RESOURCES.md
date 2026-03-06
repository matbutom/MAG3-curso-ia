# Recursos de IA para Generación de Imágenes y Video

> Directorio curado de herramientas de IA con niveles gratuitos, pruebas gratuitas u opciones de código abierto.
> Solo se incluyen herramientas activamente mantenidas (actualizadas en los últimos 12 meses).
>
> **Leyenda:**
> - ✅ Nivel gratuito especialmente generoso
> - ⚠️ Nivel gratuito muy limitado
> - 🔓 Código abierto / autoalojable

---

## Índice

- [Herramientas de Generación de Imágenes](#herramientas-de-generación-de-imágenes)
- [Herramientas de Generación de Video](#herramientas-de-generación-de-video)
- [Opciones de Código Abierto / Autoalojables](#opciones-de-código-abierto--autoalojables)
- [Acceso Rápido por Caso de Uso](#acceso-rápido-por-caso-de-uso)

---

## Herramientas de Generación de Imágenes

### Tabla Comparativa Rápida

| Herramienta | Imágenes gratuitas | Marca de agua | Tarjeta requerida | API | Código abierto |
|---|---|---|---|---|---|
| Bing Image Creator | ✅ Ilimitadas (lentas tras créditos) | No | No | Pagada (Azure) | No |
| Leonardo.AI | ~30–75/día (150 tokens) | Sí (públicas) | No | Sí (pagada) | No |
| Adobe Firefly | ~25/mes | No | No | Sí (empresa) | No |
| Ideogram | Créditos semanales lentos | No | No | Sí (pagada) | No |
| Playground AI | ⚠️ 10 cada 3 horas | No | No | Limitada | No |
| Canva IA | ⚠️ 50 créditos de por vida | No | No | Limitada | No |
| Craiyon | ✅ Ilimitadas (sin registro) | No | No | No | No |
| NightCafe | 5/día + bonos comunidad | No | No | No | No |
| Freepik IA | ✅ 20/día | No | No | Sí (pagada) | No |
| DreamStudio | ⚠️ 200 créditos al registrarse | No | No | Sí (pagada) | No |
| Fotor | ⚠️ 8 iniciales + diario | No | No | No | No |
| Raphael AI | ✅ Ilimitadas | No | No | No | No |
| Google Gemini Flash | ✅ 500/día (API) | No | No | Sí (gratis) | No |

---

### Bing Image Creator (DALL-E 3 / GPT Image 1) ✅

**URL:** https://www.bing.com/images/create
**Categoría:** Imagen
**Nivel gratuito:** Generaciones ilimitadas con cuenta Microsoft; créditos "Boost" (cola rápida) son finitos pero la generación lenta permanece gratuita para siempre. Sin marca de agua.
**Requiere tarjeta de crédito:** No — cualquier cuenta Microsoft gratuita funciona
**Acceso a API:** Solo via Azure OpenAI API (pagada); la interfaz web es completamente gratuita
**Mejor para:** Uso general, escenas fotorrealistas, arte conceptual, carteles, contenido para redes sociales
**Limitaciones:** Generación más lenta al agotarse los Boosts; sin API comercial sin facturación Azure
**Planes de pago:** Ninguno para la web; precios API de Azure (~$0.04 por imagen para DALL-E 3)
**Código abierto:** No
**Nota:** En marzo de 2025 OpenAI reemplazó DALL-E 3 con GPT Image 1 como modelo subyacente

---

### Leonardo.AI

**URL:** https://leonardo.ai
**Categoría:** Imagen (también tiene funciones de video/movimiento)
**Nivel gratuito:** 150 tokens diarios (se reinician cada 24h); los tokens cuestan 4–8 por imagen según modelo y resolución. Equivale a ~30–75 imágenes/día. Las imágenes gratuitas son públicas.
**Requiere tarjeta de crédito:** No
**Acceso a API:** Sí — API REST disponible, pago por token
**Mejor para:** Assets de videojuegos, arte conceptual, diseño de personajes, impresión bajo demanda, visualización de productos
**Limitaciones:** Imágenes gratuitas son públicas; colas más lentas en horas pico (5–20 min); algunos modelos cuestan tokens extra
**Planes de pago desde:** $12/mes (Aprendiz)
**Código abierto:** No

---

### Adobe Firefly

**URL:** https://firefly.adobe.com
**Categoría:** Imagen (también tiene generación de video y vectores)
**Nivel gratuito:** 25 créditos generativos/mes en el plan gratuito de Adobe Creative Cloud. Sin marca de agua; comercialmente seguro (entrenado con contenido licenciado)
**Requiere tarjeta de crédito:** No para cuenta Creative Cloud gratuita
**Acceso a API:** Sí — Firefly API disponible (empresa/pago)
**Mejor para:** Flujos de trabajo de diseño profesional, integración con Photoshop (Relleno Generativo), activos de marketing, imágenes comerciales seguras para marcas
**Limitaciones:** Solo 25 créditos/mes en nivel gratuito; los créditos se consumen más rápido en configuraciones de alta calidad
**Planes de pago desde:** $9.99/mes (Firefly Standard — 100 créditos)
**Código abierto:** No

---

### Ideogram

**URL:** https://ideogram.ai
**Categoría:** Imagen
**Nivel gratuito:** Créditos semanales con cola lenta (se reinician cada sábado); los usuarios gratuitos pueden generar imágenes pero los tiempos de espera pueden ser varios minutos
**Requiere tarjeta de crédito:** No
**Acceso a API:** Sí — API REST disponible (pagada)
**Mejor para:** Tipografía en imágenes, diseño de carteles, logos, diseños de camisetas, visuales con texto legible — Ideogram es especialmente fuerte en renderizar texto coherente y legible en imágenes
**Limitaciones:** El nivel gratuito usa cola lenta; sin acceso prioritario; algunas funciones avanzadas requieren plan de pago
**Planes de pago desde:** $8/mes (Básico)
**Código abierto:** No

---

### Playground AI

**URL:** https://playground.com
**Categoría:** Imagen
**Nivel gratuito:** ⚠️ 10 imágenes cada 3 horas. Aloja modelos GPT-4o y Nano Banana Pro.
**Requiere tarjeta de crédito:** No
**Acceso a API:** Limitada
**Mejor para:** Maquetas de diseño, gráficos para redes sociales, proyectos creativos colaborativos
**Limitaciones:** 10 imágenes por ventana de 3 horas; la plataforma ha pivotado hacia una experiencia de herramienta de diseño
**Planes de pago desde:** $15/mes (Pro)
**Código abierto:** No

---

### Canva Generador de Imágenes IA

**URL:** https://www.canva.com/ai-image-generator/
**Categoría:** Imagen
**Nivel gratuito:** ⚠️ 50 créditos IA de por vida en el plan gratuito de Canva. Estilos incluyen Acuarela, Fílmico, Neón, etc. Totalmente integrado en el entorno de diseño de Canva.
**Requiere tarjeta de crédito:** No
**Acceso a API:** Via plataforma de desarrolladores de Canva (limitada)
**Mejor para:** Publicaciones en redes sociales, presentaciones, materiales de marketing, flujos de trabajo de diseño integrados
**Limitaciones:** 50 créditos son de por vida (no mensual); no apto para generación masiva; resolución limitada en plan gratuito
**Planes de pago desde:** $15/mes (Canva Pro — 500 créditos/mes)
**Código abierto:** No

---

### Craiyon (antes DALL-E mini) ✅

**URL:** https://www.craiyon.com
**Categoría:** Imagen
**Nivel gratuito:** ✅ Generaciones ilimitadas — sin registro requerido. Genera 9 variaciones de imagen por prompt.
**Requiere tarjeta de crédito:** No
**Acceso a API:** Sin API pública oficial
**Mejor para:** Ideación rápida, generación experimental/lúdica, acceso sin registro
**Limitaciones:** Generación más lenta; soportado por anuncios; calidad de imagen inferior a herramientas premium
**Planes de pago desde:** $5/mes (Supporter — sin anuncios, más rápido)
**Código abierto:** No (derivado de modelos de código abierto)
**Nota:** Sin marcas de agua; uso comercial permitido

---

### NightCafe

**URL:** https://nightcafe.studio
**Categoría:** Imagen (también ofrece modelos de video: Runway, Kling, Seedance)
**Nivel gratuito:** 5 créditos/día (1 crédito ≈ 1 imagen). La participación en la comunidad (me gusta, comentarios) gana créditos extra. Aloja la selección de modelos más amplia: FLUX, Stable Diffusion, DALL-E 3, Imagen, Gemini, Ideogram, HiDream, Seedream.
**Requiere tarjeta de crédito:** No
**Acceso a API:** Sin API pública
**Mejor para:** Exploración artística, experimentos con múltiples estilos, compartir en comunidad; ideal para usuarios que quieren comparar muchos modelos en una sola plataforma
**Limitaciones:** Solo 5 créditos gratuitos/día; uso comercial permitido incluso en plan gratuito
**Planes de pago desde:** $6/mes (Principiante IA — 100 créditos)
**Código abierto:** No (plataforma; usa modelos de código abierto)

---

### Freepik Generador de Imágenes IA ✅

**URL:** https://www.freepik.com/ai/image-generator
**Categoría:** Imagen
**Nivel gratuito:** ✅ 20 generaciones de imágenes IA gratuitas por día. Usa modelos FLUX y el modelo propietario "Mystic".
**Requiere tarjeta de crédito:** No
**Acceso a API:** Sí — API de Freepik disponible para generación de imágenes (pagada)
**Mejor para:** Assets de diseño, visuales de marketing, contenido estilo stock comercial
**Limitaciones:** 20 imágenes/día en nivel gratuito; algunos estilos y la mejora de resolución requieren premium
**Planes de pago desde:** $12/mes (Essential)
**Código abierto:** No

---

### DreamStudio (Stability AI)

**URL:** https://dreamstudio.stability.ai
**Categoría:** Imagen
**Nivel gratuito:** ⚠️ 200 créditos al registrarse para nuevos usuarios (~25+ imágenes en configuración predeterminada). Pago por uso después.
**Requiere tarjeta de crédito:** No para créditos de prueba; sí para comprar créditos adicionales
**Acceso a API:** Sí — API REST de Stability AI (pagada, ~$0.065/imagen para SD 3.5 Large)
**Mejor para:** Interfaz oficial para modelos Stable Diffusion; generación de imágenes fotorrealistas, artísticas y estilizadas
**Limitaciones:** Los créditos se agotan rápidamente; sin nivel gratuito continuo tras los créditos iniciales
**Planes de pago:** Pago por crédito: $10 por 1,000 créditos (~5,000 imágenes estándar)
**Código abierto:** No (pero los modelos Stable Diffusion subyacentes sí lo son)

---

### Raphael AI ✅

**URL:** https://raphael.app
**Categoría:** Imagen
**Nivel gratuito:** ✅ Completamente gratuito sin tarifas ocultas, sin tarjeta de crédito y sin límites de uso
**Requiere tarjeta de crédito:** No
**Acceso a API:** No prominentemente anunciada
**Mejor para:** Generación de imágenes en general, creación de obras de arte
**Limitaciones:** Plataforma menos establecida que las principales; la profundidad de calidad y funciones puede variar
**Planes de pago:** Ninguno reportado (totalmente gratuito)
**Código abierto:** No

---

### Google Gemini / Imagen 3 (via AI Studio) ✅

**URL:** https://aistudio.google.com / https://gemini.google.com
**Categoría:** Imagen
**Nivel gratuito:** ✅ Gemini 2.5 Flash Image: 500 solicitudes API gratuitas/día via Google AI Studio (clave API gratuita, sin facturación). Gemini.google.com incluye generación de imágenes en el nivel gratuito para consumidores.
**Requiere tarjeta de crédito:** No para la app Gemini; No para el nivel gratuito de AI Studio
**Acceso a API:** Sí — nivel gratuito de Gemini API a 500 solicitudes/día; Imagen 3 requiere facturación
**Mejor para:** Prototipado rápido, flujos de trabajo integrados, experimentación de desarrolladores
**Limitaciones:** Gemini 3 Pro Image e Imagen 3 requieren facturación de pago; el nivel gratuito usa el modelo Flash
**Planes de pago desde:** $20/mes (Gemini Advanced); API de pago por uso
**Código abierto:** No

---

## Herramientas de Generación de Video

### Tabla Comparativa Rápida

| Herramienta | Generaciones gratuitas | Resolución | Marca de agua | CC requerida | API | Uso comercial (gratis) |
|---|---|---|---|---|---|---|
| Runway | ⚠️ 125 créditos únicos | 720p | Sí | No | Sí (pagada) | No |
| Pika | ⚠️ 80 créditos únicos | Limitada | Sí | No | Limitada | No |
| Luma AI | 30/mes | Borrador | Sí | No | Sí (pagada) | No |
| Kling AI | ✅ 66 créditos/día | 720p | Sí | No | Sí (pagada) | No |
| Hailuo (MiniMax) | ⚠️ 70 únicos (expiran 3d) | Varía | Sí | No | Sí | No |
| Synthesia | 10 min/mes | 1080p | Sí | No | Sí (pagada) | No |
| HeyGen | ⚠️ 1 min total | Varía | Sí | No | Sí | No |
| Fliki | ⚠️ 5 min/mes | 720p | Sí | No | Sí | No |
| InVideo AI | ⚠️ 2 min/semana | Varía | Sí | No | No | No |
| PixVerse | ✅ 60 créditos/día | 540p | Sí | No | Sí (pagada) | No |
| Kapwing | 4 min por exportación | 720p | Sí | No | No | No |

---

### Runway (Gen-4 / Gen-4 Turbo)

**URL:** https://runwayml.com
**Categoría:** Video (texto a video, imagen a video, video a video)
**Nivel gratuito:** ⚠️ 125 créditos únicos al registrarse (~8–10 segundos de video Gen-2). Acceso a 30+ Herramientas Mágicas IA. Resolución máxima 720p. Videos con marca de agua.
**Requiere tarjeta de crédito:** No
**Acceso a API:** Sí — API de Runway disponible (pagada)
**Mejor para:** Generación de video cinematográfico, efectos creativos, edición de video con IA, creación de contenido profesional. Gen-4.5 obtuvo la puntuación Elo más alta (1,247) en el benchmark de Text-to-Video de Artificial Analysis (diciembre 2025).
**Limitaciones:** 125 créditos son únicos (no se recargan); videos gratuitos con marca de agua; 720p máximo; uso comercial restringido en nivel gratuito
**Planes de pago desde:** $15/mes (Standard — 625 créditos)
**Código abierto:** No

---

### Pika (Pika 2.2)

**URL:** https://pika.art
**Categoría:** Video
**Nivel gratuito:** ⚠️ 80 créditos al registrarse; recarga mensual con créditos diarios adicionales. Exportaciones con marca de agua; sin uso comercial en plan gratuito.
**Requiere tarjeta de crédito:** No
**Acceso a API:** API beta limitada
**Mejor para:** Clips cortos para redes sociales, animación de personajes, imagen a video, sincronización de labios
**Limitaciones:** Marcas de agua en todas las exportaciones gratuitas; los 80 créditos se agotan rápidamente; sin derechos comerciales en nivel gratuito
**Planes de pago desde:** $8/mes (Básico)
**Código abierto:** No

---

### Luma AI (Dream Machine)

**URL:** https://lumalabs.ai
**Categoría:** Video (también generación 3D)
**Nivel gratuito:** 30 generaciones de video gratuitas al mes; resolución "borrador"; con marca de agua; solo uso no comercial
**Requiere tarjeta de crédito:** No
**Acceso a API:** Sí — API de Luma disponible (pagada)
**Mejor para:** Generación de video cinematográfico, visualización de productos, generación de escenas 3D, texto a video e imagen a video
**Limitaciones:** 30 generaciones/mes; resolución borrador en nivel gratuito; marca de agua; solo uso personal
**Planes de pago desde:** $29.99/mes (Plus — 10,000 créditos, sin marca de agua)
**Código abierto:** No

---

### Kling AI (Kuaishou) ✅

**URL:** https://klingai.com
**Categoría:** Video
**Nivel gratuito:** ✅ 66 créditos gratuitos al día (se reinician cada 24 horas) — suficiente para 1–6 clips de video cortos. Resolución 720p; salidas con marca de agua; colas más largas.
**Requiere tarjeta de crédito:** No
**Acceso a API:** Sí — API de Kling disponible (pagada)
**Mejor para:** Texto a video, imagen a video, consistencia de personajes, sincronización de labios, video de largo formato hasta 3 minutos
**Limitaciones:** Con marca de agua en nivel gratuito; colas de generación más lentas; máximo 720p
**Planes de pago desde:** $6.99/mes (Standard — 660 créditos)
**Código abierto:** No

---

### Hailuo AI (MiniMax Video-01)

**URL:** https://hailuoai.video
**Categoría:** Video
**Nivel gratuito:** ⚠️ 70 créditos de bienvenida únicos para nuevos usuarios (expiran en 3 días); promociones ocasionales ofrecen 1,000 créditos extra
**Requiere tarjeta de crédito:** No para créditos iniciales
**Acceso a API:** Sí — API de MiniMax disponible
**Mejor para:** Texto a video, imagen a video, movimiento realista; el modelo Hailuo 2.3 fue lanzado con mejor rendimiento en escenas complejas
**Limitaciones:** Los créditos de bienvenida expiran en 3 días; la generación continua requiere suscripción de pago; marca de agua en salidas gratuitas
**Planes de pago desde:** $14.99/mes (Standard — 1,000 créditos)
**Código abierto:** No

---

### Synthesia

**URL:** https://www.synthesia.io
**Categoría:** Video (especialista en avatares IA / cabezas parlantes)
**Nivel gratuito:** Plan demo gratuito: hasta 10 minutos/mes, 9 avatares IA de stock, voces IA en 160+ idiomas, exportación en 1080p; con marca de agua
**Requiere tarjeta de crédito:** No
**Acceso a API:** Sí — API de Synthesia disponible (pagada)
**Mejor para:** Videos de formación corporativa, eLearning, demos de productos, contenido multilingüe a escala usando presentadores IA
**Limitaciones:** Marca de agua en salidas gratuitas; limitado a avatares de stock; avatares personalizados requieren plan de pago
**Planes de pago desde:** $18/mes (Starter — 10 min video/mes)
**Código abierto:** No

---

### HeyGen

**URL:** https://www.heygen.com
**Categoría:** Video (avatar IA / cabeza parlante)
**Nivel gratuito:** ⚠️ Plan gratuito: 1 minuto de video con marca de agua; sin tarjeta de crédito requerida. Acceso a texto a video y funciones de avatar IA.
**Requiere tarjeta de crédito:** No
**Acceso a API:** Sí — API de HeyGen disponible
**Mejor para:** Videos de marketing, explicaciones de productos, portavoz IA, traducción de video con sincronización de labios
**Limitaciones:** Solo 1 minuto total en plan gratuito; marca de agua; sin avatar personalizado sin plan de pago
**Planes de pago desde:** $24/mes (Creator — 15 min/mes)
**Código abierto:** No

---

### Fliki

**URL:** https://fliki.ai
**Categoría:** Video (enfocado en texto a video y texto a voz)
**Nivel gratuito:** ⚠️ 5 minutos de video a 720p por mes; con marca de agua; 300+ voces IA incluidas
**Requiere tarjeta de crédito:** No
**Acceso a API:** Sí — API de Fliki disponible
**Mejor para:** Blog a video, clips para redes sociales, generación de voz en off, automatización de script a video
**Limitaciones:** La marca de agua hace que la salida gratuita sea prácticamente inutilizable para uso profesional; límite duro de 5 min/mes
**Planes de pago desde:** $28/mes (Standard)
**Código abierto:** No

---

### InVideo AI

**URL:** https://invideo.io
**Categoría:** Video (script a video, editor IA)
**Nivel gratuito:** ⚠️ 2 minutos de video y 1 crédito IA por semana; exportaciones con marca de agua
**Requiere tarjeta de crédito:** No
**Acceso a API:** Sin API pública
**Mejor para:** Contenido de YouTube, explicaciones educativas, redes sociales, flujo de trabajo completo de script a video
**Limitaciones:** 2 minutos/semana es muy limitado; marca de agua en todas las exportaciones gratuitas
**Planes de pago desde:** $35/mes (Plus — 10 créditos IA, 50 min/mes)
**Código abierto:** No

---

### PixVerse ✅

**URL:** https://app.pixverse.ai
**Categoría:** Video
**Nivel gratuito:** ✅ 90–100 créditos iniciales + 60 créditos de renovación diaria; resolución 540p con marca de agua PixVerse; soporta texto a video e imagen a video
**Requiere tarjeta de crédito:** No
**Acceso a API:** Sí — API de Plataforma PixVerse (pagada)
**Mejor para:** Clips para redes sociales, video estilo anime, video realista, transformación de baile, sincronización de labios (añadida julio 2025), filtros de efectos virales
**Limitaciones:** 540p en nivel gratuito; marca de agua; uso comercial restringido
**Planes de pago desde:** $10/mes (Standard — 720p, sin marca de agua)
**Código abierto:** No

---

### Kapwing

**URL:** https://www.kapwing.com
**Categoría:** Video (editor asistido por IA más que generador puro)
**Nivel gratuito:** Exportaciones ilimitadas con marca de agua; calidad 720p; funciones IA incluyen subtítulos automáticos, Smart Cut (eliminación de silencios), texto a voz, redimensionado; límite de exportación de 4 minutos
**Requiere tarjeta de crédito:** No
**Acceso a API:** No
**Mejor para:** Edición de video, subtítulos, conversión de formato, contenido de formato corto, reutilización de videos largos
**Limitaciones:** Marca de agua; límite de exportación de 4 minutos; máximo 720p en plan gratuito
**Planes de pago desde:** $16/mes (Pro — sin marca de agua, 1080p)
**Código abierto:** No

---

## Opciones de Código Abierto / Autoalojables

### Herramientas de Imagen Código Abierto

#### 🔓 Stable Diffusion + ComfyUI / A1111

**URL:** https://github.com/AUTOMATIC1111/stable-diffusion-webui | https://github.com/comfyanonymous/ComfyUI
**Categoría:** Imagen (código abierto, autoalojable)
**Nivel gratuito:** ✅ Completamente gratuito e ilimitado en tu propio hardware. Sin marcas de agua, sin restricciones de contenido más allá de las que configures.
**Requiere tarjeta de crédito:** No
**Acceso a API:** ComfyUI expone una API REST local; puede envolvirse para acceso externo
**Licencia:** Modelos SD: Stability AI Community License (gratuita para individuos y orgs bajo $1M de ingresos); ComfyUI: GNU GPL
**Mejor para:** Cualquier caso de generación de imágenes; fotorrealismo, anime, ilustración, estilos 3D, guía de poses/profundidad con ControlNet, inpainting, outpainting
**Limitaciones:** Requiere GPU capaz (mínimo 6–8 GB VRAM para SDXL); configuración técnica requerida
**Interfaces disponibles:**
- **ComfyUI** — Editor de flujo de trabajo basado en nodos; más avanzado, mejor soporte para FLUX y modelos de video; 10-20% más rápido que A1111
- **Automatic1111 (A1111)** — UI basada en formularios; más amigable para principiantes; ecosistema de extensiones rico
- **SD WebUI Forge** — Fork de A1111; más rápido; añade soporte nativo para FLUX
- **Fooocus** — Interfaz más simple posible; generación con un clic; enfocado en principiantes
- **InvokeAI** — UI de lienzo moderno; excelente inpainting; amigable comercialmente (Apache 2.0)
**Código abierto:** Sí

---

#### 🔓 FLUX.1 (Black Forest Labs) ✅

**URL:** https://github.com/black-forest-labs/flux | https://huggingface.co/black-forest-labs/FLUX.1-schnell
**Categoría:** Imagen (modelo de código abierto)
**Nivel gratuito:** ✅ FLUX.1 [schnell] — Licencia Apache 2.0, completamente gratuito para uso personal, científico y comercial; ejecutar localmente o via endpoints API gratuitos (Together AI ofrece un endpoint FLUX.1 Schnell gratuito). FLUX.1 [dev] — pesos abiertos, solo uso no comercial.
**Requiere tarjeta de crédito:** No
**Acceso a API:** API gratuita via Together AI (FLUX.1 Schnell); API pagada via Black Forest Labs (bfl.ai), Replicate, fal.ai
**Mejor para:** Generación de texto a imagen de alta calidad, prototipado, canalizaciones de producción de imágenes. Notable por su excelente adherencia a prompts y calidad de imagen.
**Limitaciones:** Modelo [dev]: solo no comercial; modelo [pro]: solo API, pagado; ejecución local requiere GPU moderna
**Licencia:** schnell: Apache 2.0 (comercial OK); dev: licencia no comercial; pro: propietario
**Código abierto:** Sí (variante schnell — Apache 2.0)

---

#### 🔓 Stable Diffusion 3.5

**URL:** https://huggingface.co/stabilityai/stable-diffusion-3.5-large
**Categoría:** Imagen (modelo de código abierto)
**Nivel gratuito:** Gratuito para descargar y ejecutar localmente bajo la Stability AI Community License (gratuita para individuos y orgs comerciales bajo $1M/año de ingresos)
**Requiere tarjeta de crédito:** No
**Acceso a API:** Via DreamStudio ($0.065/imagen) o API de la plataforma Stability AI
**Mejor para:** Imágenes fotorrealistas y creativas de última generación; arquitectura MMDiT para mejor renderizado de texto; resolución nativa 1024x1024
**Limitaciones:** Requiere GPU de alta gama localmente (nivel RTX 4090 para mejor rendimiento); sin acceso gratuito continuo en la nube
**Licencia:** Stability AI Community License
**Código abierto:** Sí (pesos del modelo abiertos)

---

#### 🔓 InvokeAI

**URL:** https://invoke.ai | https://github.com/invoke-ai/InvokeAI
**Categoría:** Imagen (UI/plataforma de código abierto)
**Nivel gratuito:** ✅ Completamente gratuito y de código abierto; generación local ilimitada
**Requiere tarjeta de crédito:** No
**Acceso a API:** Sí — expone una API local
**Mejor para:** Flujos de trabajo creativos profesionales, composición basada en lienzo, inpainting, gestión de modelos, ControlNet
**Limitaciones:** Requiere configuración GPU local; configuración inicial más compleja que Fooocus
**Licencia:** Apache 2.0
**Código abierto:** Sí

---

### Herramientas de Video Código Abierto

#### 🔓 Wan 2.1 (Alibaba) ✅

**URL:** https://github.com/Wan-Video/Wan2.1
**Categoría:** Video (modelo de código abierto)
**Nivel gratuito:** ✅ Completamente gratuito para descargar y ejecutar localmente; la variante T2V-1.3B requiere solo 8.19 GB de VRAM (compatible con GPUs de consumidor). Ganó 4,000+ estrellas en GitHub en 2 días tras su lanzamiento.
**Requiere tarjeta de crédito:** No
**Acceso a API:** Ejecución local; también disponible via servicios de inferencia de terceros
**Mejor para:** Texto a video e imagen a video; movimiento limpio y coherente con iluminación consistente y movimiento de cámara estable; hasta ~15 segundos por clip. Los benchmarks muestran que supera a muchas soluciones comerciales.
**Limitaciones:** El modelo más grande (14B) necesita GPU profesional; requiere configuración local
**Licencia:** Apache 2.0
**Código abierto:** Sí (Apache 2.0)

---

#### 🔓 HunyuanVideo (Tencent)

**URL:** https://github.com/Tencent-Hunyuan/HunyuanVideo
**Categoría:** Video (modelo de código abierto)
**Nivel gratuito:** Completamente de código abierto; modelo de 13B parámetros; pesos en Hugging Face; integración con ComfyUI disponible
**Requiere tarjeta de crédito:** No
**Acceso a API:** Via inferencia local; APIs de terceros (Replicate, fal.ai)
**Mejor para:** Generación de video largo de alta calidad; espacio latente espacio-temporal; diseño de transformador "doble flujo a flujo único". Rendimiento comparable a sistemas de código cerrado líderes. Incluye inferencia en GPU única y múltiple, pesos FP8, integraciones con Diffusers y ComfyUI.
**Limitaciones:** 13B parámetros requiere VRAM GPU significativa (se recomiendan 24+ GB para calidad completa)
**Licencia:** Tencent HunyuanVideo Community License
**Código abierto:** Sí

---

#### 🔓 Open-Sora 2.0 (ColossalAI)

**URL:** https://github.com/hpcaitech/Open-Sora
**Categoría:** Video (modelo de código abierto)
**Nivel gratuito:** ✅ Completamente gratuito; modelo de 11B; checkpoints y código de entrenamiento disponibles públicamente; entrenado por solo $200K, siendo un hito en IA de video de código abierto asequible
**Requiere tarjeta de crédito:** No
**Acceso a API:** Sin API alojada; ejecución local o en proveedores de GPU en la nube
**Mejor para:** Generación de video de alta calidad; alcanza rendimiento comparable a HunyuanVideo de 11B y Step-Video de 30B en VBench. Lanzado el 12 de marzo de 2025.
**Limitaciones:** Requiere cómputo sustancial (GPU en la nube o GPU local de alta gama)
**Licencia:** Apache 2.0
**Código abierto:** Sí (totalmente abierto — pesos del modelo, código de entrenamiento, código de inferencia)

---

#### 🔓 CogVideoX (ZhipuAI)

**URL:** https://github.com/zai-org/CogVideo
**Categoría:** Video (modelo de código abierto)
**Nivel gratuito:** Pesos del modelo gratuitos; CogVideoX-5B genera clips de 6 segundos a 720x480 a 8fps; puede ejecutarse en instancias T4 gratuitas de Google Colab
**Requiere tarjeta de crédito:** No
**Acceso a API:** Via plataformas de inferencia de terceros
**Mejor para:** Texto a video e imagen a video; CogVideoX1.5-5B-I2V soporta cualquier resolución para imagen a video; videos de 10 segundos a mayor resolución en la última versión
**Limitaciones:** El T4 gratuito de Colab tiene límites de VRAM; los videos más largos necesitan hardware más potente
**Licencia:** Apache 2.0
**Código abierto:** Sí

---

#### 🔓 LTX-Video / LTX-2 (Lightricks)

**URL:** https://github.com/Lightricks/LTX-Video
**Categoría:** Video (modelo de código abierto)
**Nivel gratuito:** Gratuito para ejecutar localmente; notable por ser uno de los modelos de video de código abierto más rápidos — genera video a 30fps a 1216x704 más rápido que en tiempo real en hardware capaz. Integración con ComfyUI disponible.
**Requiere tarjeta de crédito:** No
**Acceso a API:** Inferencia local; nodos ComfyUI
**Mejor para:** Texto a video rápido de alta calidad; LTX-2 añade generación sincronizada de audio+video — el primer modelo de fundación audio-video basado en DiT. Soporta hasta 60 segundos de video.
**Limitaciones:** Requiere buena GPU
**Licencia:** OpenRail (abierto para uso académico y comercial; los derivados deben permanecer abiertos)
**Código abierto:** Sí

---

#### 🔓 AnimateDiff

**URL:** https://github.com/guoyww/AnimateDiff
**Categoría:** Video (módulo de movimiento de código abierto para Stable Diffusion)
**Nivel gratuito:** ✅ Completamente gratuito; se conecta a checkpoints de generación de imágenes de Stable Diffusion existentes
**Requiere tarjeta de crédito:** No
**Acceso a API:** Via API local de ComfyUI/A1111
**Mejor para:** Añadir movimiento/animación a imágenes de Stable Diffusion; funciona con LoRAs y checkpoints SD existentes
**Limitaciones:** Duración de clip corta (típicamente 2–4 segundos); la calidad depende del modelo base
**Licencia:** Apache 2.0
**Código abierto:** Sí

---

## Acceso Rápido por Caso de Uso

### Generar imágenes sin registrarse
- [Craiyon](https://www.craiyon.com) — Ilimitadas, sin cuenta
- [Raphael AI](https://raphael.app) — Ilimitadas, sin cuenta

### Imágenes gratuitas de alta calidad (con cuenta)
- [Bing Image Creator](https://www.bing.com/images/create) — Efectivamente ilimitadas (solo más lentas)
- [Freepik IA](https://www.freepik.com/ai/image-generator) — 20/día, buena calidad
- [Leonardo.AI](https://leonardo.ai) — 30–75/día con muchos modelos

### Texto en imágenes (logos, carteles)
- [Ideogram](https://ideogram.ai) — El mejor en coherencia tipográfica
- [Adobe Firefly](https://firefly.adobe.com) — Calidad comercial, 25/mes gratis

### Imágenes comercialmente seguras
- [Adobe Firefly](https://firefly.adobe.com) — Entrenado con contenido licenciado
- [FLUX.1 Schnell](https://github.com/black-forest-labs/flux) — Apache 2.0, uso comercial libre

### Videos gratuitos con recarga diaria
- [Kling AI](https://klingai.com) — 66 créditos/día (el más generoso con recarga diaria)
- [PixVerse](https://app.pixverse.ai) — 60 créditos/día

### Videos con avatares IA
- [Synthesia](https://www.synthesia.io) — 10 min/mes, 1080p, 160+ idiomas
- [HeyGen](https://www.heygen.com) — 1 min gratis, fuerte en traducción con lip sync

### Generación local sin límites (requiere GPU)
- [ComfyUI + FLUX.1 Schnell](https://github.com/comfyanonymous/ComfyUI) — Imágenes ilimitadas
- [Wan 2.1](https://github.com/Wan-Video/Wan2.1) — Videos ilimitados, Apache 2.0, 8GB VRAM mínimo

### Edición de video con IA
- [Kapwing](https://www.kapwing.com) — Subtítulos automáticos, Smart Cut, formato libre
- [InVideo AI](https://invideo.io) — Script a video completo

### Estudiantes / Educación
- **Adobe Firefly** — Adobe ofrece descuentos educativos en Creative Cloud (que incluye más créditos de Firefly)
- **Canva** — Plan Canva for Education completamente gratuito para educadores y estudiantes, incluye créditos IA
- **GitHub Student Pack** — Incluye créditos en varias plataformas de IA (verificar lista actualizada)

---

## Notas Importantes

> ⚠️ **OpenAI Sora** eliminó su nivel gratuito el 10 de enero de 2026. Ahora requiere ChatGPT Plus ($20/mes) o Pro ($200/mes).

> ⚠️ **Midjourney** no tiene prueba gratuita desde abril de 2023. El plan más económico es $10/mes.

> ✅ **Meta AI** usa tecnología similar a Midjourney de forma gratuita sin límites de generación (disponible en WhatsApp, Instagram, Facebook y meta.ai).

---

*Última actualización: 2026-03-06*
*Verificado con fuentes oficiales y directorios de herramientas IA actualizados (2025–2026)*
