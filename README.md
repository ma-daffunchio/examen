# mock-up

# Paquetes

Este proyecto fue generado utilizando `create-react-app`, es una utilidad de linea de comandos (CLI) para generar nuevos proyectos en React.

* `styled components` Este paquete se utiliza para poder crear componentes primitivos que utilizan CSS dentro de un componente Javascript
* `react-scripts` Es un paquete que oculta la configuracion de Webpack, preconfigura el proyecto con todos los valores por defecto y todas dependencias.

# Como utilizarlo, modificarlo y compilarlo

* [Para correr el proyecto en un servidor local](webpack-dev-server), primero debemos instalar las dependencias.
  Para eso nos vamos a la consola y parados en la raiz del proyecto(matias-at) corremos `npm install`.
  Esperamos la instalación de los módulos de Node y ejecutamos `npm start`.
  Esto abrira el navegador y la aplicación deberá de correr en el localhost:3000. En caso de otro proyecto esté corriendo en el puerto 3000, en la consola figurará si se desea correr la app en otro puerto.

* [Para modificar] la configuración de Webpack(técnicamente pocas veces necesario), podemos correr el comando `npm run eject`. Esto saca la dependecia de `react-scripts` y agrega la carpeta de configuración y los archivos correspondientes.

* [Para compilar el proyecto] debemos correr `npm run build`. Esto nos agrega una carpeta llamada "build", la cuál contiene todos los archivos necesarios (HTML, CSS, Javascript) para subir al servidor de producción.

# Estructura de archivos

```
matias-at/
  README.md
  package.json
  public/
    index.html
    favicon.ico
  src/
  	components/
  		Col.js
  		L.js
  		M.js
  		S.js
  		SBold.js
  		SBoldUpper.js
  		XL.js
  		XS.js
  		XXL.js
    App.css
    App.js
    App.test.js
    index.css
    index.js
```

# Usos de archivos

La carpeta `components` contiene todos los archivos de estilos (.js) de styled-components, estos son importados al `App.js` como también `App.css`. El `index.js` renderea el archivo `App.js` al cual se le asigna un nombre de id, este mismo nombre luego es insertado en `index.html` para que levante `index.js` y siga toda la secuencia.