Práctica: Git y GitHub – Aplicación autónoma del flujo de trabajo
Descripcion:Este proyecto es una aplicación desarrollada en Python que hace uso interfaz gráfica
Objetivo:Aplicar de manera autónoma el flujo de preparación, versionamiento y colaboración de un proyecto utilizando Visual Studio Code, Python, Git y GitHub.
Estructura General:Entorno virtual (ignorado por Git),Caché de ejecución de Python (ignorado por Git), Archivo principal de ejecución, Lista de dependencias del proyecto, Archivos y carpetas ignorados por Git, Documentación del proyecto.
Tecnologia Utilizadas:Git (Controlador de Versiones Local): Sistema de control de versiones distribuido que corre en tu máquina. Permite rastrear cambios, guardar estados del código (commits), aislar trabajo en ramas (branches) y gestionar fusiones (merges). GitHub (Plataforma Remota e Interfaz): Servicio en la nube para alojar y respaldar repositorios Git remotos. Proporciona la interfaz web para administrar Pull Requests (PR), gestionar la colaboración y hacer revisiones de código.   Línea de Comandos / CLI (Terminal / Git Bash): Interfaz basada en texto para ejecutar comandos de Git de forma precisa (como git init, git add, git commit, git push, etc.).
El Entorno y Dependencias:Crear el entorno virtual: Abre la terminal en la carpeta de tu proyecto y ejecuta:
python -m venv .venv

Activar el entorno virtual:
Windows: .venv\Scripts\activate
Linux/Mac: source .venv/bin/activate

Instalar dependencias:
Si ya tienes un archivo de dependencias:
pip install -r requirements.txt
Si estás instalando librerías nuevas (ej. Pandas, Flask):
pip install nombre_libreria

Guardar las dependencias actuales:
Para registrar lo que instalaste en el archivo de configuración:
pip freeze > requirements.txt

Excluir el entorno del control de versiones:
Asegúrate de agregar .venv/ dentro de tu archivo .gitignore para no subir la carpeta a Git.

## Próximas mejoras

- Implementación de la lógica de filtrado por criterio en `app/main.py`.
- Creación de interfaz CLI interactiva para consulta de recursos.
- Carga y persistencia dinámica desde el archivo JSON.