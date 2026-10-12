# Guardar credenciales HTTPS

GitHub ya no acepta tu contraseña en `git push` por HTTPS; pide un token. Para no escribirlo cada vez:

```bash
gh auth login
gh auth setup-git            # Git usa la sesión de GitHub CLI
```

Otras opciones:

```bash
git config --global credential.helper "cache --timeout=3600"   # en memoria, 1 hora
git config --global credential.helper store                    # en disco, en TEXTO PLANO
```

En Windows, Git Credential Manager viene con Git for Windows y guarda el token en el almacén del sistema.

---

[← Volver al índice](../README.md)
