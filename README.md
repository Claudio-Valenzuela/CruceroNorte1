# Crucero Norte

Este proyecto es una landing estática para el restobar `Crucero Norte`.

## Estructura del proyecto

- `public/` — archivos estáticos listos para servir en un entorno moderno.
  - `public/index.html`
  - `public/nosotros.html`
  - `public/styles.css`
  - `public/img/` — carpeta para activos de imagen.
- `.gitignore` — ignores básicos para proyectos Node.js.

## Cómo usar

1. Sitúa los archivos HTML, CSS y las imágenes en `public/`.
2. Abre `public/index.html` directamente en el navegador, o utiliza un servidor estático.

### Servir localmente con Node.js

Si tienes Node.js instalado, puedes usar un servidor estático como `serve` o `http-server`:

```bash
npx serve public
```

O con `http-server`:

```bash
npx http-server public
```

## Nota

La nueva estructura de carpeta `public/` está preparada para un flujo de desarrollo moderno. Actualmente los recursos de imagen siguen en `img/` en la raíz, por lo que `public/index.html` y `public/nosotros.html` usan rutas relativas a ese directorio.

Para que `public/` sea completamente autocontenida, mueve la carpeta `img/` dentro de `public/` y actualiza las rutas de las imágenes a `img/`.
