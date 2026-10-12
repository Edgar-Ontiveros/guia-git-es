# Encontrar el ancestro común

El ancestro común es el commit donde dos ramas se separaron:

```bash
git merge-base main feat/login
git diff $(git merge-base main feat/login) feat/login   # igual a main...feat/login
```

¿Ya está integrado un commit en otra rama?

```bash
git merge-base --is-ancestor a1b2c3d main && echo "sí está en main"
git branch --contains a1b2c3d
```

---

[← Volver al índice](../README.md)
