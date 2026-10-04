# EntiScan — sitio público

Sitio estático de EntiScan, sin JavaScript, backend, cookies, analytics ni recursos externos. Este repositorio contiene únicamente el sitio público.

- Home: https://luquemariano.github.io/entiscan-site/
- Privacidad: https://luquemariano.github.io/entiscan-site/privacy/
- Soporte: https://luquemariano.github.io/entiscan-site/support/

## Editar

Editar `index.html`, `privacy/index.html` o `support/index.html`. Los estilos compartidos están en `styles.css`; el icono de marca está en `assets/entiscan.png`. Mantener rutas relativas para funcionar bajo `/entiscan-site/`.

El botón **Chrome Web Store** es un placeholder explícitamente deshabilitado con el texto «Próximamente». Cuando exista la URL real del item, reemplazar el elemento `button.store` por un enlace `a.store` con esa URL y quitar el estado deshabilitado y el aviso. No hay una URL de tienda inventada.

## Desplegar

GitHub Settings → Pages → Source: GitHub Actions. Cada push a `main` ejecuta `.github/workflows/pages.yml`. También puede ejecutarse manualmente desde Actions. Sólo se publican los HTML, CSS, icono, robots y sitemap; la documentación y el workflow no se incluyen en el artefacto público.

Para previsualizar, ejecutar `python -m http.server 8080` y abrir http://localhost:8080/.

## Dominio propio

Cuando se elija un dominio, configurarlo en Settings → Pages → Custom domain y añadir los registros DNS indicados por GitHub. Activar HTTPS. Actualizar las URLs absolutas de canonical, Open Graph y sitemap en las tres páginas, además de este README. Conservar los enlaces relativos; verificar las tres rutas después del cambio. No se configura un dominio provisional inventado.
