# Conectarte a GitHub por SSH

Con SSH no tienes que escribir usuario ni token en cada `push`.

```bash
ssh-keygen -t ed25519 -C "tu-correo@ejemplo.com"
eval "$(ssh-agent -s)"
ssh-add ~/.ssh/id_ed25519
gh ssh-key add ~/.ssh/id_ed25519.pub --title "Laptop"   # o pégala en Settings → SSH and GPG keys
ssh -T git@github.com                                   # prueba la conexión
```

Cambia un repositorio que ya usaba HTTPS:

```bash
git remote set-url origin git@github.com:usuario/repo.git
```

---

[← Volver al índice](../README.md)
