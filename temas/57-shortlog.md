# Resumen de commits por autor

```bash
git shortlog -sn                   # número de commits por persona
git shortlog -sn --no-merges
git shortlog -sne                  # con correo
git shortlog -sn --since="1 month ago"
git shortlog v1.0.0..v1.1.0        # quién hizo qué entre dos versiones
```

Útil para notas de versión y para detectar a la misma persona con dos correos (ver el tema de `.mailmap`).

---

[← Volver al índice](../README.md)
