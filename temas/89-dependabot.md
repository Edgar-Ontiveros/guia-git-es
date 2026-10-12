# Mantener dependencias al día con Dependabot

Crea `.github/dependabot.yml`:

```yaml
version: 2
updates:
  - package-ecosystem: pip
    directory: "/"
    schedule:
      interval: weekly
  - package-ecosystem: github-actions
    directory: "/"
    schedule:
      interval: monthly
```

Dependabot abre PRs con las actualizaciones. Activa también las alertas de seguridad en *Settings → Code security*.

---

[← Volver al índice](../README.md)
