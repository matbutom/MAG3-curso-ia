# Stable Diffusion — Recursos y Guía de Uso

> Recursos gratuitos y de prueba gratuita para ejecutar, aprender y aprovechar al máximo Stable Diffusion.
> **Leyenda:** ✅ Gratuito sin tarjeta de crédito | ⚠️ Nivel gratuito muy limitado | 🖥️ Requiere GPU local

*Última actualización: 2026-03-06*

---

## Tabla de Contenidos

1. [Inicio Rápido](#1-inicio-rápido)
2. [Plataformas en la Nube](#2-plataformas-en-la-nube-sin-gpu-local)
3. [Opciones de Instalación Local](#3-opciones-de-instalación-local)
4. [Repositorios de Modelos](#4-repositorios-de-modelos)
5. [Técnicas Principales y Cómo Usarlas](#5-técnicas-principales-y-cómo-usarlas)
6. [Guía de Prompt Engineering](#6-guía-de-prompt-engineering)
7. [Extensiones y Plugins](#7-extensiones-y-plugins)
8. [Recursos de Aprendizaje y Comunidades](#8-recursos-de-aprendizaje-y-comunidades)

---

## 1. Inicio Rápido

**¿Quieres probar Stable Diffusion ahora mismo, sin instalar nada?**

### Ruta para principiantes absolutos (5 minutos)

| Paso | Opción | Por qué |
|------|--------|---------|
| **Sin cuenta** | [Dezgo](https://dezgo.com) | Solo escribes y generas. Sin registro. FLUX y SDXL gratis. |
| **Con cuenta gratuita** | [SeaArt](https://www.seaart.ai) o [Tensor.Art](https://tensor.art) | Más modelos, más control, créditos diarios gratuitos. |
| **Con GPU propia** | [Stability Matrix](https://lykos.ai) | Instala ComfyUI, Forge, A1111 con un clic. Sin conflictos. |

### ¿Qué versión de SD debo usar?

| Modelo | Cuándo usarlo |
|--------|--------------|
| **SD 1.5** | Tienes GPU de 4-6 GB VRAM. Ecosistema enorme de LoRAs. |
| **SDXL** | Tienes 8+ GB VRAM. Mejor calidad, prompts más naturales. |
| **FLUX.1** | Tienes 8-16 GB VRAM. La mejor calidad fotorrealista en 2025-2026. Apache 2.0 (variante schnell). |
| **SD3.5** | Alternativa a FLUX. Mejor en texto dentro de imágenes. |

### Guía de hardware rápida

| VRAM de GPU | ¿Qué puedes ejecutar? |
|-------------|----------------------|
| 4 GB | SD1.5 (normal), SDXL con lowvram, Fooocus |
| 6 GB | SD1.5, SDXL cómodo, FLUX cuantizado (NF4/GGUF) |
| 8 GB | SD1.5, SDXL cómodo, FLUX.1 Dev (con optimización) |
| 12 GB | Todo lo anterior + FLUX.1 cómodamente |
| 16 GB+ | FLUX.1 calidad completa, SD3.5 Large, modelos de video |
| 24 GB+ | FLUX.2, múltiples modelos cargados, procesamiento por lotes |

---

## 2. Plataformas en la Nube (Sin GPU Local)

### ✅ Dezgo

- **URL:** https://dezgo.com
- **Nivel gratuito:** Completamente gratuito. Sin cuenta ni registro.
- **Requiere GPU localmente:** No
- **Dificultad:** Principiante
- **Mejor para:** Probar Stable Diffusion en 30 segundos, generar imágenes rápidas sin compromisos.
- **Cómo empezar:** Entra a la web, escribe tu prompt en inglés, selecciona FLUX o SDXL y haz clic en "Generate". Listo.
- **Limitaciones:** Sin opciones avanzadas; sin historial de imágenes; lento en horas pico.
- **Nota:** Es el frontend simplificado de getimg.ai. Sin marca de agua.

---

### ✅ SeaArt

- **URL:** https://www.seaart.ai
- **Nivel gratuito:** Créditos diarios gratuitos generosos. Sin tarjeta de crédito.
- **Requiere GPU localmente:** No
- **Dificultad:** Principiante
- **Mejor para:** Explorar 300,000+ modelos comunitarios, probar LoRAs y ControlNet en el navegador.
- **Cómo empezar:** Crea cuenta gratuita → elige un modelo de la galería → completa el prompt → genera. También soporta flujos de trabajo estilo ComfyUI.
- **Limitaciones:** Los créditos gratuitos se agotan; funciones avanzadas requieren créditos extra.
- **Modelos compatibles:** SD 1.5, SDXL, SD3, SD3.5, FLUX.1.

---

### ✅ Tensor.Art

- **URL:** https://tensor.art
- **Nivel gratuito:** Generación gratuita con créditos diarios; repositorio de modelos para compartir.
- **Requiere GPU localmente:** No
- **Dificultad:** Principiante
- **Mejor para:** Generar imágenes en el navegador Y descargar modelos comunitarios (similar a Civitai).
- **Cómo empezar:** Crea cuenta → selecciona un modelo (SDXL, SD1.5, SD3, etc.) → genera directamente en el sitio o descarga el modelo para uso local.
- **Limitaciones:** La generación avanzada y el entrenamiento de modelos son de pago.
- **Modelos compatibles:** SD 1.5, SDXL 1.0, SD3, HunyuanDiT y más.

---

### ✅ OpenArt

- **URL:** https://openart.ai
- **Nivel gratuito:** Algunas generaciones diarias gratuitas con cuenta.
- **Requiere GPU localmente:** No
- **Dificultad:** Principiante
- **Mejor para:** Generación de referencia ("haz una imagen con este estilo"), upscaling (modos Creativo y Preciso), explorar el Prompt Book.
- **Cómo empezar:** Crea cuenta gratuita → elige modelo → usa "Image Reference" para subir una imagen de estilo → genera.
- **Limitaciones:** Generaciones gratuitas limitadas por día.
- **Recurso extra:** [Prompt Book de OpenArt](https://openart.ai/promptbook) — guía visual de prompts por categoría.

---

### ⚠️ DreamStudio (Stability AI)

- **URL:** https://dreamstudio.stability.ai
- **Nivel gratuito:** 200 créditos únicos al registrarse (~25 imágenes básicas). Sin recarga.
- **Requiere GPU localmente:** No
- **Dificultad:** Principiante
- **Mejor para:** Probar los modelos oficiales de Stability AI (SDXL, SD3, SD3.5) en su implementación de referencia.
- **Cómo empezar:** Crea cuenta → escribe prompt → ajusta modelo, resolución y pasos → genera.
- **Limitaciones:** Los créditos son únicos (no se recargan). Cada imagen de SD3.5 Large cuesta ~8 créditos. Para uso continuo se requiere pago.

---

### ✅ Google Colab (via Hugging Face Diffusers)

- **URL:** https://colab.research.google.com
- **Notebook oficial:** https://colab.research.google.com/github/huggingface/notebooks/blob/main/diffusers/stable_diffusion.ipynb
- **Nivel gratuito:** GPU T4 (~15 GB VRAM), 12 GB RAM sistema, 78 GB disco. Sesiones de hasta 12h.
- **Requiere GPU localmente:** No (usa la GPU de Google)
- **Dificultad:** Intermedio
- **Mejor para:** Experimentación con código Python, pruebas de modelos nuevos, entrenamiento ligero.
- **Cómo empezar:** Abre el notebook → Entorno de ejecución → Cambiar tipo de entorno de ejecución → GPU T4 → ejecuta celdas en orden.
- **Limitaciones:** Google bloqueó AUTOMATIC1111 en el nivel gratuito (solo funciona el notebook de Diffusers). Las sesiones se desconectan por inactividad. Colab Pro (~$10/mes) desbloquea A1111 y tiempos de sesión más largos.

---

### ✅ Kaggle Notebooks

- **URL:** https://www.kaggle.com
- **Nivel gratuito:** **30 horas semanales de GPU gratuita** (NVIDIA T4 x2 o P100). Sesiones de hasta 12h. Se reinicia cada semana.
- **Requiere GPU localmente:** No
- **Dificultad:** Intermedio
- **Mejor para:** Entrenamiento de LoRAs gratis (via Kohya SS), inferencia de SDXL, proyectos que requieren más tiempo que Colab.
- **Cómo empezar:** Crea cuenta → New Notebook → Settings → Accelerator: GPU P100 → ejecuta tu notebook de SD.
- **Limitaciones:** Requiere conocimiento básico de Jupyter; no tan inmediato como plataformas web.
- **Guía de entrenamiento LoRA:** https://civitai.com/articles/2090

---

### Massed Compute (GPU en la nube)

- **URL:** https://massedcompute.com
- **Nivel gratuito:** Sin nivel gratuito — pago por uso (alquiler de GPU por horas).
- **Requiere GPU localmente:** No (acceso remoto via ThinLinc)
- **Dificultad:** Intermedio
- **Mejor para:** Acceder a GPUs de alta gama (RTX 3090/4090) sin hardware propio, para generación intensiva o entrenamiento.
- **Cómo empezar:** Crea cuenta → selecciona GPU → accede via escritorio remoto → instala Forge Classic, ComfyUI u otro UI en el entorno ya configurado.
- **Limitaciones:** Es de pago (aunque más barato que comprar GPU propia para uso ocasional).

---

## 3. Opciones de Instalación Local

> Todas las opciones de esta sección son **completamente gratuitas** y de código abierto. Solo necesitas una GPU compatible.

---

### ✅ 🖥️ Stability Matrix (Gestor de instalación)

- **URL:** https://lykos.ai
- **GitHub:** https://github.com/LykosAI/StabilityMatrix
- **Nivel gratuito:** Completamente gratuito. Código abierto.
- **Requiere GPU localmente:** Sí (la necesitan los UIs que instala)
- **Dificultad:** **Principiante** — la forma más fácil de empezar localmente
- **Mejor para:** Instalar y gestionar múltiples UIs (A1111, ComfyUI, Forge, InvokeAI) sin conflictos de dependencias.
- **Cómo empezar:** Descarga el instalador para Windows/Mac/Linux → ejecuta → elige los UIs que quieres → Stability Matrix los instala con todas las dependencias → carpeta de modelos compartida entre todos los UIs.
- **Limitaciones:** Es un gestor, no un UI propiamente. Necesitas instalar algún UI a través de él.
- **SD compatibles:** Todos los que soporten los UIs instalados.

---

### ✅ 🖥️ SD WebUI Forge (Recomendado para empezar)

- **GitHub (fork activo):** https://github.com/Haoming02/sd-webui-forge-classic (Forge Classic)
- **Fork alternativo:** https://github.com/Panchovix/stable-diffusion-webui-reForge
- **Nivel gratuito:** Completamente gratuito.
- **VRAM mínima:** 2 GB (SD1.5) / 4 GB (SDXL) / 6 GB (FLUX cuantizado NF4)
- **Dificultad:** **Intermedio** — interfaz casi idéntica a A1111, pero con mejor rendimiento
- **Mejor para:** Usuarios que vienen de A1111 y quieren más velocidad; soporte completo de FLUX con poca VRAM.
- **Cómo empezar:** Descarga via Stability Matrix o clona el repo → ejecuta `run.bat` (Windows) o `run.sh` (Linux/Mac) → abre `localhost:7860` en tu navegador.
- **Ventajas sobre A1111:** 30-75% más rápido; mejor gestión de VRAM; soporte nativo FLUX con "GPU weight slider"; compatible con la mayoría de extensiones de A1111.
- **SD compatibles:** SD 1.5, SDXL, FLUX.1 (Dev/Schnell, BNB NF4/GGUF), SD3.5 (limitado).

---

### ✅ 🖥️ AUTOMATIC1111 (A1111 / SD WebUI)

- **GitHub:** https://github.com/AUTOMATIC1111/stable-diffusion-webui
- **Nivel gratuito:** Completamente gratuito.
- **VRAM mínima:** 4 GB (`--lowvram`, lento) / 8 GB recomendado para SDXL
- **Dificultad:** **Intermedio** — UI por pestañas, configuración compleja pero accesible
- **Mejor para:** El mayor ecosistema de extensiones; la mayoría de tutoriales hacen referencia a A1111; inpainting, hires fix, scripts.
- **Cómo empezar:** Instala Python 3.10 + Git → clona el repo → ejecuta `webui.bat` (Windows) o `webui.sh` (Linux) → primer inicio descarga los modelos automáticamente.
- **Limitaciones:** 30-50% más lento que Forge o ComfyUI; soporte FLUX pobre; GPUs 50-series de NVIDIA requieren branch de desarrollo.
- **SD compatibles:** SD 1.4, SD 1.5, SD 2.x, SDXL (FLUX limitado).
- **Wiki oficial:** https://github.com/AUTOMATIC1111/stable-diffusion-webui/wiki/features

---

### ✅ 🖥️ ComfyUI (Para usuarios avanzados)

- **GitHub:** https://github.com/comfyanonymous/ComfyUI
- **Documentación:** https://docs.comfy.org
- **Nivel gratuito:** Completamente gratuito. El más activamente desarrollado (versiones estables semanales).
- **VRAM mínima:** 4 GB (SD1.5 práctica) / 6-8 GB (SDXL) / 8 GB (FLUX básico) / 16 GB (FLUX óptimo)
- **RAM sistema:** 16 GB mínimo recomendado para FLUX (32 GB óptimo)
- **Plataformas:** NVIDIA (CUDA), AMD (ROCm en Linux), Intel, Apple Silicon (M1/M2/M3/M4 via MPS)
- **Dificultad:** **Avanzado** — interfaz de nodos (espera semanas para dominarlo)
- **Mejor para:** Los modelos nuevos siempre llegan a ComfyUI primero; flujos de trabajo reproducibles y compartibles; máximo control sobre el pipeline.
- **Cómo empezar:** Instala via Stability Matrix (recomendado) o clona el repo → ejecuta `run_nvidia_gpu.bat` → instala ComfyUI Manager (ver Extensiones) → descarga un workflow básico de la comunidad.
- **Ventajas:** 2x más rápido que A1111; flujos de trabajo en JSON compartibles; soporte de todos los modelos actuales (FLUX.2, video, etc.).
- **SD compatibles:** SD 1.x, SD 2.x, SDXL, SD3, SD3.5, FLUX.1, FLUX.2, modelos de video (Wan, HunyuanVideo).

---

### ✅ 🖥️ InvokeAI

- **GitHub:** https://github.com/invoke-ai/InvokeAI
- **Documentación:** https://invoke-ai.github.io/InvokeAI/
- **Nivel gratuito:** Completamente gratuito. Licencia Apache 2.0.
- **VRAM mínima:** 4 GB / Funciona en Mac Apple Silicon, Windows, Linux
- **Dificultad:** **Principiante a Intermedio** — la UI más pulida y profesional con enfoque en lienzo
- **Mejor para:** Flujos de trabajo creativos profesionales; inpainting avanzado con lienzo unificado; usuarios que quieren una experiencia limpia sin complejidad de nodos.
- **Cómo empezar:** Instala via Stability Matrix o descarga el instalador desde GitHub → ejecuta → abre `localhost:9090` → descarga modelos desde la interfaz de gestión de modelos integrada.
- **Limitaciones:** Ecosistema de extensiones más pequeño que A1111/ComfyUI.
- **SD compatibles:** SD 1.5, SDXL, FLUX, SD3.

---

### ✅ 🖥️ Fooocus

- **GitHub:** https://github.com/lllyasviel/Fooocus
- **Nivel gratuito:** Completamente gratuito.
- **VRAM mínima:** 4 GB NVIDIA / 8 GB RAM sistema
- **Dificultad:** **Principiante** — el más simple de todos los UIs locales
- **Mejor para:** Principiantes que quieren resultados tipo Midjourney sin configuración compleja.
- **Cómo empezar:** Descarga el zip de releases → ejecuta `run.bat` → descarga automáticamente los modelos SDXL → escribe tu prompt → genera. Sin configuración adicional.
- **Limitaciones:** Solo SDXL (sin FLUX en el original); sin extensiones; personalización muy limitada; desarrollo original ralentizado.
- **SD compatibles:** SDXL (principalmente).

---

### ✅ 🖥️ SwarmUI

- **GitHub:** https://github.com/mcmonkeyprojects/SwarmUI
- **Nivel gratuito:** Completamente gratuito.
- **VRAM mínima:** Similar a ComfyUI (usa ComfyUI como backend)
- **Dificultad:** **Intermedio** — más simple que ComfyUI pero más potente que Fooocus
- **Mejor para:** Usuarios que quieren la potencia de ComfyUI con una interfaz más accesible; generación de video con Wan y HunyuanVideo.
- **Cómo empezar:** Descarga el instalador → ejecuta el script de instalación de un solo clic (Windows/Linux/Mac/Docker) → elige los paquetes que necesitas → abre la UI.
- **Limitaciones:** Comunidad más pequeña; menos tutoriales disponibles.
- **SD compatibles:** SDXL, FLUX, LTX-Video, HunyuanVideo.

---

## 4. Repositorios de Modelos

> Los modelos son los archivos `.safetensors` o `.ckpt` que definen el estilo y capacidades del generador. Descárgalos y colócalos en la carpeta `models/` del UI que uses.

---

### ✅ Civitai (El más grande)

- **URL:** https://civitai.com
- **Hub de educación:** https://education.civitai.com
- **Qué tiene:** Millones de modelos comunitarios — checkpoints, LoRAs, embeddings, LyCORIS, VAEs, upscalers, wildcards.
- **Filtros clave:** Tipo de modelo, versión base (SD1.5, SDXL, Pony, FLUX, Illustrious), SFW/NSFW.
- **Generación online:** Genera directamente con cualquier modelo en el navegador (usa créditos "Buzz").
- **Entrenamiento online:** Entrena LoRAs en la plataforma (SD1.5: 500 Buzz, SDXL: 500 Buzz, FLUX: 2000 Buzz).
- **Cómo usar un modelo descargado:**
  1. Descarga el `.safetensors` del modelo
  2. Colócalo en `models/Stable-diffusion/` (A1111/Forge) o `models/checkpoints/` (ComfyUI)
  3. Recarga la interfaz → selecciona el modelo en el menú desplegable
- **Nota:** Algunos modelos son NSFW por defecto — requiere cuenta verificada por edad para verlos.

---

### ✅ Hugging Face

- **URL:** https://huggingface.co/models?other=stable-diffusion
- **Qué tiene:** El hub de ML más grande. Aloja los modelos oficiales de Stability AI y Black Forest Labs.
- **Modelos oficiales clave:**
  - SD 1.5: `stable-diffusion-v1-5/stable-diffusion-v1-5`
  - SDXL 1.0: `stabilityai/stable-diffusion-xl-base-1.0`
  - SD3.5 Large: `stabilityai/stable-diffusion-3.5-large`
  - FLUX.1 Dev: `black-forest-labs/FLUX.1-dev`
  - FLUX.1 Schnell (Apache 2.0): `black-forest-labs/FLUX.1-schnell`
  - FLUX.2 Dev: `black-forest-labs/FLUX.2-dev`
- **Demos gratuitas en el navegador (Spaces):**
  - SD3 Medium: https://huggingface.co/spaces/stabilityai/stable-diffusion-3-medium
- **Formatos:** Los modelos se distribuyen en formato `.safetensors` (más seguro) o formato `diffusers` (para Python).
- **Dificultad:** Intermedio — requiere entender formatos de modelos.

---

### ✅ Tensor.Art (Modelos + Generación)

- **URL:** https://tensor.art/models
- **Qué tiene:** Repositorio comunitario similar a Civitai con miles de uploads. Permite también generar directamente en el navegador con los modelos.
- **Modelos:** SD 1.5, SDXL, FLUX y más.
- **Ideal para:** Encontrar modelos alternativos a los de Civitai, con generación integrada para probar antes de descargar.

---

### ✅ Recursos de Prompts (Inspiración)

| Plataforma | URL | Para qué |
|---|---|---|
| **Lexica.art** | https://lexica.art | 10M+ imágenes con prompts visibles. Busca por estilo y copia el prompt exacto. |
| **PromptHero** | https://prompthero.com | Galería de prompts con generador integrado. |
| **Krea.ai** | https://www.krea.ai | Búsqueda visual — arrastra una imagen y encuentra prompts similares. Generación en tiempo real. |
| **OpenArt Prompt Book** | https://openart.ai/promptbook | Guía visual curada por categorías. |

---

## 5. Técnicas Principales y Cómo Usarlas

---

### txt2img (Texto a Imagen)

**Qué hace:** La función principal. Partes de ruido aleatorio y el modelo lo va "desruidando" en pasos iterativos guiado por tu prompt de texto hasta producir una imagen.

**Parámetros clave:**
- **Prompt:** Descripción de lo que quieres generar
- **Negative Prompt:** Lo que quieres evitar
- **Resolution:** Usa la resolución nativa del modelo (512×512 para SD1.5, 1024×1024 para SDXL)
- **Steps:** Número de iteraciones (20-30 es el punto óptimo calidad/velocidad)
- **CFG Scale:** Qué tan estrictamente sigue el prompt (ver sección de CFG)
- **Sampler:** Algoritmo de denoising (ver sección de Samplers)
- **Seed:** Número que fija el resultado (-1 para aleatorio)

**Consejo importante:** Generar SDXL fuera de 1024×1024 causa problemas de calidad. Si quieres otro tamaño, genera a 1024×1024 y usa HiRes Fix para escalar.

**Herramientas gratuitas que lo soportan:** Todas (Dezgo, SeaArt, A1111, ComfyUI, Forge, etc.)

---

### img2img (Imagen a Imagen)

**Qué hace:** Tomas una imagen existente + un prompt de texto. El pipeline añade ruido a la imagen de entrada (controlado por **Denoising Strength**) y luego la "desruida" usando el prompt como guía. Permite transformar, reestilizar o mejorar imágenes existentes.

**Parámetro clave — Denoising Strength (0.0 a 1.0):**

| Valor | Comportamiento |
|-------|---------------|
| 0.0 | Salida idéntica a la entrada (sin cambio) |
| 0.3–0.5 | Preserva la estructura + aplica estilo del prompt |
| 0.6–0.75 | Mezcla equilibrada: estructura + influencia del prompt |
| 1.0 | Esencialmente txt2img (ignora la imagen) |

**Casos de uso:** Transferencia de estilo, corrección de colores, boceto a render, edición de fotos.

**Consejos:**
- Empieza con 0.5 y ajusta según necesites más o menos cambio
- Para cambios de estilo conservando composición: 0.4–0.6
- Para reinterpretación completa: 0.7–0.85

**Herramientas gratuitas:** A1111, Forge, ComfyUI, InvokeAI, SeaArt, getimg.ai

---

### Inpainting (Pintura Interior)

**Qué hace:** Edición selectiva de regiones. Dibujas una máscara sobre la parte de la imagen que quieres cambiar. El área con máscara se regenera siguiendo el prompt, mientras el área sin máscara permanece intacta.

**Cómo usarlo en A1111/Forge:**
1. Ve a la pestaña "img2img" → sub-pestaña "Inpaint"
2. Sube la imagen
3. Pinta la máscara sobre el área a cambiar (herramienta de pincel)
4. Escribe el prompt describiendo QUÉ quieres en esa área
5. Ajusta Denoising Strength (0.7–0.85 para cambios fuertes, 0.4–0.6 para integración suave)

**Consejos:**
- Usa checkpoints específicos de inpainting (marcados como "inpainting" en Civitai)
- El "Mask Blur" ayuda a mezclar los bordes naturalmente (valor 4–8)
- Describe solo el contenido del área con máscara en el prompt

**Casos de uso:** Arreglar caras/manos, eliminar objetos, añadir/reemplazar elementos.

**Herramientas gratuitas:** A1111, Forge, ComfyUI (node: InpaintModelConditioning), InvokeAI (excelente canvas), SeaArt, getimg.ai

---

### Outpainting (Pintura Exterior)

**Qué hace:** Extiende una imagen más allá de sus bordes originales. El modelo genera contenido nuevo que es contextualmente consistente con la imagen original.

**Cómo usarlo en A1111:**
1. img2img → "Inpaint sketch" o usa el script "Outpainting mk2"
2. Aumenta el tamaño del lienzo (por ejemplo: de 512×512 a 768×512 para añadir a la derecha)
3. Pinta la máscara en la zona nueva (vacía)
4. Prompt describiendo la escena completa

**Mejores configuraciones:**
- Steps altos: 50–100
- Denoising Strength alta: 0.85–1.0
- Samplers: Euler Ancestral o DPM++ SDE

**Casos de uso:** Ampliar el encuadre de una foto, crear panorámicas, adaptar formato vertical/horizontal.

**Herramientas gratuitas:** A1111, InvokeAI (el mejor canvas para outpainting), ComfyUI

---

### ControlNet

**Qué hace:** Red neuronal adicional que añade condicionamiento espacial a la generación. Además del texto, ControlNet usa una imagen de control (mapa de profundidad, esqueleto de pose, mapa de bordes, etc.) para guiar con precisión la composición.

**Cómo funciona:** Se adjunta a la U-Net del modelo. Toma una imagen de control como entrada secundaria, aplica un preprocesador (ej: detector de bordes Canny) y usa el resultado para restringir la generación.

**Tipos principales de ControlNet:**

| Tipo | Preprocesador | Para qué |
|------|--------------|---------|
| **Canny** | Detector de bordes | Preservar contornos de una imagen de referencia |
| **Depth** | Estimación de profundidad MiDaS | Preservar perspectiva 3D y distancias espaciales |
| **OpenPose** | Detección de esqueleto corporal | Copiar poses humanas (manos, cabeza, extremidades) |
| **Lineart** | Extracción de líneas | Transferir estructura de bocetos o arte lineal |
| **Softedge (HED)** | Bordes suaves | Preservación suave de contornos |
| **Scribble** | Manual o automático | Generar desde bocetos aproximados |
| **Tile** | Mosaico | Upscaling tile a tile con alta coherencia |
| **IP-Adapter** | Características CLIP | Consistencia de estilo/personaje con imagen de referencia |

**Cómo instalar en A1111/Forge:**
1. Extensions → Install from URL → pega: `https://github.com/Mikubill/sd-webui-controlnet`
2. Descarga los modelos ControlNet correspondientes (A1111 los muestra en la interfaz)
3. Coloca los modelos en `models/ControlNet/`
4. En txt2img/img2img → sección ControlNet → activa → sube imagen → selecciona preprocesador y modelo → genera

**Versiones disponibles:**
- ControlNet v1.1 para SD1.5 — más maduro, mayor variedad de modelos
- ControlNet para SDXL — disponible pero menos modelos
- ControlNets para SD3.5 Large — Stability AI publicó Blur, Canny y Depth en 2025

**Herramientas gratuitas:** A1111 (extensión), Forge (extensión), ComfyUI (nodos nativos), InvokeAI, SeaArt

---

### LoRA (Low-Rank Adaptation)

**Qué hace:** Archivos de ajuste fino ligeros (típicamente 10-300 MB vs. 2-7 GB de un checkpoint completo) que añaden o modifican conceptos, estilos, personajes o técnicas específicas al modelo base. Funcionan modificando capas específicas del modelo usando descomposición de matrices de bajo rango.

**⚠️ Importante:** Los LoRAs son específicos de versión de modelo. Un LoRA de SD1.5 NO funcionará con SDXL, y viceversa.

**Cómo cargar un LoRA en A1111/Forge:**
1. Descarga el `.safetensors` del LoRA
2. Colócalo en `models/Lora/`
3. En el prompt: haz clic en el botón de LoRA o escribe directamente: `<lora:nombre_del_archivo:peso>`
4. Ejemplo: `<lora:add_detail:0.7>` (rango de peso típico: 0.3–1.0)
5. Múltiples LoRAs: `<lora:estilo1:0.5> <lora:personaje1:0.8>`

**Cómo cargar un LoRA en ComfyUI:**
1. Coloca el archivo en `ComfyUI/models/loras/`
2. Añade el nodo "Load LoRA" a tu workflow
3. Encadena múltiples nodos "Load LoRA" en serie si necesitas varios

**Dónde encontrar LoRAs:**
- [Civitai](https://civitai.com) — filtra por "LoRA" (la selección más grande)
- [Tensor.Art](https://tensor.art/models) — alternativa a Civitai
- [Hugging Face](https://huggingface.co) — busca con filtro "LoRA"

**Entrenar tu propio LoRA:**
- Local (gratuito): [Kohya SS GUI](https://github.com/bmaltais/kohya_ss) — requiere GPU y 10-50 imágenes mínimo
- En la nube (Civitai): Entrenamiento online en la plataforma (con créditos Buzz)

**Consejos:**
- Peso recomendado: 0.5–0.8 (por encima de 1.0 puede causar artefactos)
- Prueba con 0.5 y ajusta hacia arriba si el efecto es insuficiente
- Puedes combinar hasta 3-4 LoRAs simultáneamente con buenos resultados

---

### Upscaling (Mejora de Resolución)

**Qué hace:** Aumenta la resolución de una imagen. Hay varios enfoques con diferentes características.

#### HiRes Fix (A1111 integrado)
No es un upscaler puro — es un método de generación en dos pasadas:
1. Genera a resolución nativa (ej: 512×512)
2. Ejecuta img2img en el resultado a la resolución objetivo (ej: 1024×1024)

**Configuración recomendada:** Upscaler: R-ESRGAN 4x+ | Denoising Strength: 0.4–0.6 | Escala: 2x

**Ventaja:** Añade detalle genuino, no solo pixels. **Desventaja:** Tarda el doble que una generación normal.

#### ESRGAN / RealESRGAN (rápido, determinista)
Upscaler puro basado en IA — rápido y predecible. Disponible en la pestaña "Extras" de A1111.

| Modelo | Para qué |
|--------|---------|
| R-ESRGAN 4x+ | Uso general, funciona bien en la mayoría de imágenes |
| R-ESRGAN 4x+ Anime6B | Optimizado para anime e ilustración |
| ESRGAN_4x | Clásico, bueno para fotorrealismo |

#### Tiled Diffusion (Extensión A1111)
Divide la imagen en tiles solapados, procesa cada tile con img2img y reconstruye el resultado. Permite resoluciones muy altas con poca VRAM.

**Mejor combinación:** Tiled Diffusion + ControlNet Tile para máxima coherencia.

**Flujo de trabajo recomendado:**
1. Genera a resolución nativa (512/1024)
2. Aplica HiRes Fix (escala 2x, denoising 0.5)
3. Si necesitas más detalle: Ultimate SD Upscale con ControlNet Tile

**Herramientas gratuitas:** A1111 (HiRes Fix + Extras), Forge, ComfyUI (nodos de upscaling nativos), InvokeAI

---

### CFG Scale (Escala de Guía)

**Qué hace:** Controla qué tan estrictamente el modelo sigue el prompt vs. libertad creativa. Valores más altos = más adherencia al prompt. Valores más bajos = más creatividad (y a veces incoherencia).

| Valor CFG | Comportamiento | Cuándo usar |
|-----------|---------------|-------------|
| 1–3 | Casi sin influencia del prompt, muy creativo/caótico | Solo para experimentación artística |
| 4–7 | Equilibrado: buena calidad + algo de creatividad | **Recomendado para SDXL** |
| 7–10 | Alta adherencia al prompt | **Recomendado para SD1.5** |
| 10–15 | Muy estricto, prompts detallados | Con prompts muy específicos |
| 16–20 | Oversaturado, artefactos frecuentes | Evitar generalmente |

**Valores por modelo:**
- SD1.5: CFG 7-9 típico
- SDXL: CFG 5-7 (SDXL es más sensible a CFG alto)
- FLUX: CFG 1-3 (FLUX usa un mecanismo de guía diferente)

---

### Samplers y Steps (Muestreadores y Pasos)

**Qué hacen los Steps:** Controlan cuántas iteraciones de denoising realiza el modelo. Más steps = resultado más refinado hasta cierto punto, luego rendimientos decrecientes.

**Referencia rápida de samplers:**

| Sampler | Steps min. | Steps recom. | Notas |
|---------|-----------|-------------|-------|
| Euler | 15 | 20-30 | Rápido, buena calidad, determinista |
| Euler A (Ancestral) | 15 | 20-30 | Añade aleatoriedad, resultados más variados |
| DDIM | 10 | 15-25 | Rápido, determinista, pocas pasos necesarios |
| DPM++ 2M Karras | 5 | 20-30 | El más popular 2024-2025. Excelente calidad/velocidad |
| DPM++ SDE Karras | 15 | 25-35 | Más lento pero muy alta calidad. Para renders finales |
| UniPC | 5 | 15-25 | Muy eficiente, solo 10-15 steps para buena calidad |
| LCM | 4 | 4-8 | Ultra-rápido (requiere LoRA LCM). Calidad inferior. |

**Guía práctica:**
- Menos de 20 steps: las imágenes parecen "crudas" con la mayoría de samplers
- 20-30 steps: zona óptima calidad/velocidad
- Más de 40 steps: raramente mejora la calidad lo suficiente para justificar el tiempo extra

**Consejos:**
- Para previsualizar rápido: LCM con 4-8 steps
- Para resultado final: DPM++ 2M Karras con 25-30 steps
- Euler A: cambia mucho al cambiar el número de steps (útil para exploración)

---

### Negative Prompts (Prompts Negativos)

**Qué son:** Términos en el campo de prompt negativo que instruyen al modelo a evitar esos conceptos durante la generación. Funcionan via el mismo mecanismo de Guía Sin Clasificador (CFG) que el prompt positivo, pero en dirección opuesta.

**Plantilla estándar para SD1.5:**
```
ugly, tiling, poorly drawn hands, poorly drawn feet, poorly drawn face,
out of frame, extra limbs, disfigured, deformed, body out of frame,
bad anatomy, watermark, signature, cut off, low contrast, underexposed,
overexposed, bad art, distorted face, blurry, draft, grainy,
worst quality, low quality, lowres, jpeg artifacts
```

**Para SDXL (más corto es mejor):**
```
blurry, low quality, watermark, signature
```
SDXL es más inteligente — los prompts negativos muy largos a menudo empeoran los resultados.

**Negativos específicos para anatomía:**
```
extra fingers, missing fingers, extra limbs, fused fingers,
deformed hands, bad anatomy, asymmetrical eyes
```

**Embeddings de negativos (atajos):**
Los embeddings como `EasyNegative` o `BadDream` codifican muchos conceptos negativos en un solo token. Descárgalos de Civitai y úsalos como `EasyNegative` en el prompt negativo.

**Consejos:**
- Empieza minimal, añade términos solo cuando veas problemas específicos
- Con CFG 12+: reduce los negativos a 3-5 términos máximo
- Para SDXL: usa negativos muy cortos o ninguno

---

## 6. Guía de Prompt Engineering

### Estructura de Prompt para SD1.5
```
[Sujeto], [Estilo], [Referencias de artista], [Iluminación], [Cámara/óptica], [Tags de calidad]
```

**Ejemplo:**
```
portrait of a warrior woman, digital painting, concept art,
artstation trending, dramatic studio lighting, 8k, highly detailed,
sharp focus, masterpiece, by Greg Rutkowski
```

**Tags de calidad que funcionan en SD1.5:**
```
masterpiece, best quality, high quality, highly detailed,
sharp focus, 8k, ultra realistic, professional photography,
studio lighting, artstation trending
```

---

### Estructura de Prompt para SDXL (Lenguaje Natural)

SDXL prefiere descripciones conversacionales en lugar de acumulación de tags. Usa frases naturales:

```
A photorealistic portrait of a warrior woman in ornate armor,
dramatic studio lighting against a dark background,
sharp focus, professional photography, 8k
```

**Diferencias clave vs SD1.5:**
- Evita 20+ tags de calidad — 2-3 es suficiente
- **Elimina** "masterpiece, best quality" — estos tags perjudican activamente a SDXL
- Resolución objetivo nativa: 1024×1024
- Steps recomendados: 25 | CFG: 5-7

---

### Sintaxis de Ponderación de Prompts

#### En AUTOMATIC1111 / Forge:
```
(keyword)         → peso ×1.1
((keyword))       → peso ×1.21
(keyword:1.5)     → exactamente ×1.5 (explícito)
[keyword]         → peso ×0.9 (reduce énfasis)
[keyword:0.5]     → exactamente ×0.5
```

**Sintaxis de atención temporal (A1111):**
```
[word1:word2:0.5]   → usa word1 en los primeros 50% de steps, luego word2
[word:0.3]          → introduce la palabra en el 30% de los steps
```

#### En ComfyUI:
```
(keyword:1.5)     → ×1.5 (mismo formato, efecto MÁS FUERTE que en A1111)
(keyword:0.7)     → ×0.7
```
**⚠️ Importante:** El mismo valor de peso tiene **efecto más fuerte en ComfyUI** que en A1111. Usa valores más bajos en ComfyUI (ej: 1.3 en ComfyUI ≈ 1.5 en A1111).

**Rango seguro:** Mantén los pesos entre **0.4 y 1.6**. Fuera de este rango aparecen artefactos.

---

### Plantillas de Prompts Comunes

#### Retrato fotorrealista:
```
POSITIVO:
professional photo portrait of [descripción del sujeto],
[detalles de ropa/fondo], golden hour lighting, bokeh background,
50mm lens, sharp focus, high detail, 8k

NEGATIVO:
blurry, low quality, bad anatomy, poorly drawn face, watermark
```

#### Arte conceptual:
```
POSITIVO:
[sujeto] concept art, digital painting, by [artista],
artstation trending, epic lighting, detailed environment,
cinematic composition, highly detailed

NEGATIVO:
ugly, tiling, poorly drawn, bad anatomy, worst quality, sketch
```

#### Anime / Ilustración:
```
POSITIVO:
[sujeto], anime style, [artista si aplica],
beautiful detailed eyes, vivid colors, soft lighting,
high quality, sharp focus

NEGATIVO:
lowres, bad anatomy, extra limbs, poorly drawn face,
mutation, deformed, ugly, blurry, bad proportions
```

---

### Recursos de Inspiración de Prompts

| Recurso | URL | Para qué |
|---------|-----|---------|
| **Lexica.art** | https://lexica.art | Busca por estilo → ve el prompt exacto, semilla, CFG y sampler. El mejor recurso. |
| **PromptHero** | https://prompthero.com | Galería de prompts con generador integrado. |
| **Krea.ai** | https://www.krea.ai | Búsqueda visual + generación en tiempo real. Muy útil para matching de estilo. |
| **OpenArt Prompt Book** | https://openart.ai/promptbook | Guía visual curada. Buena para empezar. |
| **Civitai Guides** | https://civitai.com/articles/11432 | Guía definitiva de prompts SDXL realistas (comunidad). |

---

## 7. Extensiones y Plugins

### Para AUTOMATIC1111 y Forge

**Cómo instalar extensiones en A1111/Forge:**
1. Ve a la pestaña `Extensions`
2. Haz clic en `Available` → `Load from` para ver el catálogo
3. O usa `Install from URL` con el enlace de GitHub
4. Después de instalar: `Installed` → `Apply and restart UI`

---

#### sd-webui-controlnet ✅

- **Qué hace:** Añade condicionamiento ControlNet a la generación (pose, profundidad, bordes, etc.)
- **GitHub:** https://github.com/Mikubill/sd-webui-controlnet
- **Instalación:** Extensions → Install from URL → pega el enlace de GitHub
- **Nota:** Descarga los modelos de preprocesador desde la propia interfaz de ControlNet; los modelos ControlNet van en `models/ControlNet/`

---

#### ADetailer (After Detailer) ✅

- **Qué hace:** Detecta y mejora automáticamente caras, manos y cuerpos después de la generación inicial. Soluciona el problema de "cara de papa" en resoluciones bajas.
- **Cómo funciona:** Ejecuta un modelo de detección (YOLOv8) para encontrar caras/manos → recorta → hace inpainting con más detalle → compone el resultado de vuelta.
- **GitHub:** https://github.com/Bing-su/adetailer
- **Recomendado para:** Cualquier generación con sujetos humanos.
- **Guía:** https://stable-diffusion-art.com/adetailer/

---

#### Tiled Diffusion + VAE ✅

- **Qué hace:** Genera o escala imágenes de muy alta resolución con poca VRAM procesando en tiles solapados.
- **GitHub:** https://github.com/pkuliyi2015/multidiffusion-upscaler-for-automatic1111
- **Mejor uso:** Combinado con ControlNet Tile para salida coherente en alta resolución.

---

#### Ultimate SD Upscale ✅

- **Qué hace:** Script de upscaling por tiles con soporte ControlNet. Más flexible que el upscale integrado.
- **GitHub:** https://github.com/Coyote-A/ultimate-upscale-for-automatic1111
- **Nota:** El solapamiento de tiles es configurable; funciona con o sin ControlNet Tile.

---

#### CLIP Interrogator ✅

- **Qué hace:** Hace ingeniería inversa — analiza cualquier imagen y genera el prompt de texto que la describiría. Usa modelos CLIP + BLIP.
- **GitHub:** https://github.com/pharmapsychotic/clip-interrogator
- **Caso de uso:** "¿Qué prompt generaría una imagen como esta?"

---

#### Regional Prompter ✅

- **Qué hace:** Divide el lienzo en regiones (filas, columnas o áreas con máscara) y asigna diferentes prompts a cada región. Permite escenas con múltiples personajes o elementos precisamente controlados.
- **GitHub:** https://github.com/hako-mikan/sd-webui-regional-prompter
- **Guía:** https://stable-diffusion-art.com/regional-prompter/

---

#### Deforum ✅

- **Qué hace:** Extensión de animación. Crea videos animados con una secuencia de prompts de texto y configuraciones de movimiento de cámara.
- **GitHub:** https://github.com/deforum-art/sd-webui-deforum

---

### Para ComfyUI (Nodos Personalizados)

**Cómo instalar nodos en ComfyUI:**
1. Instala primero **ComfyUI Manager** (ver abajo)
2. Abre ComfyUI → haz clic en "Manager" en el menú
3. Busca el nodo → Install → reinicia ComfyUI

---

#### ComfyUI Manager ✅ (Instala este primero)

- **Qué hace:** Instala, actualiza y elimina nodos personalizados con un clic. Imprescindible — instálalo antes que cualquier otra cosa.
- **GitHub:** https://github.com/ltdrdata/ComfyUI-Manager
- **Instalación manual (primera vez):** `git clone https://github.com/ltdrdata/ComfyUI-Manager` en la carpeta `ComfyUI/custom_nodes/`
- **Consenso comunidad:** "El 100% de los usuarios avanzados lo usa. Empieza por aquí."

---

#### ComfyUI Impact Pack ✅

- **Qué hace:** Equivalente a ADetailer para ComfyUI. Detección y mejora de caras/manos, segmentación, pipelines de upscaling.
- **GitHub:** https://github.com/ltdrdata/ComfyUI-Impact-Pack
- **Funciones clave:** Detector, Detailer (mejora cara/manos), nodos Upscaler, sistema SEGS (segmentación).

---

#### WAS Node Suite ✅

- **Qué hace:** Más de 218 nodos de utilidad — procesamiento de imágenes, manipulación de texto, operaciones de archivo, matemáticas y más.
- **GitHub (fork mantenido):** https://github.com/ltdrdata/was-node-suite-comfyui
- **Nota:** El repositorio original de WASasquatch está archivado (autor retirado en marzo 2025) — usa el fork de ltdrdata.
- **Instalación:** Busca "WAS Node Suite" en ComfyUI Manager.

---

#### ComfyUI IPAdapter Plus ✅

- **Qué hace:** Integración de IP-Adapter para ComfyUI. Permite usar imágenes de referencia para guiar el estilo, personaje o cara de la generación sin ControlNet.
- **GitHub:** https://github.com/cubiq/ComfyUI_IPAdapter_plus
- **Caso de uso:** "Hazlo parecido a esta imagen de referencia" para consistencia de estilo, personaje o cara.
- **Nota:** Requiere descargar los archivos de modelo IPAdapter por separado.

---

#### ComfyUI ControlNet Auxiliary Preprocessors ✅

- **Qué hace:** Todos los preprocesadores de ControlNet (Canny, Depth, Pose, Lineart, etc.) en un solo paquete.
- **Instalación:** Busca "ControlNet Auxiliary Preprocessors" en ComfyUI Manager.

---

## 8. Recursos de Aprendizaje y Comunidades

### Canales de YouTube

| Canal | URL | Nivel | Enfoque |
|-------|-----|-------|---------|
| **Aitrepreneur** | https://www.youtube.com/@Aitrepreneur | Principiante–Intermedio | Tutoriales completos de A1111, InvokeAI, FLUX. Aplicaciones creativas y de negocio. |
| **Olivio Sarikas** | https://www.youtube.com/@OlivioSarikas | Principiante–Intermedio | Guías de instalación paso a paso, prompt engineering, múltiples herramientas desde perspectiva artística. |
| **Scott Detweiler** | Buscar en YouTube | Intermedio–Avanzado | Casos de uso detallados, workflows técnicos. Referenciado por Stability AI como leyenda de la comunidad. |

---

### Comunidades Reddit

#### r/StableDiffusion ✅
- **URL:** https://www.reddit.com/r/StableDiffusion
- **Tamaño:** 500,000+ miembros
- **Contenido:** Muestras de arte, preguntas sobre herramientas, lanzamientos de modelos, compartir workflows, resolución de problemas.
- **Recurso clave:** El wiki de la comunidad tiene notebooks de Colab y guías de inicio mantenidas.
- **Consenso 2026:** "Empieza con A1111 si eres nuevo; cambia a ComfyUI para FLUX y rendimiento."

#### r/comfyui ✅
- **URL:** https://www.reddit.com/r/comfyui
- **Contenido:** Compartir workflows en nodos, preguntas específicas de ComfyUI, recomendaciones de nodos personalizados.
- **Recursos clave:** La comunidad recomienda ComfyUI Manager como primera instalación; hilo de inicio fijado.

---

### Sitios de Tutoriales y Documentación

#### Stable Diffusion Art ✅ (El más completo)
- **URL:** https://stable-diffusion-art.com
- **Qué tiene:** El sitio más comprehensivo en inglés — cubre ComfyUI, A1111, Forge, técnicas, modelos.
- **Páginas clave:**
  - Guía de principiantes: https://stable-diffusion-art.com/beginners-guide/
  - ControlNet: https://stable-diffusion-art.com/controlnet/
  - LoRA: https://stable-diffusion-art.com/lora/
  - Samplers: https://stable-diffusion-art.com/samplers/
  - Sitios generadores gratuitos: https://stable-diffusion-art.com/free-ai-image-generator-sites/

#### Civitai Education Hub ✅
- **URL:** https://education.civitai.com
- **Qué tiene:** Guías oficiales de la plataforma + tutoriales comunitarios verificados.
- **Guías destacadas:**
  - Primeros pasos con SD3.5: https://education.civitai.com/getting-started-with-stable-diffusion-3-5/
  - FLUX Quickstart: https://education.civitai.com/quickstart-guide-to-flux-1/
  - Entrenador de LoRA: https://education.civitai.com/using-civitai-the-on-site-lora-trainer/

#### Documentación oficial ComfyUI ✅
- **URL:** https://docs.comfy.org
- Tutorial de LoRA: https://docs.comfy.org/tutorials/basic/lora
- Requisitos del sistema: https://docs.comfy.org/installation/system_requirements

#### Stability AI Learning Hub ✅
- **URL:** https://stability.ai/learning-hub
- Configurar SD3 Medium localmente: https://stability.ai/learning-hub/setting-up-and-using-sd3-medium-locally
- ControlNets para SD3.5 Large: https://stability.ai/news/sd3-5-large-controlnets

#### Wiki de AUTOMATIC1111 ✅
- Features: https://github.com/AUTOMATIC1111/stable-diffusion-webui/wiki/features
- Negative prompts: https://github.com/AUTOMATIC1111/stable-diffusion-webui/wiki/Negative-prompt
- Optimizaciones: https://github.com/AUTOMATIC1111/stable-diffusion-webui/wiki/Optimizations

---

### Línea de Tiempo de Modelos (Contexto Histórico)

| Modelo | Año | Resolución nativa | Estado en 2026 |
|--------|-----|-------------------|----------------|
| SD 1.5 | 2022 | 512×512 | Aún muy usado; ecosistema masivo de LoRAs |
| SDXL 1.0 | 2023 | 1024×1024 | Popular; gran ecosistema de LoRAs |
| SD3 / SD3.5 | 2024 | 1024×1024 | Arquitectura MMDiT; mejor texto en imágenes |
| FLUX.1 Dev/Schnell | 2024 | Flexible | El más popular para fotorrealismo; 12B params |
| FLUX.2 Dev | Nov 2025 | Flexible | 32B params; soporte multi-referencia (hasta 10 imgs); variante "Klein" Apache 2.0 |

---

*Última actualización: 2026-03-06*
*Fuentes: Stable Diffusion Art, Civitai Education Hub, documentación oficial de ComfyUI, A1111, InvokeAI, Forge Classic, r/StableDiffusion, Stability AI Learning Hub, GitHub oficial de cada proyecto.*
