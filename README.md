# Guia de uso de Markdown y HTML

## 1. Cómo Crear un Repositorio en GitHub

1. Registrarte e Iniciar Sesión en GitHub:

* Crea una cuenta en GitHub si no tienes una.
* Inicia sesión en tu cuenta.

2. Crear un Repositorio:

* Selecciona **"*_New repository_"**.
* Escribe el nombre del repositorio.
* Escoge entre Public o Private.
* Agrega un archivo **README.md**.
* Haz clic en **_Create repository_**.

3. Clonar el Repositorio Localmente:

* Copia la URL del repositorio (haz clic en el botón verde Code).
* Abre la terminal o el CMD y escribe:

```
git clone URL_DEL_REPOSITORIO
```

* Esto descarga el repositorio en tu pc.

## 2. Comandos Básicos de Git en CMD

1. Configurar Git por primera vez:

```
git config --global user.name "TuNombre"
git config --global user.email "TuEmail"
```

2. Iniciar un Repositorio Local:

```
git init
```
3. Listar ramas:

```
git branch
```

4. Crear main: 

```
git branch -M main
```

5. Añadir Archivos al Área de Preparación:

```
git add .  
```

6. Guardar cambios con un Commit:

```
git commit -m "Mensaje descriptivo del cambio"
```

7. Subir Cambios al Repositorio Remoto:

```
git push origin main
```

8. Actualizar tu Repositorio Local desde el Remoto:

```
git pull origin main
```

9. Ver el Estado del Repositorio:

```
git status
```
## 6. Modificación de archivo con Markdown

1. Formatos de texto:

* Podemos definir el formato del texto con "_" o "*" para remarcar un texto en **negrita** o en _cursiva_. Para ello debemos usarlos de la siguiente manera:

```
**Hola** <!--Negrita-->

_Hola_ <!--Cursiva-->
```
2. Listado: 

```
1. Primer punto de la lista <!--Lista numerica-->
    1. Primer elemento de la sublista 1 <!--Lista de subpunto o subnivel>
    2. Segundo elemento dela sublista 1
2. Segundo punto de la lista
    * Primer elemento de la sublista 2 <!--Lista en puntos transparentes-->
    * Segundo elemento de la sublista 2
3. Tercer punto de la lista

* Primer punto de lista desordenada <!--Lista en puntos negros>
- Segundo punto de lista desordenada
+ Tercer punto de lista desordenada
```
3. Mostrar código en un repositorio: 

* Para ello debemos usar "**```**" al inicio y al final, quedando de esta manera: 

```
<DOCTYPE html>
<html lang="en">
<head>
    <tr>Hola mundo</tr>
</head>
<body>

</body>
</html>
```
4. Como poner un link:

```
[NombreLink](LinkURL "Titulo opcional")
```
5. Como poner una imagen:

```
![NombreImagen](LinkImagen "Titulo opcional")
```
* Es preferible que la imagen este alojado en el repositorio local.

6. Uso de tablas:

* Las tablas se estructuran de la siguiente manera: 

```
| **Titulo 1** | **Titulo 2** | **Titulo 3** | <!--Las celdas se definen con "|"-->
|:----------:|-------------------:|:--------------| <!--Forma de definir tanto la longitud "-" como la orientación del texto ":"-->
|SMX2|Curso24-25|2080$| <!--Contenido de la tabla-->
```

## 5. Conceptos y Elementos Principales de HTML

* Es el lenguaje estándar para páginas web y define las estructuras y el contenido mediante etiquetas. Todas las páginas web están construidas en base a etiquetas (**Markup**).

* Estructura básica de un html:

    ```
    <!DOCTYPE html>
    <html>
    <head>
        <title>Mi Página</title>
    </head>
    <body>
        <h1>Bienvenido a mi página</h1>
        <p>Este es un párrafo.</p>
    </body>
    </html>
    ```
* Cada contenido va entre comillas de inicio **<>** y de cierre **</>**.

* Los atributos contienen información adicional acerca del elemento. Se definen justo a continuación del elemento, separado con un espacio y dentro de la etiqueta de inicio.

* __DOCTYPE__ es un elemento que se sitúa al inicio del documento y que define el tipo del documento. Va acompañado de un **html** y el documento finaliza con otro **html**.

