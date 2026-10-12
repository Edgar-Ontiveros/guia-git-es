# Corregir el último commit

Olvidaste un archivo o te equivocaste en el mensaje:

```bash
git add archivo-olvidado.txt
git commit --amend              # abre el editor para cambiar el mensaje
git commit --amend --no-edit    # conserva el mensaje
```

`--amend` reemplaza el commit (cambia su hash). Si ya lo subiste, tendrás que empujar con `git push --force-with-lease`, y solo hazlo en ramas donde nadie más trabaje.

---

[← Volver al índice](../README.md)
