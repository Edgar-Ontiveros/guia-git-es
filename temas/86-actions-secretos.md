# Secretos y variables en GitHub Actions

Guárdalos en *Settings → Secrets and variables → Actions* o desde la terminal:

```bash
gh secret set API_KEY
gh variable set ENTORNO --body produccion
```

Úsalos en el workflow:

```yaml
- run: ./desplegar.sh
  env:
    API_KEY: ${{ secrets.API_KEY }}
    ENTORNO: ${{ vars.ENTORNO }}
```

GitHub oculta los secretos en los logs, y los PRs que vienen de forks no los reciben.

---

[← Volver al índice](../README.md)
