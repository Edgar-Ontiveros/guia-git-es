# Renombrar una rama

```bash
git branch -m nombre-viejo nombre-nuevo
git push origin -u nombre-nuevo
git push origin --delete nombre-viejo
```

Para pasar de `master` a `main`, renómbrala en GitHub (*Settings → Branches*; GitHub redirige los enlaces) y en cada clon local:

```bash
git branch -m master main
git fetch origin
git branch -u origin/main main
git remote set-head origin -a
```

---

[← Volver al índice](../README.md)
