# Reutilizar resoluciones de conflictos (rerere)

`rerere` ("reuse recorded resolution") recuerda cómo resolviste un conflicto y lo aplica sola la próxima vez:

```bash
git config --global rerere.enabled true
```

Ayuda mucho cuando haces rebase de una rama larga varias veces o repites un merge de prueba.

```bash
git rerere status     # conflictos que está registrando
git rerere diff       # la resolución registrada
```

---

[← Volver al índice](../README.md)
