# Nombrar versiones con git describe

`git describe` da un nombre legible al commit actual a partir de la última etiqueta:

```bash
git describe --tags
# v1.4.0-12-ga1b2c3d  →  12 commits después de v1.4.0, en el commit a1b2c3d
git describe --tags --always --dirty
# agrega "-dirty" si hay cambios sin commit
```

Es común usarlo para imprimir la versión en un build o en la pantalla de "Acerca de".

---

[← Volver al índice](../README.md)
