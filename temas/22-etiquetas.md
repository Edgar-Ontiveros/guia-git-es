# Etiquetas y versiones

Marca versiones con etiquetas anotadas (guardan autor, fecha y mensaje):

```bash
git tag -a v1.2.0 -m "Versión 1.2.0"
git tag                         # lista
git show v1.2.0
git push origin v1.2.0          # las etiquetas no se suben solas
git push origin --tags          # todas
git tag -d v1.2.0               # borra local
git push origin --delete v1.2.0 # borra remota
```

Usa versionado semántico: `MAYOR.MENOR.PARCHE`.

---

[← Volver al índice](../README.md)
