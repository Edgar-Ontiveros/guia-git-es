# Guardar trabajo temporal con stash

Necesitas cambiar de rama pero no quieres hacer commit todavía:

```bash
git stash push -m "a medio terminar"
git stash list
git stash pop            # aplica el último y lo quita de la lista
git stash apply stash@{1}  # aplica uno sin quitarlo
git stash drop stash@{1}
```

Incluye archivos nuevos (no rastreados) con `-u`:

```bash
git stash push -u -m "con archivos nuevos"
```

---

[← Volver al índice](../README.md)
