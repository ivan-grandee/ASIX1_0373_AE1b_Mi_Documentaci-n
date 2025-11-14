# ASIX1_0373_AE1b_Mi_Documentaci-n #
## Github y Git ##
![GitHub Logo](https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png)
### ¿Qué es GitHub? ###
GitHub es una plataforma online que aloja repositorios Git.
Además permite colaborar, revisar código, gestionar proyectos y compartir tu trabajo.
### Crear un repositorio en GitHub ###
1. Ve a github.com y accede a tu cuenta.
2. Haz clic en New repository.
3. Rellena:
- Nombre del repositorio
- Descripción (opcional)
- Visibilidad: público o privado
7. Opcional: inicializa con README, .gitignore, y licencia.
8. Haz clic en Create repository.
### Comenzar con Git ###
#### Inicializa Git abriendo un cmd en tu carpeta local
"git init"

#### Configura tu usuario (solo una vez)
"git config --global user.name "Tu Nombre""
"git config --global user.email "tu@email.com""

#### Añade archivos al área de preparación
"git add archivo.txt"

#### Guarda los cambios con un mensaje
"git commit -m "Primer commit""

#### Sube tu proyecto
"git push origin main"

### Comandos esenciales de Git

| Comando | Descripción | 
|-----------|----------------|
| **git init** | Inicializa un repositorio local |
| **git clone + URL** | Clona un repositorio remoto | 
| **git status** | Muestra el estado de los archivos |
| **git add .** | Añade archivos al área de preparación |
| **git commit -m "mensaje"** | Guarda los cambios con un mensaje |
| **git push** | Sube los cambios al repositorio remoto |
| **git log** | Muestra el historial de commits 1 |
| **git branch** | Lista ramas |


## HTML

### ¿Que es HTML?
HTML (HyperText Markup Language) es el lenguaje estándar para estructurar el contenido de una página web.
Se basa en etiquetas (tags) que definen los diferentes elementos de la página: títulos, párrafos, imágenes, enlaces, tablas, formularios, etc.

### Estructura básica de un documento HTML
```
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Título de la página</title>
</head>
<body>
  <!-- Contenido visible -->
</body>
</html>
```

### Etiquetas Fundamentales HTML
```
<!DOCTYPE html>
```
Función: Declara el tipo de documento y versión de HTML.
Ejemplo: <!DOCTYPE html> indica que es HTML5.


```
<html lang="es">
```
Función: Elemento raíz que contiene todo el documento HTML.
Ejemplo: <html lang="es"> define español como idioma.

```
<head>
```
Función: Contiene metadatos, enlaces y scripts no visibles.
Ejemplo:

```
<head>
    <meta charset="utf-8">
    <title>Mi Página</title>
</head>

<body>
```
Función: Contiene todo el contenido visible de la página.
```
Ejemplo: <body><h1>Hola Mundo</h1></body>
```

### ETIQUETAS DE TABLAS
#### Estructura de Tablas
```
<table border="1">
```
Función: Crea una tabla con borde visible.
Ejemplo:
```
 <table border="1"> tabla con bordes de 1px.
 ```

```
<thead>
```
Función: Define la sección de encabezado de la tabla.
Ejemplo:
```
<thead>
    <tr><th>Nombre</th><th>Edad</th></tr>
</thead>
```

```
<tbody>
```
Función: Define el cuerpo principal de la tabla.
Ejemplo:
```
<tbody>
    <tr><td>Juan</td><td>25</td></tr>
</tbody>
```
```
<tr>
```
Función: Define una fila en la tabla.
Ejemplo: 
```
<tr><td>Dato 1</td><td>Dato 2</td></tr>
```
```
<th>
```
Función: Define una celda de encabezado (negrita y centrada).
Ejemplo: 
```
<th>Producto</th>
```

```
<td>
```
Función: Define una celda normal de datos.
Ejemplo: 
```
<td>Manzanas</td>
```

### Atributos Especiales de Tablas
```
colspan="X"
```
Función: Une horizontalmente X celdas.
```
Ejemplo: <th colspan="2">Título Amplio</th>
```

```
rowspan="X"
```
Función: Une verticalmente X celdas.
Ejemplo: 
```
<td rowspan="2">Dato Largo</td>
```

### ETIQUETAS MULTIMEDIA
#### Imágenes
```
<img src="ruta" alt="texto">
```
Función: Inserta una imagen en la página.
Ejemplo:
```
<img src="images/foto.jpg" alt="Descripción" width="200" height="150">
```
#### Audio
```
<audio controls>
```
Función: Reproductor de audio con controles.
Ejemplo:
```
<audio controls>
    <source src="musica/cancion.mp3" type="audio/mpeg">
</audio>
```
#### Contenido Embebido
```
<iframe>
```
Función: Inserta contenido externo en la página.
Ejemplo:
```
<iframe src="https://open.spotify.com/embed/track/..." width="100%" height="152"></iframe>
```

