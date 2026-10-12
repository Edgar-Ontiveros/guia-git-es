# Ordenar commits con rebase interactivo

Antes de abrir un PR puedes limpiar tus commits locales:

```bash
git rebase -i HEAD~4
```

Se abre una lista y cambias la palabra de cada línea:

- `pick` lo deja igual
- `reword` cambia el mensaje
- `squash` / `fixup` lo une al anterior
- `drop` lo elimina
- puedes reordenar las líneas

Solo en commits que aún no compartes. Si te pierdes: `git rebase --abort`.

---

[← Volver al índice](../README.md)
