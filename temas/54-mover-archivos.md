# Mover y renombrar archivos

```bash
git mv viejo.py nuevo.py
git mv src/utils.py src/comun/utils.py
```

Git no guarda "renombres": los detecta comparando contenido. Por eso conviene renombrar en un commit y modificar en otro.

Cambiar solo mayúsculas en Windows o macOS (sistemas que no distinguen mayúsculas):

```bash
git mv readme.md temp.md
git mv temp.md README.md
```

Para ver el historial completo de un archivo renombrado: `git log --follow nuevo.py`.

---

[← Volver al índice](../README.md)
