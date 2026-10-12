# Trabajar con remotos

```bash
git remote -v                                 # ver remotos
git remote add upstream https://github.com/org/repo.git
git remote set-url origin git@github.com:usuario/repo.git   # cambiar a SSH
git remote rename origin github
git remote remove upstream
```

Patrón típico con un fork: `origin` es tu copia y `upstream` el repositorio original.

```bash
git fetch upstream
git rebase upstream/main
```

---

[← Volver al índice](../README.md)
