# Ramas: crear, cambiar y borrar

```bash
git branch                    # lista ramas locales
git branch -a                 # incluye las remotas
git switch -c feat/login      # crea y cambia a la rama
git switch main               # cambia de rama
git switch -                  # regresa a la rama anterior
git branch -d feat/login      # borra (solo si ya está fusionada)
git branch -D feat/login      # borra aunque no esté fusionada
git push origin --delete feat/login   # borra la rama remota
```

Nombra las ramas por intención: `feat/…`, `fix/…`, `docs/…`.

---

[← Volver al índice](../README.md)
