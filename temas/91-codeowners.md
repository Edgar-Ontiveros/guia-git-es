# Responsables del código con CODEOWNERS

Crea `.github/CODEOWNERS` para pedir revisión automática a quien conoce cada parte:

```
*               @usuario-lider
/docs/          @org/equipo-docs
*.sql           @usuario-dba
/.github/       @usuario-devops
```

La **última** regla que coincide es la que gana. Combínalo con la regla "Require review from Code Owners" para que su aprobación sea obligatoria.

---

[← Volver al índice](../README.md)
