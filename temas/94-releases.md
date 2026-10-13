# Publicar versiones (releases)

```bash
git tag -a v1.2.0 -m "Versión 1.2.0"
git push origin v1.2.0
gh release create v1.2.0 --generate-notes             # notas automáticas a partir de los PRs
gh release create v1.2.0 dist/*.zip --notes-file NOTAS.md   # con archivos adjuntos
gh release list
```

Agrupa las notas automáticas por etiqueta con `.github/release.yml` (por ejemplo: "Novedades" para `enhancement` y "Correcciones" para `bug`).

---

[← Volver al índice](../README.md)