* Elementos principales: 
    * Estructura ->
        * Raíz del documento.
        ```
        <html>
        ```
        * Contiene metadatos y enlaces a hojas de estilo o scripts.
        ```
        <head> 
        ```
        * Contenido visible de la página.
        ```
        <body>
        ```

    * Texto ->
        * Títulos (de mayor a menor importancia).
        ```
        <h1> a <h6> 
        ```
        * Párrafos
        ```
        <p>
        ```
        * Texto en negrita.
        ```
        <b>
        ```
        * Texto en cursiva
        ```
        <i>
        ```

    * Atributos de html ->
        * __meta__: añade metainformación a la página.
        * __charset__: denota la codificación de caracteres.
        * __title__: descripción del titulo de la etiqueta del navegador.
        * __keywords__: descripción de la página en los resultados de búsqueda.

    * Enlaces e imagenes ->
        * Enlaces
        ```
        <a href="URL">Texto del enlace</a>
        ```
        * Imágenes
        ```
        <img src="URL" alt="Descripción de la imagen">
        ```

    * Listas ->
        * Lista no ordenada (con puntos)
        ```
        <ul>
        ```
        * Lista ordenada (con números)
        ```
        <ol>
        ```
        * Elemento de lista
        ```
        <li>
        ```
    
    * Formularios ->
        ```
        <form action="ejemplo.php" method="get">
            <label for="nombre">Nombre:</label>
            <input type="text" id="nombre" name="nombre">
            <input type="submit" value="Enviar">
        </form>
        ```
* Los formularios nos sirven para interactuar con el usuario y que este pueda transmitir información. 

* Contenido de los formularios ->
    * campos de texto
    * campos de contraseña
    * botones de opción
    * casilla de verificación
    * campos para introducir archivos
    * listas de selección
    * areas de texto
    * botones

* Elementos de los formularios ->
    * <input> ->entrada de datos
    * <type> -> forma en la que se comporta el campo
    * <name> -> nombre del campo de entrada
    * <email> ->formato email
    * <reset> -> resetea todo el campo para dejarlo vacío
    * <submit> -> envía datos
    * <value> -> valor de la variable
    * <required> -> campo obligatorio
    * <placeholder> -> texto indicativo
    * <disable> ->desactivar campo
    * <readonly> -> campo de solo lectura
    * <textarea> ->espacio de rellenar
        * <cols> ->ancho
        * <row> ->alto
    * <select> -> elegir una opción
        * <options> -> definir opciones

Permite aplicar estilos visuales a los elementos HTML.

### Sintaxis Básica

```css
selector {
  propiedad: valor;
}
```

### Ejemplo

```css
body {
  font-family: Arial;
  background-color: #f4f4f4;
}

input[type="text"] {
  border: 1px solid #ccc;
  padding: 8px;
}
```

### Selectores útiles

- `#id` — selecciona por ID
- `.clase` — selecciona por clase
- `elemento` — selecciona por etiqueta
- `div > p` — hijo directo
- `a:hover` — pseudoclase

### Aplicación del CSS

- **Inline**: `<p style="color:red">Texto</p>`
- **Interno**: dentro de `<style>` en HTML
- **Externo**: enlazado con `<link rel="stylesheet" href="estilos.css">`

---

## Diseño Responsive

Hace que el diseño se adapte a diferentes dispositivos y tamaños de pantalla.

### Recomendaciones

- Usa **unidades relativas**: `%`, `em`, `rem`
- Aplica **media queries** para adaptar estilos
- Usa diseño flexible con **Flexbox** o **Grid**

### Ejemplo con Media Query

```css
/* Estilo base */
body {
  font-size: 16px;
}

/* Móvil */
@media (max-width: 768px) {
  body {
    font-size: 14px;
  }

  .menu {
    display: none;
  }
}
```

### Ejemplo con Flexbox

```css
.contenedor {
  display: flex;
  justify-content: space-between;
  flex-wrap: wrap;
}
```

---

## Sesiones en Aplicaciones Web

Las sesiones permiten guardar información del usuario entre páginas o durante su visita.

### ¿Qué es una sesión?

Una sesión almacena datos temporales para un usuario, como si ha iniciado sesión, su carrito de compras, etc.

### Ejemplo en PHP

```php
<?php
session_start();

// Guardar datos
$_SESSION['usuario'] = 'juan123';

// Leer datos
echo $_SESSION['usuario'];

// Eliminar sesión
session_destroy();
?>
```

### Uso común

- Autenticación de usuarios
- Mostrar contenido personalizado
- Proteger rutas restringidas