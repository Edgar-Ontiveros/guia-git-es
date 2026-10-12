# Trabajar solo con una carpeta (sparse-checkout)

En monorepos grandes puedes descargar y ver solo lo que necesitas:

```bash
git clone --filter=blob:none --sparse https://github.com/org/monorepo.git
cd monorepo
git sparse-checkout set servicios/ventas docs
git sparse-checkout add servicios/inventario
git sparse-checkout list
git sparse-checkout disable          # volver a ver todo
```

---

[← Volver al índice](../README.md)
