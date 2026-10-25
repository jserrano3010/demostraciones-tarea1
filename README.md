# Demostraciones – Tarea 1 (Jupyter Book)

**Estudiante:** Jairo Andrés Serrano Meléndez · **Profesor:** PhD. Lihki Rubio · Machine Learning

## Compilar localmente
```bash
pip install -r requirements.txt
jupyter-book build .
```
Luego abrir `_build/html/index.html` en el navegador.

## Publicar en GitHub Pages
1. Crear un repositorio en GitHub y subir esta carpeta a la rama `main`.
2. En el repositorio: **Settings → Pages → Source: GitHub Actions**.
3. Cada `push` a `main` compila y publica el libro automáticamente.

## Estructura
- `_config.yml` – configuración (incluye las macros LaTeX para MathJax)
- `_toc.yml` – tabla de contenido
- `intro.md` – portada
- `01.md` … `08.md` – un capítulo por demostración
- `figuras/` – capturas de los enunciados
