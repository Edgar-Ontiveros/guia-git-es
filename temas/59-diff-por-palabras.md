# Diferencias por palabra y código movido

Para textos largos o líneas extensas, compara por palabra:

```bash
git diff --word-diff
git diff --word-diff=color
```

Para distinguir código que solo se movió de lugar:

```bash
git diff --color-moved
git config --global diff.colorMoved zebra
```

Ignorar cambios de espacios:

```bash
git diff -w
```

---

[← Volver al índice](../README.md)
