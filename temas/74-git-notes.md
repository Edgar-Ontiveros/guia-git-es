# Notas en commits

Las notas agregan información a un commit sin cambiar su hash:

```bash
git notes add -m "Desplegado en producción el 2026-10-01" a1b2c3d
git log -1 a1b2c3d          # la nota aparece debajo del mensaje
git notes edit a1b2c3d
git notes remove a1b2c3d
```

No se suben solas:

```bash
git push origin refs/notes/*
git fetch origin refs/notes/*:refs/notes/*
```

---

[← Volver al índice](../README.md)
