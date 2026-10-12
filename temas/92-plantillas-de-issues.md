# Formularios para issues

Crea `.github/ISSUE_TEMPLATE/error.yml`:

```yaml
name: Reportar un error
description: Algo no funciona como debería
labels: [bug]
body:
  - type: textarea
    id: que-paso
    attributes:
      label: ¿Qué pasó?
    validations:
      required: true
  - type: input
    id: version
    attributes:
      label: Versión
```

Y `config.yml` en la misma carpeta con `blank_issues_enabled: false` para obligar a usar los formularios.

---

[← Volver al índice](../README.md)
