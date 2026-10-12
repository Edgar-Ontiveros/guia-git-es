# Personalizar la salida de git log

```bash
git log --format="%h %ad %an  %s" --date=short
git log --format="%h %<(15,trunc)%an %ar  %s"
git log --pretty=fuller -1
```

Marcadores útiles:

| Marcador | Significado |
|---|---|
| `%h` / `%H` | hash corto / completo |
| `%an` / `%ae` | nombre / correo del autor |
| `%ad` / `%ar` | fecha / fecha relativa |
| `%s` | asunto del commit |
| `%d` | ramas y etiquetas que apuntan ahí |

---

[← Volver al índice](../README.md)
