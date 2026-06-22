# Iván Roblero — Portfolio

Sitio estático de una sola página. Todo (runtime, fuentes e imágenes) está incrustado en `index.html`; no requiere build ni dependencias.

## Contenido
- `index.html` — el sitio completo, autocontenido.
- `vercel.json` — configuración mínima (URLs limpias + headers de seguridad).

## Desplegar en Vercel

### Opción A — Drag & drop (la más rápida)
1. Entra a https://vercel.com/new
2. Arrastra **esta carpeta** completa.
3. Framework Preset: **Other**. No hace falta configurar build. Deploy.

### Opción B — Vercel CLI
```bash
npm i -g vercel
cd deploy
vercel        # despliegue de preview
vercel --prod # despliegue a producción
```

### Opción C — Git + Vercel (recomendado para actualizar)
1. Sube esta carpeta a un repositorio de GitHub.
2. En Vercel: **Add New → Project → Import** ese repo.
3. Framework Preset: **Other** → Deploy.
4. Cada `git push` redeploya automáticamente.

## Editar el sitio
El `index.html` es un archivo generado. Para cambios edita el diseño original
(`Portfolio - Ivan Roblero.dc.html`) y vuelve a generar el bundle.
