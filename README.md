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
