# Sacar archivos del staging

Agregaste algo con `git add` que no va en este commit:

```bash
git restore --staged archivo.txt
```

El archivo conserva tus cambios, solo deja de estar preparado. En versiones viejas de Git el equivalente es:

```bash
git reset HEAD archivo.txt
```

---

[← Volver al índice](../README.md)
