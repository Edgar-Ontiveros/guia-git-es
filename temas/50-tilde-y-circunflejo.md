# HEAD~ y HEAD^: cómo moverse entre commits

- `HEAD~1` (o `HEAD~`): el padre del commit actual.
- `HEAD~3`: tres commits hacia atrás, siguiendo siempre el primer padre.
- `HEAD^` es igual a `HEAD~1`.
- `HEAD^2`: el **segundo padre** de un commit de merge (la rama que se integró).

```bash
git show HEAD~2
git diff HEAD^1 HEAD^2      # en un merge: compara las dos ramas que se unieron
git log main~5..main        # los últimos 5 commits de main
```

---

[← Volver al índice](../README.md)
