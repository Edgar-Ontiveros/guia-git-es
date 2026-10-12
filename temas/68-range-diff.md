# Comparar dos versiones de una rama

Después de un rebase o de corregir commits, `range-diff` muestra qué cambió entre la versión vieja y la nueva de la serie:

```bash
git range-diff main feat/login@{1} feat/login
```

`feat/login@{1}` es la rama antes de la última operación (sale del reflog). Muy útil para revisar un PR al que le hicieron force-push.

---

[← Volver al índice](../README.md)
