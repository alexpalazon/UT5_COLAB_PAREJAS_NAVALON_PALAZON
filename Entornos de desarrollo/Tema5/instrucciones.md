# INSTRUCCIONES PARA TRABAJAR CON EL REPOSITORIO
#
# Este archivo explica cómo trabajar en este proyecto usando Git y GitHub.
# Todo está en un único bloque bash para poder copiar y pegar sin problemas.
#
# --------------------------------------------------
# CLONAR EL REPOSITORIO
# --------------------------------------------------
# Para obtener una copia local del repositorio, usa el siguiente comando.
# Sustituye APELLIDOS_DEL_COMPA por los apellidos del compañero que creó el repo.

git clone https://github.com/alexpalazon/UT5_COLAB_PAREJAS_NAVALON_PALAZON

# Esto crea una copia del repositorio en tu ordenador.
#
# --------------------------------------------------
# CREAR UNA RAMA
# --------------------------------------------------
# Una rama es una línea de trabajo independiente que no afecta a main.
# Siempre se debe trabajar en una rama propia.
# El siguiente comando crea la rama y cambia a ella automáticamente.

git checkout -b feature-NombreAlumnoB

# -------------------------------------------------
# HACER COMMIT
# -------------------------------------------------
# El commit guarda los cambios de forma local en tu rama.
# Primero se añaden los archivos y luego se hace el commit con mensaje etiquetado.

git add INSTRUCCIONES.md
git commit -m "docs: añadir archivo de instrucciones"

# Etiquetas permitidas en los commits:
# feat: nueva funcionalidad
# docs: documentación
# fix: corrección de errores
# chore: tareas de mantenimiento
#
# --------------------------------------------------
# HACER PUSH
# --------------------------------------------------
# El push sube tus commits a GitHub para compartirlos con el equipo.

git push -u origin feature-NombreAlumnoB

# --------------------------------------------------
# MERGE MEDIANTE PULL REQUEST
# --------------------------------------------------
# El merge sirve para integrar tu trabajo en la rama principal (main).
# Normalmente se hace desde GitHub usando un Pull Request:
# 1. Pull Requests -> New Pull Request
# 2. Base: main / Compare: tu rama
# 3. Revisar cambios y comentar
# 4. Merge pull request
#
# --------------------------------------------------
# SINCRONIZACIÓN FINAL
# --------------------------------------------------
# Después de que el merge esté hecho en GitHub, se actualiza el repositorio local.

git checkout main
git pull

# Esto trae todos los cambios nuevos a tu ordenador.
#
# FIN DE LAS INSTRUCCIONES
