# Trabajar en dos ramas a la vez con worktrees

En lugar de hacer `stash` y cambiar de rama, abre otra rama en otra carpeta:

```bash
git worktree add ../proyecto-hotfix fix/urgente
cd ../proyecto-hotfix      # trabajas aquí sin tocar tu carpeta principal
git worktree list
git worktree remove ../proyecto-hotfix
```

Comparten el mismo repositorio (`.git`), así que los commits se ven en ambos lados. Una rama solo puede estar abierta en un worktree a la vez.

---

[← Volver al índice](../README.md)
