# Descartar cambios en un archivo

Volver un archivo al estado del último commit:

```bash
git restore archivo.txt
git restore .               # todos los archivos modificados
```

Traer un archivo tal como estaba en otra rama o commit:

```bash
git restore --source main archivo.txt
git restore --source HEAD~3 archivo.txt
```

Los cambios descartados así no se pueden recuperar con Git: nunca estuvieron en un commit.

---

[← Volver al índice](../README.md)
