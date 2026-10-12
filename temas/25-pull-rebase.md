# pull con rebase

Evita commits de merge innecesarios del tipo "Merge branch 'main' of …":

```bash
git pull --rebase
```

Hazlo el comportamiento por defecto:

```bash
git config --global pull.rebase true
git config --global rebase.autoStash true   # guarda y restaura cambios sin commit
```

Si prefieres que `pull` falle cuando no puede avanzar en línea recta:

```bash
git config --global pull.ff only
```

---

[← Volver al índice](../README.md)
