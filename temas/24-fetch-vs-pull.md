# fetch vs pull

- `git fetch` descarga lo nuevo del remoto **sin tocar** tu rama.
- `git pull` hace `fetch` y luego integra (merge o rebase) en tu rama.

```bash
git fetch origin
git log --oneline main..origin/main   # qué llegó y aún no tienes
git diff main origin/main             # qué cambiaría
git merge origin/main                 # cuando estés listo
```

Hacer `fetch` primero te deja revisar antes de mezclar.

---

[← Volver al índice](../README.md)
