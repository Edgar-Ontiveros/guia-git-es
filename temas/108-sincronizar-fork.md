# Mantener un fork al día

Desde GitHub: botón **Sync fork** en la página de tu fork.

Desde la terminal:

```bash
gh repo sync usuario/mi-fork          # actualiza el fork en GitHub desde el original
git pull                              # y luego tu copia local
```

Con Git solo:

```bash
git remote add upstream https://github.com/org/proyecto.git
git fetch upstream
git switch main
git rebase upstream/main
git push --force-with-lease
```

---

[← Volver al índice](../README.md)
