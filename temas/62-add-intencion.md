# Ver archivos nuevos en git diff

`git diff` no muestra archivos nuevos que aún no agregas. Márcalos con "intención de agregar":

```bash
git add -N nuevo.py
git diff                 # ahora sí aparece todo su contenido
git add -p nuevo.py      # y puedes agregarlo por partes
```

`-N` registra el archivo vacío en el índice; el contenido entra hasta que hagas `git add`.

---

[← Volver al índice](../README.md)
