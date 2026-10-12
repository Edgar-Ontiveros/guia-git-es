# HEAD separado (detached HEAD)

Si cambias a un commit o etiqueta en lugar de una rama, quedas en "detached HEAD":

```bash
git switch --detach v1.0.0
```

Puedes mirar y probar sin problema. Si haces commits ahí y luego cambias de rama, quedan sin rama que los sostenga. Para conservarlos:

```bash
git switch -c rescate-v1      # crea una rama donde estás
```

Si ya te fuiste, búscalos con `git reflog`.

---

[← Volver al índice](../README.md)
