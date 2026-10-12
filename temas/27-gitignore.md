# Ignorar archivos con .gitignore

```gitignore
# dependencias y compilados
node_modules/
__pycache__/
dist/

# secretos y configuración local
.env
*.pem

# del sistema
.DS_Store
Thumbs.db
```

Ver por qué se ignora un archivo:

```bash
git check-ignore -v ruta/archivo
```

Plantillas listas para cada lenguaje: <https://github.com/github/gitignore>.

---

[← Volver al índice](../README.md)
