# Correcciones automáticas con fixup y autosquash

Encontraste un error en un commit anterior de tu rama:

```bash
git add archivo.py
git commit --fixup a1b2c3d
git rebase -i --autosquash main
```

Git acomoda el commit `fixup!` justo debajo del original y lo une al guardar. Actívalo siempre:

```bash
git config --global rebase.autoSquash true
```

---

[← Volver al índice](../README.md)
