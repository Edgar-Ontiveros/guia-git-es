# Probar varias versiones con una matriz

```yaml
jobs:
  pruebas:
    strategy:
      fail-fast: false
      matrix:
        os: [ubuntu-latest, windows-latest]
        python-version: ["3.11", "3.12", "3.13"]
    runs-on: ${{ matrix.os }}
    steps:
      - uses: actions/checkout@v4
      - uses: actions/setup-python@v5
        with:
          python-version: ${{ matrix.python-version }}
      - run: pytest
```

Esto crea 6 trabajos en paralelo. `fail-fast: false` deja que terminen los demás aunque uno falle.

---

[← Volver al índice](../README.md)
