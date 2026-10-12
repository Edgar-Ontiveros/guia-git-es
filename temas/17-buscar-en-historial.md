# Buscar en el historial

Encontrar cuándo apareció o desapareció un texto en el código:

```bash
git log -S "calcularIVA" --oneline        # commits que cambiaron cuántas veces aparece
git log -G "IVA\s*=" --oneline            # con expresión regular
git log --grep "factura" --oneline        # busca en los mensajes
git grep "TODO"                           # busca en los archivos del commit actual
git grep "TODO" v1.2.0                    # en otra versión
```

`-S` es ideal para saber en qué commit se agregó o eliminó una función.

---

[← Volver al índice](../README.md)
