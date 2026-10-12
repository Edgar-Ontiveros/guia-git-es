# Submódulos (lo básico)

Un submódulo es otro repositorio dentro del tuyo, fijado en un commit concreto:

```bash
git submodule add https://github.com/org/libreria.git libs/libreria
git clone --recurse-submodules https://github.com/usuario/repo.git
git submodule update --init --recursive    # si ya clonaste sin ellos
git submodule update --remote              # trae lo último del submódulo
```

Cuando el submódulo cambia, el repo principal registra el nuevo commit: hay que hacer `git add libs/libreria` y commit.

---

[← Volver al índice](../README.md)
