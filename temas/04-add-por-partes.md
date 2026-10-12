# Preparar cambios por partes

Si en un archivo hiciste dos cambios sin relación, puedes meterlos en commits distintos:

```bash
git add -p archivo.py
```

Git te muestra cada bloque (hunk) y preguntas:

- `y` lo agrega, `n` lo salta
- `s` lo divide en bloques más chicos
- `e` lo editas a mano
- `q` sales

Así cada commit cuenta una sola historia y es más fácil revisar o revertir.

---

[← Volver al índice](../README.md)
