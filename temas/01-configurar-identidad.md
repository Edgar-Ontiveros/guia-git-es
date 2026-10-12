# Configurar tu identidad

Git firma cada commit con un nombre y un correo. Configúralos una vez por equipo:

```bash
git config --global user.name "Tu Nombre"
git config --global user.email "tu-correo@ejemplo.com"
git config --global init.defaultBranch main
```

Para un repositorio concreto (por ejemplo, uno del trabajo) omite `--global` y se guarda solo en ese repo.

Revisa lo que tienes configurado y de dónde sale cada valor:

```bash
git config --list --show-origin
```

> En GitHub, el correo del commit debe estar vinculado a tu cuenta para que el commit cuente en tu perfil. Si no quieres exponer tu correo, usa el `@users.noreply.github.com` que GitHub te asigna.

---

[← Volver al índice](../README.md)
