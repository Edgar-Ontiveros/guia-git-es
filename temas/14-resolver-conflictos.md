# Resolver conflictos

Cuando dos ramas cambian las mismas líneas, Git marca el archivo así:

```
<<<<<<< HEAD
precio = 100
=======
precio = 120
>>>>>>> feat/precios
```

Pasos:

1. Edita el archivo y deja la versión correcta (borra las marcas).
2. `git add archivo`
3. `git commit` (en merge) o `git rebase --continue` (en rebase).

Atajos para quedarte con un lado completo:

```bash
git checkout --ours archivo     # tu versión
git checkout --theirs archivo   # la versión que estás integrando
```

---

[← Volver al índice](../README.md)
