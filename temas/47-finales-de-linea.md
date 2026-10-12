# Finales de línea (LF y CRLF)

Windows usa CRLF y Linux/macOS usan LF. Si no se controla, cada archivo aparece "modificado entero".

La forma más confiable es un `.gitattributes` en el repo:

```gitattributes
* text=auto
*.sh  text eol=lf
*.bat text eol=crlf
```

Si el repo ya tenía archivos mezclados, normalízalos una vez:

```bash
git add --renormalize .
git commit -m "Normaliza finales de línea"
```

Como respaldo individual: `core.autocrlf=true` en Windows e `input` en Linux/macOS.

---

[← Volver al índice](../README.md)
