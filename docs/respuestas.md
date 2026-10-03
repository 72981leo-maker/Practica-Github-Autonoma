1-Espacio y ligereza: requirements.txt es un texto plano de unos pocos kilobytes; .venv pesa cientos de megabytes y llena el proyecto de archivos innecesarios.

2-Compatibilidad universal: .venv incluye archivos compilados que fallan al cambiar de sistema operativo (Windows, Mac, Linux); requirements.txt instala la versión adecuada para cada equipo.

3-Buenas prácticas con Git: Evita conflictos de código y repositorios pesados (la carpeta .venv siempre debe ir en .gitignore).

4-Despliegues automáticos: Permite que servidores en la nube y sistemas CI/CD instalen el proyecto desde cero de forma rápida y limpia.

5. ¿Por que el repositorio que tienes ahora en tu computadora no es el mismo concepto de fork creado en Github?
R=por que el tenemos que en nuestra computadora no es el nosotros y por que las modificaciones qwue le hicimos no se notar tanto al menos que el dueño ponga los comando y ahora si pueda ver los camnios que hicimos 

## Preguntas y Respuestas ##
 79. Identificación del comando: Consultando los mensajes de orientación que muestra git status, la ayuda integrada de Git (git --help) o la documentación oficial.

80. Preparar vs. crear commit: Preparar (git add) selecciona los cambios y los pone en una zona intermedia (Staging Area); crear el commit (git commit) guarda esa foto de los cambios de forma permanente en el historial del repositorio.

81. Comprobar la rama activa: Ejecutando git branch (la rama actual estará marcada con un asterisco * y resaltada) o con el comando git status.

82. Determinar archivos modificados: Con el comando git status, el cual lista en color rojo todos los archivos que fueron modificados antes de prepararse.

83. Observar cambios exactos: Usando el comando git diff (o haciendo clic sobre el archivo en la sección de control de fuente de Visual Studio Code para ver la comparativa).

84. Reconstrucción de .venv: Porque la carpeta .venv es pesada y específica para la computadora y sistema operativo de quien la creó. No debe subirse a GitHub, por lo que cada desarrollador la genera localmente al descargar el proyecto.

85. Relación entre requirements.txt y .gitignore: Como .venv se excluye en .gitignore para no saturar el repositorio con archivos innecesarios, requirements.txt actúa como una lista ligera con las dependencias necesarias para que cualquiera pueda volver a construir la carpeta .venv.

86. Colaborar desde una rama: Para proteger el código estable de la rama principal (main), trabajar en paralelo sin afectar a otros colaboradores y permitir la revisión del código mediante Pull Requests antes de integrarlo.

87. Sin nuevo Pull Request: Porque el PR está vinculado a la rama, no a un commit específico; al subir correcciones con git push a esa misma rama, el Pull Request existente se actualiza automáticamente.

88. Actualizar el repositorio local: Porque el merge se realiza directamente en el servidor de GitHub; tu computadora no recibe esos cambios en su rama main local hasta que los descargues usando git pull.