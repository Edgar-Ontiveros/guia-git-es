# Ver el estado y las diferencias

Antes de hacer commit, revisa qué cambió:

```bash
git status            # qué archivos cambiaron y en qué zona están
git status -s         # versión corta
git diff              # cambios que aún NO están en staging
git diff --staged     # cambios que SÍ van en el próximo commit
git diff --stat       # resumen por archivo
```

Regla práctica: `git diff --staged` justo antes de `git commit` evita subir cosas que no querías.

---

[← Volver al índice](../README.md)
