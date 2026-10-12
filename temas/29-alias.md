# Alias útiles

```bash
git config --global alias.st "status -s"
git config --global alias.co "switch"
git config --global alias.br "branch"
git config --global alias.lg "log --oneline --graph --all --decorate"
git config --global alias.last "log -1 HEAD --stat"
git config --global alias.unstage "restore --staged"
git config --global alias.amend "commit --amend --no-edit"
```

Luego: `git st`, `git lg`, `git amend`. Los alias viven en `~/.gitconfig`, en la sección `[alias]`.

---

[← Volver al índice](../README.md)
