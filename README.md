# XR Lab Multiplataforma — A-Frame (UMNG)

Guía de laboratorio: **Desarrollo de Ambientes de Realidad Extendida (XR)
Multiplataforma con A-Frame** (Realidad Virtual, Ing. Mecatrónica, UMNG).

## Novedades de esta versión

- Interfaz con el escudo de la UMNG en la barra lateral, en paleta institucional
  (azul marino + dorado) en lugar del azul corporativo genérico anterior.
- **Fase 1**: nuevo orden de primitivas (cilindro → caja → esfera), nueva paleta
  de color (terracota / verde azulado / morado) y nuevo entorno (piso e
  iluminación cálidos, niebla suave).
- **Fase 2**: el tanque se reemplazó por un **silo con tolva** (a-cylinder +
  a-cone) y el brazo robótico por una **grúa pórtico** (a-box + a-torus) con
  un carro que se desplaza sobre la viga.
- **Fase 3**: ahora referencia `models/Cubo_v1.glb`, el nombre de tu archivo.

## Estructura

```
xr-lab-v4/
├── index.html            → hub con tarjetas hacia cada fase
├── assets/umng-logo.png   → escudo de la universidad
├── css/xr-ui.css           → sistema visual compartido (barra lateral, paleta UMNG)
├── fases/
│   ├── fase1.html           → Parte A: escena básica reordenada
│   ├── fase2.html            → Parte C: silo + banda + grúa pórtico
│   └── fase3.html             → Parte D: integración de Cubo_v1.glb
└── models/
    ├── LEEME.txt               → instrucciones para colocar el modelo
    └── Cubo_v1.glb              → ⚠️ marcador temporal, ver aviso abajo
```

## ⚠️ Sobre tu archivo Cubo_v1.GLB

El archivo que subiste llegó con **0 KB** (vacío), probablemente por un problema
al adjuntarlo. Mientras tanto, dejé un cubo de referencia con el mismo nombre
para que la Fase 3 no se vea vacía. Para ver tu modelo real:

1. Verifica que el archivo `.glb` no esté corrupto ni vacío en tu computador.
2. Reemplaza `models/Cubo_v1.glb` por el archivo correcto.
3. Abre la Fase 3 y pulsa **↻ Reintentar carga**.

## Publicar en GitHub Pages

1. Sube esta carpeta a un repositorio público de GitHub.
2. Activa **Settings → Pages** con `Branch: main`, `Folder: /root`.
3. Prueba `index.html` y las tres fases en escritorio, móvil, modo VR, modo AR y
   en el navegador del Meta Quest 3.
