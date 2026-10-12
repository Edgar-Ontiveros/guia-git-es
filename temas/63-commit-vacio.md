# Commits vacíos

A veces necesitas un commit sin cambios, por ejemplo para volver a disparar la integración continua:

```bash
git commit --allow-empty -m "Vuelve a ejecutar CI"
git push
```

También sirve como primer commit de un repositorio para tener una raíz limpia antes de importar código.

Si solo quieres reintentar un workflow de GitHub Actions, `gh run rerun` evita ensuciar el historial.

---

[← Volver al índice](../README.md)
