# Contexto del Proyecto: Portafolio Profesional de DIT y Data Manager

## Perfil del Cliente
* **Nombre/Marca:** FeloRF (Felipe Andrés Rojas Flores)
* **Profesión:** Director de Fotografía (DoP), Digital Imaging Technician (DIT) y Data Manager con 15 años de experiencia en cine y publicidad.
* **Objetivo de la Web:** Exhibición de portafolio técnico, flujos de trabajo de datos seguros (MD5/XXHash, LTO), gestión de color en set (Livegrade, monitorización HDR) y contacto para productoras de cine y publicidad.
* **Enfoque Visual:** Estética cinematográfica, prolija, minimalista, modo oscuro por defecto. Máxima prioridad a la velocidad de carga de material multimedia pesado.

## Stack Tecnológico Detectado
* **Framework Principal:** Astro v6 (Enrutamiento basado en archivos en `src/pages/`)
* **Estilos:** Tailwind CSS v4 (Configurado vía `@tailwindcss/vite`)
* **Lenguaje:** TypeScript (`tsconfig.json` estricto)
* **Entorno:** Node.js >= 22.12.0

## Reglas de Desarrollo Globales
1.  **Cero JavaScript innecesario:** Mantener la filosofía de islas de Astro. Los componentes visuales deben ser estáticos a menos que requieran interactividad explícita.
2.  **Optimización Multimedia:** Todo renderizado de fotogramas (stills) debe procesarse a través de `src/assets/` usando las herramientas de optimización nativas de Astro para no comprometer el rendimiento en dispositivos móviles.