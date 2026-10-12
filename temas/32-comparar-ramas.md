# Comparar ramas

```bash
git diff main..feat/login                  # diferencias de contenido
git diff main..feat/login -- src/app.py    # solo un archivo
git diff --name-only main..feat/login      # solo nombres
git diff --stat main..feat/login           # resumen
git log --oneline main..feat/login         # commits que tiene la rama y main no
git diff main...feat/login                 # lo que cambió la rama desde que salió de main
```

Dos puntos compara las puntas; tres puntos compara contra el ancestro común (es lo que muestra un PR).

---

[← Volver al índice](../README.md)
