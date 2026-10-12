# Aplicar un commit específico

Copiar un commit de otra rama a la actual, sin traer todo lo demás:

```bash
git cherry-pick a1b2c3d
git cherry-pick a1b2c3d e4f5g6h      # varios
git cherry-pick -x a1b2c3d           # anota de dónde vino en el mensaje
```

Útil para llevar una corrección urgente a una rama de versión. Si hay conflicto: resuelve, `git add` y `git cherry-pick --continue`.

---

[← Volver al índice](../README.md)
