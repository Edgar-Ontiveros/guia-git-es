# Clones parciales y superficiales

```bash
git clone --depth 1 URL               # superficial: solo el último commit
git clone --filter=blob:none URL      # parcial: todo el historial, contenidos bajo demanda
git clone --filter=tree:0 URL         # aún más ligero (bueno para CI)
```

Si clonaste superficial y luego necesitas la historia completa:

```bash
git fetch --unshallow
```

Para trabajo diario, `--filter=blob:none` suele ser mejor que `--depth 1`: `log` y `blame` siguen funcionando.

---

[← Volver al índice](../README.md)
