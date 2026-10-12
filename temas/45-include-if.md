# Configuración por carpeta con includeIf

Que todo lo que esté en `~/trabajo/` use tu correo del trabajo, sin configurarlo repo por repo:

```ini
# ~/.gitconfig
[user]
  name = Tu Nombre
  email = personal@ejemplo.com

[includeIf "gitdir:~/trabajo/"]
  path = ~/.gitconfig-trabajo
```

```ini
# ~/.gitconfig-trabajo
[user]
  email = tu.nombre@empresa.com
```

La diagonal final en `gitdir:~/trabajo/` es importante: hace que aplique a todas las subcarpetas.

---

[← Volver al índice](../README.md)
