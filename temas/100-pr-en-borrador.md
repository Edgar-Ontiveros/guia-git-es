# PRs en borrador, revisores y auto-merge

```bash
gh pr create --draft --fill            # aún no está listo para revisión
gh pr ready                            # marcarlo como listo
gh pr edit --add-reviewer usuario
gh pr merge --auto --squash            # se integra solo cuando pasen pruebas y aprobaciones
gh pr checks                           # estado de las pruebas
```

`--auto` requiere activar *Allow auto-merge* en *Settings → General*.

---

[← Volver al índice](../README.md)
