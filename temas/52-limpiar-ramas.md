# Limpiar ramas viejas

Quitar referencias a ramas remotas que ya se borraron:

```bash
git fetch --prune
git config --global fetch.prune true      # que lo haga siempre
```

Borrar ramas locales ya fusionadas en `main`:

```bash
git branch --merged main | grep -vE '^\*|^\s*main$' | xargs -r git branch -d
```

Ver ramas locales cuyo remoto desapareció:

```bash
git branch -vv | grep ': gone]'
```

---

[← Volver al índice](../README.md)
