# Unificar autores con .mailmap

Si una persona aparece con dos nombres o correos, `.mailmap` los une sin reescribir la historia:

```
Edgar Ontiveros <correo@actual.com> <correo@viejo.com>
Edgar Ontiveros <correo@actual.com> edgar <edgar@laptop.local>
```

Lo usan `git shortlog`, `git blame` y `git log` con `--use-mailmap`:

```bash
git shortlog -sne
git check-mailmap "edgar <edgar@laptop.local>"
```

---

[← Volver al índice](../README.md)
