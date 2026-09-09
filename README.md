# XR Lab Multiplataforma — A-Frame

Guía de laboratorio: **Desarrollo de Ambientes de Realidad Extendida (XR)
Multiplataforma con A-Frame** (Realidad Virtual, Ing. Mecatrónica, UMNG).

## Estructura

```
xr-lab-v2/
├── index.html            → hub con tarjetas hacia cada fase
├── css/xr-ui.css           → sistema visual compartido (header, toolbar, panel info, hint)
├── fases/
│   ├── fase1.html           → Parte A: escena básica con primitivas
│   ├── fase2.html            → Parte C: celda de manufactura (tanque, banda, robot)
│   └── fase3.html             → Parte D: integración de modelo CAD (GLB)
└── models/
    └── LEEME.txt              → instrucciones para colocar modelo.glb
```

Cada fase es una página **independiente y autosuficiente**: se puede abrir directamente
o navegar hacia ella desde `index.html`. Dentro de cada una, la barra de botones superior
aísla un componente a la vez y desplaza la cámara suavemente hasta él; el panel inferior
izquierdo explica qué se está mostrando.

## Fase 3 — tu propio modelo CAD

`fases/fase3.html` intenta cargar `models/modelo.glb`. Si no existe, aparece un marcador
de referencia y el botón **↻ Reintentar carga**. Para ver tu ensamblaje:

1. Exporta el ensamblaje de SolidWorks a `.stl`.
2. Impórtalo en Blender y optimiza la geometría.
3. Exporta como `.glb` y guárdalo en `models/modelo.glb`.
4. Pulsa **↻ Reintentar carga** en la Fase 3.

## Publicar en GitHub Pages

1. Sube esta carpeta a un repositorio público de GitHub.
2. Activa **Settings → Pages** con `Branch: main`, `Folder: /root`.
3. Prueba `index.html` y las tres fases en escritorio, móvil, modo VR, modo AR y en el
   navegador del Meta Quest 3.
