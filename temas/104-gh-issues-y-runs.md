# Issues y workflows con GitHub CLI

```bash
gh issue create --title "Error en reporte" --label bug
gh issue list --assignee @me
gh issue develop 12 --checkout     # crea una rama ligada al issue
gh issue close 12 --comment "Resuelto en #15"

gh run list --limit 5
gh run watch                       # sigue en vivo la ejecución
gh run view --log-failed           # solo los logs de los pasos que fallaron
gh run rerun --failed
```

---

[← Volver al índice](../README.md)
