# Más usos de .gitattributes

```gitattributes
*.png   binary                    # nunca intentes hacer diff ni merge de texto
*.lock  -diff                     # no muestres el diff de archivos lock
*.py    diff=python               # encabezados de función en los diffs
docs/** linguist-documentation    # no cuenta para el lenguaje del repo en GitHub
*.min.js linguist-generated       # GitHub lo oculta por defecto en los PRs
pruebas/ export-ignore            # no se incluye en git archive
```

Los atributos `linguist-*` solo los usa GitHub; los demás los usa Git en tu equipo.

---

[← Volver al índice](../README.md)
