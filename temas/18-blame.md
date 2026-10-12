# Saber quién cambió una línea

```bash
git blame archivo.py
git blame -L 40,60 archivo.py      # solo esas líneas
git blame -w archivo.py            # ignora cambios de espacios
git blame -C archivo.py            # detecta código movido de otros archivos
```

Si un commit de solo formato "ensucia" el blame, agrégalo a `.git-blame-ignore-revs` y configura:

```bash
git config blame.ignoreRevsFile .git-blame-ignore-revs
```

GitHub también respeta ese archivo en su vista de blame.

---

[← Volver al índice](../README.md)
