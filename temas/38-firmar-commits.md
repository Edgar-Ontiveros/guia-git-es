# Firmar commits con SSH

GitHub muestra la etiqueta **Verified** en commits firmados. Puedes firmar con tu llave SSH:

```bash
git config --global gpg.format ssh
git config --global user.signingkey ~/.ssh/id_ed25519.pub
git config --global commit.gpgsign true
git config --global tag.gpgsign true
```

Luego sube la misma llave en GitHub → *Settings → SSH and GPG keys → New SSH key* con tipo **Signing key**.

Verifica: `git log --show-signature -1`.

---

[← Volver al índice](../README.md)
