# Fusionar ramas

Traer los cambios de una rama a la actual:

```bash
git switch main
git merge feat/login
```

Opciones comunes:

- `--no-ff` siempre crea un commit de merge (deja visible que hubo una rama).
- `--ff-only` solo fusiona si no hace falta commit de merge; si no, falla.
- `--squash` junta todo en un solo cambio que tú confirmas con `git commit`.

Si algo sale mal a la mitad: `git merge --abort`.

---

[← Volver al índice](../README.md)
