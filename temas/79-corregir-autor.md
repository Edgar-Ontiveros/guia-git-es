# Corregir el autor de commits

Del último commit:

```bash
git commit --amend --author="Tu Nombre <correo@ejemplo.com>" --no-edit
git commit --amend --reset-author --no-edit     # usa tu user.name/user.email actuales
```

De varios commits de tu rama (reescribe historia):

```bash
git rebase --exec 'git commit --amend --no-edit --reset-author' main
git push --force-with-lease
```

Antes de esto, configura bien `user.email` para que no vuelva a pasar.

---

[← Volver al índice](../README.md)
