# Encontrar el commit que rompió algo

`git bisect` hace búsqueda binaria entre un commit bueno y uno malo:

```bash
git bisect start
git bisect bad                 # el commit actual falla
git bisect good v1.4.0         # esta versión funcionaba
# Git te cambia a un commit intermedio; pruebas y dices:
git bisect good    # o
git bisect bad
# ...hasta que Git te dice cuál fue el primer commit malo
git bisect reset
```

Si tienes una prueba automática, Git lo hace solo:

```bash
git bisect run ./probar.sh
```

---

[← Volver al índice](../README.md)
