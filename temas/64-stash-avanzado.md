# Stash: trucos útiles

```bash
git stash show -p stash@{0}             # ver el contenido de un stash
git stash push -m "solo config" -- config.yml   # guardar solo un archivo
git stash push --staged                 # guardar solo lo que está en staging
git stash branch prueba stash@{0}       # crea una rama desde el stash y lo aplica
git stash clear                         # borra todos (sin confirmación)
```

`git stash branch` es la salida limpia cuando un `stash pop` da conflictos porque la rama avanzó mucho.

---

[← Volver al índice](../README.md)
