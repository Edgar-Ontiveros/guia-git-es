# Crear o clonar un repositorio

Empezar un proyecto nuevo desde una carpeta existente:

```bash
cd mi-proyecto
git init
git add .
git commit -m "Primer commit"
```

Traer un repositorio que ya existe:

```bash
git clone https://github.com/usuario/repo.git
git clone https://github.com/usuario/repo.git otra-carpeta   # con otro nombre
git clone --depth 1 https://github.com/usuario/repo.git       # solo el último estado, más rápido
```

`git clone` ya deja configurado el remoto `origin` y la rama principal.

---

[← Volver al índice](../README.md)
