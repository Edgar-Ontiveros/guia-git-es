# Datos del repo para scripts con rev-parse

```bash
git rev-parse --show-toplevel        # carpeta raíz del repo
git rev-parse --abbrev-ref HEAD      # nombre de la rama actual
git rev-parse --short HEAD           # hash corto del commit actual
git rev-parse --is-inside-work-tree  # true si estás dentro de un repo
git rev-parse main~3                 # hash completo de una referencia
```

Ejemplo en un script de despliegue:

```bash
VERSION="$(git describe --tags --always)-$(git rev-parse --short HEAD)"
```

---

[← Volver al índice](../README.md)
