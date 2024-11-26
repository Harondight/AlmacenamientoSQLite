# AlmacenamientoSQLite
 Administrador de tares

 # Proyecto de Gestión de Tareas
## Requisitos

- **Node.js**: Asegúrate de tener **Node.js** instalado. Si no lo tienes, puedes descargarlo desde [aquí](https://nodejs.org/en/).

- **SQLite**: Este proyecto usa SQLite como base de datos. Asegúrate de tener **SQLite** instalado en tu máquina. Puedes descargarlo desde [aquí](https://www.sqlite.org/).

**Importante**: Si tienes problemas con Node.js, o si ves un error al intentar ejecutar el proyecto, puedes ejecutar el siguiente comando para instalar las dependencias necesarias:

```bash
npm install express sqlite3 body-parser cors
```

#### 2. **Clonación y configuración**
La parte de clonación y configuración está bien, pero podrías especificar algunos pasos adicionales si es necesario, especialmente si otras personas van a ejecutar el proyecto. Por ejemplo, si el proyecto tiene configuraciones especiales de entorno o base de datos, es bueno dejarlo claro:

```markdown
## Configuración

1. **Clona el repositorio**:

   ```bash
   git clone <url-del-repositorio>
   ```

   Si no tienes **Git** instalado, puedes descargarlo desde [aquí](https://git-scm.com/).

2. **Instala las dependencias**:

   Una vez que hayas clonado el repositorio, navega a la carpeta `server` y ejecuta el siguiente comando para instalar todas las dependencias necesarias para el backend:

   ```bash
   cd server
   npm install
   ```

   Esto instalará los módulos **express**, **sqlite3**, **body-parser** y **cors**.

3. **Inicia el servidor**:

   Luego, puedes iniciar el servidor de backend con el siguiente comando:

   ```bash
   node server.js
   ```

   Si todo está configurado correctamente, el servidor debería arrancar y te mostrará un mensaje similar a este en la consola:

   ```
   Servidor corriendo en el puerto 3000
   Conexión exitosa a la base de datos SQLite.
   ```

4. **Accede a la aplicación**:

   Ahora puedes abrir tu navegador y dirigirte a:

   ```
   http://localhost:3000
   ```

   Esto abrirá la aplicación en tu navegador. Si ves el mensaje de error "Cannot GET /", es posible que necesites crear una ruta básica en tu `server.js` o asegurarte de que los archivos estáticos estén configurados correctamente (por ejemplo, tu `index.html` y demás archivos estáticos).

## Solución de problemas

Si te aparece algún error relacionado con dependencias faltantes, asegúrate de haber ejecutado correctamente el comando `npm install` en la carpeta `server`. Si aún persisten problemas, verifica que **Node.js** y **SQLite** estén instalados correctamente.


## Solución de problemas comunes

- Si ves el error **"Cannot GET /"**: Esto podría ser porque no se ha configurado una ruta para manejar la petición de la página de inicio (`index.html`). Revisa tu `server.js` para asegurarte de que estés sirviendo los archivos estáticos correctamente o que tengas la ruta `/` definida.

- Si tienes problemas con la base de datos: Asegúrate de que el archivo `tareas.db` esté presente en el directorio correcto, o revisa la conexión con la base de datos en `server.js`.

- Si el servidor no inicia: Asegúrate de que todas las dependencias se hayan instalado correctamente ejecutando `npm install` dentro de la carpeta `server`. Si hay errores adicionales, verifica que la versión de **Node.js** sea compatible con las dependencias.


