# Ver qué hay en un commit

```bash
git show a1b2c3d                 # mensaje y diff completo
git show --stat a1b2c3d          # solo archivos y número de líneas
git show --name-only a1b2c3d     # solo nombres de archivos
git show -s --format="%an %ad%n%s" a1b2c3d   # solo datos, sin diff
git show v1.2.0                  # una etiqueta anotada y su commit
```

`git show` también acepta rangos: `git show HEAD~2..HEAD`.

---

[← Volver al índice](../README.md)
