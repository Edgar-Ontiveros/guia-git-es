# Mover un repositorio sin red con git bundle

Un bundle es un archivo con commits que se puede clonar como si fuera un remoto:

```bash
git bundle create repo.bundle --all
# copiar repo.bundle por USB, correo, etc.
git clone repo.bundle repo
```

Para enviar solo lo nuevo:

```bash
git bundle create cambios.bundle v1.0.0..main
git bundle verify cambios.bundle
git fetch cambios.bundle main:actualizacion
```

---

[← Volver al índice](../README.md)
