# En juego · Bitácora de negociación

Portafolio estático del semestre con cuatro relatos de actividades de clase y una síntesis de los aprendizajes. Funciona con HTML y CSS, sin dependencias.

## Vista local

Abre `site/index.html` en un navegador. También puedes ejecutar `python3 -m http.server 8000 --directory site` desde la raíz y abrir http://localhost:8000.

## Publicación en GitHub Pages

1. Crea un repositorio público vacío, por ejemplo `bitacora-negociacion`, y descomprime el proyecto. Incluye la carpeta oculta `.github` al subir los archivos.
2. Desde el directorio que contiene este README ejecuta estos comandos, sustituyendo `TU_USUARIO` por tu cuenta de GitHub.

   ```bash
   git init -b main
   git add .
   git commit -m "Crear bitácora interactiva de negociación"
   git remote add origin git@github.com:TU_USUARIO/bitacora-negociacion.git
   git push -u origin main
   ```

3. En el repositorio, entra en **Settings → Pages → Build and deployment → Source** y selecciona **GitHub Actions**.
4. Abre **Actions → Publicar bitácora → Run workflow** y elige `main`. La URL aparece en el entorno `github-pages` al terminar. Los siguientes cambios enviados a `main` se publican automáticamente.

Si usas el sitio en un repositorio existente, comprueba el nombre de su rama principal y adapta el disparador del workflow cuando corresponda.

## Editar la bitácora

- `site/index.html` contiene la narración de cada actividad, las reflexiones y los materiales de referencia.
- `site/assets/styles.css` define el aspecto, las ilustraciones y las animaciones.
- `.github/workflows/pages.yml` publica únicamente el contenido de `site/`.

El sitio cita los materiales de clase y no requiere subir los documentos originales.
