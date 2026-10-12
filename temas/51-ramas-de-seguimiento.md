# Ramas de seguimiento (upstream)

Una rama local puede "seguir" a una remota; así `git pull` y `git push` saben a dónde ir y `git status` te dice cuántos commits vas adelante o atrás.

```bash
git push -u origin feat/login        # publica y queda vinculada
git branch -u origin/feat/login      # vincula una rama que ya existe
git branch -vv                       # ver qué sigue cada rama y [ahead/behind]
```

Para que el primer `git push` vincule solo:

```bash
git config --global push.autoSetupRemote true
```

---

[← Volver al índice](../README.md)
