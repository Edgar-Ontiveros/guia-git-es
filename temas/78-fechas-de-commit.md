# Fecha de autor y fecha de commit

Cada commit tiene dos fechas:

- **Autor**: cuándo se escribió el cambio.
- **Commit**: cuándo se aplicó (cambia con `rebase`, `cherry-pick` o `--amend`).

```bash
git log --format="%h  autor: %ad  commit: %cd" --date=iso
git commit --date="2026-10-01 10:00"           # fija la fecha de autor
git rebase --committer-date-is-author-date main
```

GitHub ordena la lista de commits por fecha de commit.

---

[← Volver al índice](../README.md)
