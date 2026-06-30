# Alpha Book

Diccionario juvenil moderno con **Modo Joven** y **Modo Guía** para padres y educadores.

## Demo local

Abre `index.html` en el navegador, o usa un servidor local:

```bash
npx serve .
```

## Publicar en GitHub Pages

1. Crea un repositorio en GitHub (por ejemplo `alpha-book`).
2. Sube estos archivos a la rama `main`:
   - `index.html` (entrada del sitio)
   - `.nojekyll`
   - `.github/workflows/pages.yml`
3. En el repo: **Settings → Pages → Build and deployment**
   - Source: **GitHub Actions**
4. Haz push a `main`. El workflow **Deploy to GitHub Pages** publicará el sitio.

Tu URL será:

```text
https://TU_USUARIO.github.io/NOMBRE_DEL_REPO/
```

Ejemplo: `https://dinoj.github.io/alpha-book/`

### Enlaces directos a palabras

Funcionan con hash en la URL:

```text
https://TU_USUARIO.github.io/alpha-book/#cringe
```

## Estructura

| Archivo | Uso |
|---------|-----|
| `index.html` | Sitio completo (GitHub Pages) |
| `alpha_book_dictionary (1).html` | Copia de trabajo local (opcional) |

Edita `index.html` (o mantén ambos archivos sincronizados) cuando hagas cambios.

## Notas

- No requiere build: HTML + Tailwind CDN + Font Awesome.
- Los datos del usuario (palabras añadidas) se guardan en `localStorage` del navegador.
