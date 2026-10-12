# Exportar el proyecto sin .git

```bash
git archive --format=zip -o proyecto.zip HEAD
git archive --format=tar.gz --prefix=proyecto-v1.2/ -o proyecto-v1.2.tar.gz v1.2.0
git archive HEAD src/ | tar -x -C /ruta/destino
```

Solo incluye lo que está en el commit (nada de archivos ignorados ni cambios sin commit). Excluye rutas con `export-ignore` en `.gitattributes`.

---

[← Volver al índice](../README.md)
