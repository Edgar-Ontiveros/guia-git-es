# switch y restore en lugar de checkout

`git checkout` hace demasiadas cosas. Desde Git 2.23 hay comandos separados:

| Antes | Ahora |
|---|---|
| `git checkout rama` | `git switch rama` |
| `git checkout -b nueva` | `git switch -c nueva` |
| `git checkout -- archivo` | `git restore archivo` |
| `git checkout main -- archivo` | `git restore --source main archivo` |
| `git reset HEAD archivo` | `git restore --staged archivo` |

Los comandos nuevos hacen más difícil borrar cambios por accidente.

---

[← Volver al índice](../README.md)
