# Historial de una función con log -L

`git log -L` muestra cómo evolucionó un rango de líneas o una función, commit por commit:

```bash
git log -L :calcular_total:ventas.py
git log -L 40,60:ventas.py
git log -L '/def calcular_total/,+20:ventas.py'
```

Es más preciso que `git blame` cuando quieres entender **cómo** llegó una función a su forma actual.

---

[← Volver al índice](../README.md)
