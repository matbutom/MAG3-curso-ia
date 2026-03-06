# Cheatsheet: Herramientas IA Gratuitas — Imágenes y Video

> Referencia rápida. Para detalles completos ver [AI_RESOURCES.md](./AI_RESOURCES.md).
> **✅** = Especialmente generoso | **⚠️** = Muy limitado | **🔓** = Código abierto

---

## Generación de Imágenes

| Herramienta | URL | Gratis | CC | Nota |
|---|---|---|---|---|
| ✅ Bing Image Creator | https://www.bing.com/images/create | Ilimitadas (lentas) | No | Sin marca de agua. Mejor opción gratuita general. |
| ✅ Craiyon | https://www.craiyon.com | Ilimitadas, sin cuenta | No | 9 variaciones por prompt. Sin registro. |
| ✅ Raphael AI | https://raphael.app | Ilimitadas | No | Sin límites ni tarifas ocultas. |
| ✅ Freepik IA | https://www.freepik.com/ai/image-generator | 20/día | No | Modelos FLUX + Mystic. Con API pagada. |
| Leonardo.AI | https://leonardo.ai | ~30–75/día | No | 150 tokens/día. Imágenes públicas en gratis. |
| Google Gemini Flash | https://aistudio.google.com | 500/día (API) | No | API gratuita para desarrolladores. |
| Adobe Firefly | https://firefly.adobe.com | 25/mes | No | Comercialmente seguro. Sin marca de agua. |
| NightCafe | https://nightcafe.studio | 5/día + bonos | No | Más modelos que ninguna otra plataforma. |
| Ideogram | https://ideogram.ai | Créditos semanales | No | El mejor para texto en imágenes. |
| ⚠️ DreamStudio | https://dreamstudio.stability.ai | 200 créditos únicos | No | Solo para probar Stable Diffusion oficial. |
| ⚠️ Playground AI | https://playground.com | 10 cada 3h | No | Muy limitado para uso serio. |
| ⚠️ Canva IA | https://www.canva.com/ai-image-generator/ | 50 de por vida | No | Integrado en Canva. Educación: gratuito ilimitado. |
| 🔓 FLUX.1 Schnell | https://github.com/black-forest-labs/flux | Ilimitadas (local) | No | Apache 2.0. También API gratis via Together AI. |
| 🔓 Stable Diffusion + ComfyUI | https://github.com/comfyanonymous/ComfyUI | Ilimitadas (local) | No | Requiere GPU 6-8 GB VRAM mínimo. |
| 🔓 InvokeAI | https://github.com/invoke-ai/InvokeAI | Ilimitadas (local) | No | Apache 2.0. UI de lienzo profesional. |

---

## Generación de Video

| Herramienta | URL | Gratis | CC | Nota |
|---|---|---|---|---|
| ✅ Kling AI | https://klingai.com | 66 créditos/día | No | La recarga diaria más generosa. 720p con marca de agua. |
| ✅ PixVerse | https://app.pixverse.ai | 60 créditos/día | No | 540p. Efectos virales, lip sync. API disponible. |
| Luma AI | https://lumalabs.ai | 30/mes | No | Calidad cinematográfica. Resolución borrador en gratis. |
| ⚠️ Runway Gen-4 | https://runwayml.com | 125 créditos únicos | No | Top de benchmarks. Marca de agua. Sin recarga. |
| ⚠️ Pika 2.2 | https://pika.art | 80 créditos únicos | No | Marca de agua. Sin uso comercial en gratis. |
| ⚠️ Hailuo AI | https://hailuoai.video | 70 únicos (expiran 3d) | No | MiniMax Video-01. Caducan rápido. |
| Synthesia | https://www.synthesia.io | 10 min/mes | No | Avatares IA. 1080p. 160+ idiomas. |
| ⚠️ HeyGen | https://www.heygen.com | 1 min total | No | Lip sync multilingüe. Muy limitado en gratis. |
| ⚠️ Fliki | https://fliki.ai | 5 min/mes | No | Blog/script a video con voz IA. |
| ⚠️ InVideo AI | https://invideo.io | 2 min/semana | No | Script a video completo. |
| Kapwing | https://www.kapwing.com | Ilimitado (4 min/export) | No | Editor IA. Subtítulos, Smart Cut. Sin generación pura. |
| 🔓 Wan 2.1 | https://github.com/Wan-Video/Wan2.1 | Ilimitadas (local) | No | Apache 2.0. Mejor calidad/accesibilidad. 8GB VRAM mínimo. |
| 🔓 HunyuanVideo | https://github.com/Tencent-Hunyuan/HunyuanVideo | Ilimitadas (local) | No | 13B params. Alta calidad. Requiere 24GB VRAM. |
| 🔓 Open-Sora 2.0 | https://github.com/hpcaitech/Open-Sora | Ilimitadas (local) | No | Apache 2.0. 11B params. Código de entrenamiento incluido. |
| 🔓 LTX-Video | https://github.com/Lightricks/LTX-Video | Ilimitadas (local) | No | El más rápido (más rápido que tiempo real). Hasta 60s. |
| 🔓 CogVideoX | https://github.com/zai-org/CogVideo | Ilimitadas (local) | No | Apache 2.0. Corre en Google Colab T4 gratuito. |
| 🔓 AnimateDiff | https://github.com/guoyww/AnimateDiff | Ilimitadas (local) | No | Añade movimiento a imágenes SD. Clips cortos (2-4s). |

---

## Guía de Decisión Rápida

```
¿Necesito imágenes SIN registrarme?
  → Craiyon | Raphael AI

¿Necesito imágenes gratuitas diarias (con cuenta)?
  → Bing Image Creator (ilimitadas lentas) | Freepik (20/día) | Leonardo.AI (30-75/día)

¿Necesito texto legible dentro de imágenes?
  → Ideogram

¿Necesito imágenes comercialmente seguras (sin preocuparme por licencias)?
  → Adobe Firefly | FLUX.1 Schnell (Apache 2.0)

¿Necesito videos gratuitos con recarga diaria?
  → Kling AI (66/día) | PixVerse (60/día)

¿Necesito videos con avatares IA?
  → Synthesia (10 min/mes) | HeyGen (1 min total)

¿Quiero generación local sin límites (tengo GPU)?
  → Imágenes: ComfyUI + FLUX.1 Schnell
  → Videos: Wan 2.1 (8GB VRAM) | LTX-Video (más rápido)

¿Soy estudiante/educador?
  → Canva Education (gratuito completo) | Adobe CC Education (descuento)
```

---

*Última actualización: 2026-03-06 | Ver [AI_RESOURCES.md](./AI_RESOURCES.md) para detalles completos*
