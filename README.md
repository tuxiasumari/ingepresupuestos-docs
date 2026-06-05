# Manual de IngePresupuestos (docs)

Sitio de documentación de usuario, hecho con [MkDocs Material](https://squidfunk.github.io/mkdocs-material/).

## Desarrollo local

```bash
python3 -m venv venv
venv/bin/pip install -r requirements.txt
venv/bin/mkdocs serve        # http://127.0.0.1:8000
```

Editar el contenido en `docs/` (Markdown). La navegación se define en `mkdocs.yml`.

## Publicar (Cloudflare Pages)

- **Build command:** `pip install -r requirements.txt && mkdocs build`
- **Output directory:** `site`
- **Dominio:** docs.ingepresupuestos.com
