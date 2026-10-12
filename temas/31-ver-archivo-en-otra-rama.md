# Ver un archivo de otra rama o commit

Sin cambiar de rama:

```bash
git show main:src/config.py
git show v1.0.0:README.md
git show HEAD~2:package.json > package.viejo.json
```

Listar los archivos de otra rama:

```bash
git ls-tree -r --name-only feat/login
```

---

[← Volver al índice](../README.md)
