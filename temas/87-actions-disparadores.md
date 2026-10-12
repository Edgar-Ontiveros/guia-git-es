# Cuándo se ejecuta un workflow

```yaml
on:
  push:
    branches: [main]
    paths: ["src/**", "requirements.txt"]   # solo si cambian estos archivos
  pull_request:
  workflow_dispatch:                         # botón "Run workflow" y gh workflow run
    inputs:
      entorno:
        type: choice
        options: [pruebas, produccion]
  schedule:
    - cron: "0 13 * * 1-5"                   # lunes a viernes 13:00 UTC
```

```bash
gh workflow run ci.yml -f entorno=pruebas
```

Los horarios de `schedule` siempre están en UTC.

---

[← Volver al índice](../README.md)
