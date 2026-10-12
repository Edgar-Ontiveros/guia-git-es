# Archivos grandes con Git LFS

Git no maneja bien binarios pesados (videos, modelos, PSD). Git LFS los guarda aparte y deja un puntero en el repo:

```bash
git lfs install
git lfs track "*.psd"
git lfs track "modelos/*.bin"
git add .gitattributes
git add archivo.psd
git commit -m "Agrega diseño con LFS"
```

GitHub rechaza archivos de más de 100 MB en un push normal; con LFS sí se pueden subir (con cuota).

---

[← Volver al índice](../README.md)
