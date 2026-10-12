# Hooks de Git

Los hooks son scripts que Git ejecuta en ciertos momentos. Viven en `.git/hooks/`:

```bash
# .git/hooks/pre-commit
#!/bin/sh
if git diff --cached | grep -q "console.log"; then
  echo "Quita los console.log antes de hacer commit"
  exit 1
fi
```

```bash
chmod +x .git/hooks/pre-commit
```

`.git/hooks` no se versiona. Para compartir hooks con el equipo usa `git config core.hooksPath .githooks` o una herramienta como `pre-commit`.

---

[← Volver al índice](../README.md)
