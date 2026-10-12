# Qué commits faltan por llevar a otra rama

```bash
git cherry -v main feat/login
```

- `+` el commit no tiene equivalente en `main`.
- `-` ya existe un cambio equivalente (por ejemplo, se le hizo `cherry-pick`).

Variante con `log`:

```bash
git log --oneline --cherry-pick --right-only main...feat/login
```

Útil para saber qué correcciones faltan en una rama de versión.

---

[← Volver al índice](../README.md)