### ETIQUETAS DE FORMULARIO
#### Estructura del Formulario
```
<form action="url" method="post">
```
Función: Define un formulario para entrada de datos.
Ejemplo:
```
<form action="procesar.php" method="post" enctype="multipart/form-data">
```
#### Campos de Entrada
```
<input type="text">
```
Función: Campo de texto de una línea.
Ejemplo:
```
<input type="text" name="nombre" placeholder="Tu nombre" required>
```

```
<input type="email">
```
Función: Campo específico para emails con validación.
Ejemplo: 
```
<input type="email" name="email" required>
```
```
<input type="number">
```
Función: Campo para números con controles.
Ejemplo:
```
<input type="number" name="edad" min="0" max="100">
```
```
<input type="checkbox">
```
Función: Casilla de verificación múltiple.
Ejemplo:
```
<input type="checkbox" name="intereses" value="musica"> Música
```

#### Listas Desplegables
```
<select>
```
Función: Lista desplegable de opciones.
Ejemplo:
```
<select name="pais">
    <option value="es">España</option>
    <option value="mx">México</option>
</select>
```
```
<textarea>
```
Función: Campo de texto multilínea.
Ejemplo:
```
<textarea name="comentario" rows="4" cols="50"></textarea>
```
```
<button type="submit">
```
Función: Botón para enviar el formulario.
Ejemplo: 
```
<button type="submit">Enviar</button>
```

### ETIQUETAS DE CONTENIDO
#### Encabezados
```
<h1> a <h6>
```
Función: Define encabezados de diferentes niveles.
Ejemplo:
```
<h1>Título Principal</h1>
<h2>Subtítulo</h2>
<h3>Apartado</h3>
```
#### Párrafos y Saltos
```
<p>
```
Función: Define un párrafo de texto.
Ejemplo:
```
<p>Este es un párrafo de ejemplo.</p>
```
```
<br>
```
Función: Salto de línea (etiqueta vacía).
Ejemplo: 
```
Texto aquí<br>Nueva línea
```
#### Enlaces
```
<a href="url">
```
Función: Crea un hipervínculo.
Ejemplo:
```
<a href="pagina2.html">Ir a página 2</a>
<a href="#seccion">Ir a sección</a>
```
#### Listas
```
<ol>
```
Función: Lista ordenada (numerada).
Ejemplo:
```
<ol>
    <li>Primer paso</li>
    <li>Segundo paso</li>
</ol>
```
```
<ul>
```
Función: Lista no ordenada (con viñetas).
Ejemplo:
```
<ul>
    <li>Elemento 1</li>
    <li>Elemento 2</li>
</ul>
```
```
<li>
```
Función: Elemento individual de una lista.
Ejemplo: 
```
<li>Manzanas</li>
```

### ETIQUETAS DE FORMATEO
#### Texto
```
<strong>
```
Función: Texto en **negrita** (importancia semántica).
Ejemplo: 
```
<strong>Texto importante</strong>
```
```
<em> o <i>
```
Función: Texto en *cursiva* (énfasis).
Ejemplo: 
```
<i>Texto en cursiva</i>
```
```
<hr>
```
Función: Línea horizontal separadora.
Ejemplo: <hr> crea una línea divisoria.

### ETIQUETAS META Y ENLACES
#### Metadatos
```
<meta charset="utf-8">
```
Función: Define la codificación de caracteres.
Ejemplo: Obligatorio para caracteres especiales.
```
<meta name="viewport" content="width=device-width, initial-scale=1">
```
Función: Configura la visualización en dispositivos móviles.
Ejemplo: Esencial para diseño responsive.

#### Enlaces Externos
```
<link rel="icon" href="ruta">
```
Función: Define el favicon de la página.
Ejemplo: 
```
<link rel="icon" href="favicon.ico">
```

```
<script src="url"></script>
```
Función: Enlaza o ejecuta código JavaScript.
Ejemplo:
```
<script src="https://kit.fontawesome.com/..."></script>
```
### VALIDATOR HTML
#### ¿Qué es el Validator HTML?
Es una herramienta oficial del W3C que verifica si el código HTML cumple con los estándares web.

#### ¿Para qué sirve?
- Detecta errores de sintaxis

- Verifica etiquetas mal cerradas

- Comprueba atributos incorrectos

- Asegura compatibilidad entre navegadores

#### Cómo usarlo:
1. Visitar validator.w3.org

2. Introducir URL, subir archivo o pegar código

3. Revisar los errores y advertencias

4. Corregir problemas identificados


#### Cómo se ve el validador

![imagenvalidador](./newslettercheck.png)
