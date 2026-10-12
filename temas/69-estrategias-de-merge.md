# -X ours, -X theirs y -s ours

```bash
git merge -X theirs feat/precios   # en los conflictos gana la otra rama; lo demás se fusiona normal
git merge -X ours feat/precios     # en los conflictos ganas tú
git merge -s ours rama-vieja       # registra el merge pero IGNORA todos los cambios de la otra rama
```

`-X` (opción) y `-s` (estrategia) son muy distintos: `-s ours` descarta todo lo de la otra rama.

En un **rebase**, "ours" y "theirs" se invierten: "ours" es la rama sobre la que estás reaplicando.

---

[← Volver al índice](../README.md)
