# Empujar con seguridad

Después de un `rebase` o `--amend` necesitas reescribir la rama remota. No uses `--force` a secas:

```bash
git push --force-with-lease
```

`--force-with-lease` se niega a sobrescribir si alguien más subió commits que tú no has descargado. Es la versión segura.

Nunca reescribas `main` ni ramas compartidas sin avisar al equipo.

---

[← Volver al índice](../README.md)
