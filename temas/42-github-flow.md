# Flujo de trabajo con ramas y PRs (GitHub flow)

Un flujo simple que funciona para casi cualquier equipo:

1. `main` siempre está lista para desplegar.
2. Cada cambio sale de una rama nueva: `git switch -c feat/descripcion`.
3. Commits pequeños con mensajes claros.
4. `git push -u origin feat/descripcion` y abre un PR.
5. Revisión y pruebas automáticas (GitHub Actions) en el PR.
6. Merge a `main` y borra la rama.
7. Despliega desde `main`.

Protege `main` en *Settings → Branches* para exigir PR y pruebas en verde antes de integrar.

---

[← Volver al índice](../README.md)
