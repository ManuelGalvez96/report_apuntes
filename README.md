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

## 6. Conceptos de CSS
1. ¿Que es CSS?
   
* **CSS** sirve para dar instrucciones al naveador para representar elementos de la web.
  
* No es ni un lenguage de programación ni de marcas.

* Las ventajas que trae el uso de CSS són:

  * Crea un código eficiente y és más fácil de trabajar
  * Ofrece mayor capacidad de diseño
  * Se pueden definir diferentes hojas de estilo en un solo documento
  * Es reutilizable
  
1. Integrar CSS
   
* Las hojas de estilo se hubican en la propia etiqueta (_inline_), en la cabecera del HTML (_interno_) o en otro fichero (_externo_).

* **INLINE**
```
<p style="text-align:center; color:red">Paragrafo rojo</p>
```

* **INTERNO**
```
<head>
   <style>
    p {
        text-align:center; 
        color:red;
    }
    </style>
</head>
```

* **EXTERNO**
```
<link rel ="stylesheet" href="estilo.css" type="text/css" />

 p {
    text-align:center; 
    color:red;
}
```

* Ejemplo CSS:

```
<!DOCTYPE html>
    <html>
    <head>
        <title>Mi Página</title>
        <link rel ="stylesheet" href="estilo.css" type="text/css" />
        <style>
            p{
                font-size: italic;
                color:green;
            }
            
        </style>
    </head>
    <body>
        <h1 style="color:red">Bienvenido a mi página</h1>

        <h2>Titulo secundario 1</h2>
        <p>Primer parrafo</p>
        <h2>Titulo secundario 2</h2>
        <p>Segundo parrafo</p>
    </body>
    </html>
```
```
h2 { 
    color:blue
}
```
* De esta forma aplicamos CSS tanto de forma _interna_ como _externa_.

* La prioridad que sigue el estilo CSS es la siguiente:

  1. definicion de estilo CSS en etiqueta
  2. definicion de estilo CSS en **HEAD**
  3. archivo CSS
 
* Cuanto más cerca este la definicion CSS del codigo mayor prioridad tiene.

* Dentro del mismo nivel de prioridad tenemos niveles de **especifilidad** que prioriza elementos más especificos a otros como sería el caso de las **ID**. Tanmién cuenta el **orden del código** o **reglas importantes** (__!important__).
  
* Los **selectores** nos sirven para definir que elemento 

* Tipos de Selectores:

    * selector de id
        *
        ```
        <h1 id="titulo">
        ``` 
    * selector de clase
        * Identifica de forma inequivoca a un elemento aplicandole un valor especifico.
        ```
        <p class= "example">
        ```
    * selecotor de elementos
        * 
        ```
        ```
* 
 

