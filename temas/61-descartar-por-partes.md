# Descartar o sacar cambios por partes

Así como `git add -p` agrega por bloques, también puedes descartar por bloques:

```bash
git restore -p archivo.py            # descarta solo los bloques que elijas
git restore --staged -p archivo.py   # saca de staging solo algunos bloques
git stash push -p                    # guarda en stash solo algunos bloques
```

Recuerda: lo descartado con `restore` no se puede recuperar.

---

[← Volver al índice](../README.md)
