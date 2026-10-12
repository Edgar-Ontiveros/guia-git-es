# Quitar un secreto del historial

Si subiste una contraseña o llave:

1. **Revócala o cámbiala primero.** Si ya estuvo en GitHub, considérala expuesta.
2. Elimínala del historial con `git filter-repo`:

```bash
pip install git-filter-repo
git filter-repo --invert-paths --path config/secreto.env    # borra el archivo de todo el historial
git filter-repo --replace-text reemplazos.txt               # o reemplaza el texto
git push --force --all
git push --force --tags
```

3. Pide a quienes tengan clones que vuelvan a clonar.

---

[← Volver al índice](../README.md)
