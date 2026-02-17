# Clase 01

> Fecha: 17/02/2026
> Tema: Introducción

## Descripción

## Notas

Nick Bostrom - Superintelligence 

**Modelos para generaciones**

Kling
Nano Banana (Google)
Veo3 (Google)
Seedance 2.0 (Tiktok)

**Apps recomendadas**

Higgsfield
Freepik

**Plataformas Node-Based**

- Reutilización de recursos
- Flujos Visuales claro
- Control creativo
- Escalabilidad de proyectos
- Automatización de proyectos
- Creación de sistemas repetibles (workflows)
- Mapa conceptual de generaciones

Las plataformas node-based permiten construir flujos de trabajo visuales conectando nodos, donde cada nodo representa una operación o herramienta de IA. En lugar de escribir código, se arrastran y conectan bloques que procesan texto, imágenes o video en secuencia. Esto facilita automatizar pipelines de generación complejos y reutilizarlos con distintos inputs sin reconfigurar todo desde cero.

**Prompts en formato JSON**

```json
{
  "role": "cinematographer",
  "scene": {
    "subject": "a lone astronaut walking on Mars",
    "style": "cinematic, photorealistic",
    "lighting": "golden hour, long shadows",
    "camera": "low angle, slow dolly forward",
    "mood": "epic, solitary",
    "duration": "5 seconds"
  }
}
```

Un prompt en JSON estructura la instrucción al modelo en pares `clave: valor`, lo que lo hace más preciso y reproducible que el lenguaje natural. Se compone de:

- **`role`** — define el "personaje" o especialidad que adopta el modelo (ej: cinematógrafo, director de arte)
- **`scene`** — objeto que agrupa todos los parámetros visuales de la generación:
  - **`subject`** — qué o quién aparece en la escena
  - **`style`** — estética visual deseada
  - **`lighting`** — tipo de iluminación
  - **`camera`** — ángulo y movimiento de cámara
  - **`mood`** — emoción o atmósfera buscada
  - **`duration`** — duración del clip en segundos

> La ventaja es reutilizar la estructura base y solo cambiar los valores para generar variaciones consistentes.

Gemini - GEMS - Módulos de memoria creativa

Los GEMS son asistentes personalizados dentro de Gemini a los que se les puede configurar un comportamiento fijo, como si se les asignara un "rol permanente". Sirven para reutilizar contexto creativo sin tener que repetir las instrucciones cada vez.

**Ejemplo de configuración de un GEM para generación de videos:**

```
Eres un director creativo especializado en generación de videos con IA.

Cuando el usuario te dé una idea, responde SIEMPRE con:
1. Una descripción visual de la escena en lenguaje cinematográfico
2. Un prompt listo para usar en formato JSON con los campos: role, scene (subject, style, lighting, camera, mood, duration)
3. Una sugerencia de herramienta recomendada (Kling, Veo3, Seedance, etc.) según el tipo de contenido

Mantén un tono profesional pero directo. Prioriza la coherencia visual y la reutilización de estilos entre escenas.
```

> Con este GEM configurado, solo se le describe la idea y él genera el prompt JSON listo para copiar y pegar en la herramienta de generación.

## Recursos

- [MAG3 - Curso de IA para Video](https://www.instagram.com/mag3.gg/)
- [Veo 3 - Google AI Studio](https://aistudio.google.com/models/veo-3)
- [Gemini 2.5 Flash Image - Google AI Studio](https://aistudio.google.com/models/gemini-2-5-flash-image)
- [Kling AI](https://klingai.com/global/)
- [Higgsfield AI](https://higgsfield.ai/)
- [Freepik AI Video Generator](https://www.freepik.com/ai/video-generator)
- [Gemini GEMS](https://gemini.google/es/overview/gems/?hl=es)
- [Why JSON Prompts Make AI More Reliable - Medium](https://medium.com/coding-nexus/why-json-prompts-make-ai-more-reliable-with-code-real-examples-edf439999ce7)
- [Genie - Google DeepMind](https://deepmind.google/models/genie/)