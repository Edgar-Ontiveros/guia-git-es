# Permisos del token y OIDC en Actions

Da a cada workflow solo los permisos que necesita:

```yaml
permissions:
  contents: read
```

Para desplegar en la nube sin guardar llaves de larga duración, usa OIDC:

```yaml
permissions:
  id-token: write
  contents: read
steps:
  - uses: aws-actions/configure-aws-credentials@v4
    with:
      role-to-assume: arn:aws:iam::123456789012:role/despliegue-github
      aws-region: us-east-1
```

El rol en la nube confía solo en tu repo (y si quieres, solo en la rama `main`).

---

[← Volver al índice](../README.md)
