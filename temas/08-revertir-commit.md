# Revertir un commit publicado

`git revert` crea un commit nuevo que hace lo contrario de otro. No reescribe la historia, así que es seguro en ramas compartidas:

```bash
git revert a1b2c3d
git revert HEAD             # revierte el último
git revert --no-commit a1b2c3d b4c5d6e   # varios, en un solo commit
```

Para revertir un merge indica qué padre conservar:

```bash
git revert -m 1 <hash-del-merge>
```

---

[← Volver al índice](../README.md)
