# Acelerar workflows con caché

Muchas acciones de configuración ya traen caché integrada:

```yaml
- uses: actions/setup-python@v5
  with:
    python-version: "3.12"
    cache: pip
```

Para cualquier otra carpeta:

```yaml
- uses: actions/cache@v4
  with:
    path: ~/.cache/mi-herramienta
    key: ${{ runner.os }}-mi-herramienta-${{ hashFiles('**/lockfile') }}
    restore-keys: ${{ runner.os }}-mi-herramienta-
```

La `key` cambia cuando cambia el lockfile, así la caché se renueva sola.

---

[← Volver al índice](../README.md)
