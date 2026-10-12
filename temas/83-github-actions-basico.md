# Tu primer workflow de GitHub Actions

Crea `.github/workflows/ci.yml`:

```yaml
name: CI
on:
  push:
    branches: [main]
  pull_request:

jobs:
  pruebas:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - uses: actions/setup-python@v5
        with:
          python-version: "3.12"
      - run: pip install -r requirements.txt
      - run: pytest
```

Cada push a `main` y cada PR ejecuta las pruebas; el resultado aparece en el PR.

---

[← Volver al índice](../README.md)
