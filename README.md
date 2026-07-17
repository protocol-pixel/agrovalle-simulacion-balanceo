# Simulación · Balanceo de línea y espacio (Guerchet) — AgroValle Piura S.A.C.

Simulación interactiva en una sola página (HTML/CSS/JS, sin dependencias) que muestra cómo el **balanceo de una línea de producción** y el **cálculo de espacio físico (método de Guerchet)** están conectados entre sí, usando como caso el proceso de envasado de pulpa de mango de AgroValle Piura S.A.C.

## Qué hace

Al mover el control de "unidades por turno (8 h)" la simulación recalcula en vivo:

- **Producción (u/h)** y **tiempo de ciclo** disponible por estación.
- **Número de estaciones de trabajo** necesarias, agrupando las 10 tareas del proceso (Recepción → Empaque) según el tiempo de ciclo.
- **Aprovechamiento de la línea** (eficiencia de balanceo).
- **Cuello de botella**: la estación con más carga respecto al ciclo, resaltada visualmente.
- **Espacio por zona (m²)**, calculado previamente con el método de Guerchet, y el espacio total de planta.

El objetivo es didáctico: evidenciar que la estación que más tiempo consume (pasteurizado) suele ser también la que más espacio requiere.

## Cómo usarlo

Abre `index.html` directamente en el navegador — no requiere instalación, servidor ni build.

También puedes verlo publicado con GitHub Pages (ver sección siguiente).

## Publicar con GitHub Pages (opcional)

1. Settings → Pages → Source: rama `main`, carpeta `/root`.
2. La simulación quedará disponible en `https://protocol-pixel.github.io/agrovalle-simulacion-balanceo/`.

## Estructura

```
index.html   # HTML + CSS + JS, todo en un solo archivo
```

## Contexto

Caso práctico del curso de Diseño de Instalaciones.
