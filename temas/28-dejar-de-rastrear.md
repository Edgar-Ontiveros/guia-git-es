# Dejar de rastrear un archivo ya versionado

Agregar un archivo al `.gitignore` no basta si ya estaba en un commit. Quítalo del índice sin borrarlo del disco:

```bash
git rm --cached .env
echo ".env" >> .gitignore
git commit -m "Deja de versionar .env"
```

Para una carpeta: `git rm -r --cached carpeta/`.

> Si el archivo tenía secretos, sigue en el historial. Cambia esas credenciales: quitarlo del último commit no las protege.

---

[← Volver al índice](../README.md)
