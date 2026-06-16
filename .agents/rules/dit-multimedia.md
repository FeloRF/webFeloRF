---
trigger: manual
---

# Regla: Optimización de Stills y Contenedores de Video de Rodajes

Esta regla regula cómo el agente debe construir componentes que manejen capturas de pantalla de esquemas técnicos, interfaces de software de color o fotogramas de películas.

## 1. Tratamiento de Imágenes Técnicas y Stills
* Las imágenes de muestras de color o setups en set DEBEN guardarse en `src/assets/`.
* Queda estrictamente PROHIBIDO usar la etiqueta nativa `<img>` para archivos locales.
* Usa siempre el componente `<Image />` de `astro:assets` forzando formatos modernos (`.webp` o `.avif`).
* Cada imagen debe incluir metadatos descriptivos en su atributo `alt` (ej: "Esquema de flujo de datos DIT - ARRI Alexa 35 ").

## 2. Integración de Video (Reels y Muestras)
* Para incrustar reproductores de Vimeo o YouTube para los reels de proyectos, se deben utilizar fachadas (*facades*) o el atributo `loading="lazy"` para que los scripts pesados de los reproductores no bloqueen la carga inicial de la página.