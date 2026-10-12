# Pull requests desde la terminal con GitHub CLI

```bash
gh auth login
gh pr create --title "Agrega login" --body "Detalle del cambio"
gh pr create --fill              # usa el mensaje del commit
gh pr list
gh pr checkout 42                # trae la rama de un PR
gh pr view 42 --web
gh pr merge 42 --squash --delete-branch
```

Con `gh` también manejas issues (`gh issue create`), releases (`gh release create`) y workflows (`gh run watch`).

---

[← Volver al índice](../README.md)
