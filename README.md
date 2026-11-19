# Dashboard del Clima

Dashboard del clima con React, TypeScript, MUI y la API de Open-Meteo (código de las guías 08 a 11 de DAWM).

- Selector de ciudades: Guayaquil, Quito, Manta y Cuenca
- Indicadores del clima actual, gráfico y tabla de temperatura y viento por hora
- Estados de carga y de error

URL pública (reemplace `TU_USUARIO`): https://TU_USUARIO.github.io/dashboard/

## Antes de publicar

1. El repositorio debe llamarse **dashboard**. Si usa otro nombre, cambie `base: '/dashboard/'` en `vite.config.ts` por `base: '/<nombre_del_repositorio>/'`.
2. En `package.json`, reemplace `TU_USUARIO` en `homepage` por su usuario de GitHub.

## Opción A: con la terminal (como en la guía 08)

```
npm install
npm run dev        # vista previa local
npm run deploy     # compila y publica la carpeta dist en la rama gh-pages
```

Luego, en GitHub: **Settings > Pages > Build and deployment > Source: Deploy from a branch**, rama **gh-pages**, carpeta **/ (root)**.

Si usa esta opción, puede borrar la carpeta `.github` para que no se ejecute el flujo de la opción B.

## Opción B: sin terminal (GitHub Actions)

1. Suba todos los archivos a la rama **main** del repositorio (incluida la carpeta `.github/workflows`).
2. En GitHub: **Settings > Pages > Build and deployment > Source: GitHub Actions**.
3. Espere a que termine el flujo en la pestaña **Actions** (1 a 2 minutos). La URL aparece en el paso *deploy*.

## Verificación

Abra la URL en una ventana de incógnito. Debe mostrar el dashboard sin pedir inicio de sesión. Si el repositorio es privado, haga que sea público para que cualquiera pueda abrir la página.
