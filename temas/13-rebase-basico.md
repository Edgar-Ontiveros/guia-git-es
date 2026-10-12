# Rebase básico

`rebase` mueve tus commits para que queden encima de otra rama, con una historia lineal:

```bash
git switch feat/login
git rebase main
```

Si hay conflictos, resuélvelos y sigue:

```bash
git add archivo-resuelto
git rebase --continue
git rebase --abort      # para cancelar todo
```

Regla de oro: no hagas rebase de commits que otras personas ya descargaron.

---

[← Volver al índice](../README.md)
