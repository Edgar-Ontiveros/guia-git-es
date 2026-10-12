# Deshacer el último commit

Depende de qué quieras conservar:

```bash
git reset --soft HEAD~1    # quita el commit, los cambios quedan en staging
git reset HEAD~1           # quita el commit, los cambios quedan sin preparar
git reset --hard HEAD~1    # quita el commit y BORRA los cambios
```

`--hard` no tiene "deshacer" fácil (salvo con `git reflog`). Úsalo solo si estás seguro.

Si el commit ya está publicado y otros lo tienen, mejor usa `git revert`.

---

[← Volver al índice](../README.md)
