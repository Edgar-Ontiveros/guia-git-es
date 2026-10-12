# Limpiar archivos no rastreados

`git clean` borra archivos que Git no rastrea. Siempre empieza con una prueba en seco:

```bash
git clean -n          # muestra qué borraría
git clean -fd         # borra archivos y carpetas no rastreados
git clean -fdx        # además los ignorados (node_modules, builds…)
git clean -i          # modo interactivo
```

Lo que borra `git clean` no se puede recuperar con Git.

---

[← Volver al índice](../README.md)
