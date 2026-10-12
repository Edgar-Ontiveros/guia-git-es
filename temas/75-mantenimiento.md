# Mantenimiento del repositorio

```bash
git count-objects -vH       # cuánto ocupa el repo
git gc                      # compacta y limpia objetos sueltos
git fsck                    # verifica la integridad
git maintenance start       # tareas automáticas en segundo plano
```

`git maintenance start` programa tareas como `prefetch` y `commit-graph`, que aceleran `fetch`, `log` y `status` en repos grandes.

---

[← Volver al índice](../README.md)
