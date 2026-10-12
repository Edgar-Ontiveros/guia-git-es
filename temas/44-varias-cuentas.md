# Dos cuentas de GitHub en el mismo equipo

Usa una llave SSH por cuenta y un alias de host en `~/.ssh/config`:

```
Host github.com
  IdentityFile ~/.ssh/id_personal

Host github-trabajo
  HostName github.com
  IdentityFile ~/.ssh/id_trabajo
```

Clona los repos del trabajo con el alias:

```bash
git clone git@github-trabajo:empresa/repo.git
```

Combínalo con `includeIf` (siguiente tema) para que cada carpeta use también el correo correcto.

---

[← Volver al índice](../README.md)
