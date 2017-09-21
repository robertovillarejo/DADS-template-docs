# DADS-template-docs
Ésta es una plantilla para generar la documentación de los proyectos de la DADS Infotec.

# Instalación (Getting Started)
Necesitarás tener instalado:
- [Python](https://www.python.org/downloads/)
- [Sphinx](http://www.sphinx-doc.org)
- [recommonmark](https://github.com/rtfd/recommonmark)

- Instalación de Sphinx:  
  `pip install sphinx sphinx-autobuild`

- Instalación de recommonmark:  
  `pip install recommonmark`

# Uso

1. En la carpeta raíz de tu proyecto, copia la carpeta `docs` de este repositorio.
2. Dentro de `docs`, ejecuta el siguiente comando:
  ```
  sphinx-quickstart --quiet --sep \
  --project="Mi proyecto" \
  --author="Roberto Villarejo Martinez" \
  -v 0.1 \
  --release 0.1 \
  --language=es \
  --makefile \
  --batchfile \
  -t template-DADS .
  ```  

  - Deberás modificar los siguientes parámetros:

  `--project`: El nombre de tu proyecto  
  `--author`: El nombre del autor  
  `-v`: El número de la versión  
  `--release`: El número del _release_ (Probablemente lo manejes como igual a la versión)  
  `--language`: El idioma en que escribes la documentación  

3. Escribe la documentación en los siguientes archivos que se encuentran en `docs/source`:
  - description.md
  - getting-started.md
  - usage.md
  - FAQs.md
  - license.md
  - known-issues.md
  - contributing.md
  - about-developer.md

4. Genera los archivos html ejecutando `make html` dentro de la carpeta `docs`

5. Verifica el sitio generado abriendo el archivo `/docs/build/html/index.html`
