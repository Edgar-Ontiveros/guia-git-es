# Ver el historial de forma legible

```bash
git log --oneline
git log --oneline --graph --all --decorate
git log -5                      # los últimos 5
git log --since="2 weeks ago"
git log --author="Edgar"
git log -- ruta/archivo.py      # solo commits que tocaron ese archivo
git log -p archivo.py           # con el diff de cada commit
```

Un alias cómodo:

```bash
git config --global alias.lg "log --oneline --graph --all --decorate"
```

---

[← Volver al índice](../README.md)
