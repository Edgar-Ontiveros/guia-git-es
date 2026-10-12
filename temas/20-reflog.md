# Recuperar commits "perdidos"

`git reflog` registra a dónde ha apuntado `HEAD`, incluso después de un `reset --hard` o de borrar una rama:

```bash
git reflog
# a1b2c3d HEAD@{3}: commit: Agrega reporte mensual
git switch -c rescate a1b2c3d
```

También sirve para deshacer un rebase que salió mal:

```bash
git reset --hard HEAD@{5}
```

El reflog es local y caduca (por defecto 90 días), así que no lo dejes para después.

---

[← Volver al índice](../README.md)
