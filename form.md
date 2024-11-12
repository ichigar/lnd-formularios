# ¿Qué es form en HTML?
#### El form en HTML es un contenedor que contiene campos para que las personas ingresen datos (como su nombre, correo, etc.) y luego lo envia al servidor servidor.
![Mi imagen local](img/form.png)

## Atributos del form
### 1. action
Define la URL a la que se enviarán los datos del formulario cuando el usuario lo envíe.
Ejemplo:
```html
<form action="procesar.php" method="post">
```
### 2. method
Especifica el método HTTP que se usará para enviar los datos. Los valores más comunes son:

* **GET**: Envía los datos como parte de la URL.

* **POST**: Envía los datos en el cuerpo de la solicitud.
```html
<form action="procesar.php" method="post">
```
### 3. name
Define un nombre para el formulario, lo que permite referirse a él en scripts o al enviarlo a través de JavaScript.
```html
<form name="miFormulario">
```
### 4. id
Asigna un identificador único al formulario
```html
<form id="formularioContacto">
```
### 5. target
Determina dónde se abrirá la página de destino especificada en el atributo action. Como por ejemplo:

* **_self**: Abre en la misma ventana o pestaña.
* **_blank**: Abre en una nueva ventana o pestaña.
* **_parent**: Abre en la ventana o marco superior.
* **_top**: Abre en la ventana principal.
```html
<form action="gracias.html" target="_blank">
```
### 6. enctype
Especifica cómo se deben codificar los datos del formulario antes de enviarlos al servidor. Se usa principalmente cuando se envían archivos. Como por ejemplo:

* **application/x-www-form-urlencoded**: Valor predeterminado; los datos se codifican como una cadena de texto en la URL.
* **multipart/form-data**: Usado para formularios que contienen archivos.
* **text/plain**: Los datos se envían como texto plano.
```html
<form action="upload.php" method="post" enctype="multipart/form-data">
```
### 7. autocomplete
Define si el navegador debe autocompletar los campos del formulario con datos previamente ingresados por el usuario. Como por ejemplo:

* **on**: Activa el autocompletado.
* **off**: Desactiva el autocompletado.
```html
<form autocomplete="off">
```
### 8. accept-charset
Define el conjunto de caracteres que se usará para codificar los datos del formulario cuando se envíen al servidor.
```html
<form action="procesar.php" accept-charset="UTF-8">
```
### 9. novalidate
Desactiva la validación de los campos del formulario.
```html
<form action="procesar.php" novalidate>
```
### 10. role
Define el rol del formulario en la interfaz de usuario, útil para accesibilidad.
```html
<form role="form">
```

## Ejemplo de uso de varios atributos en un formulario
```html
<form id="miFormulario" action="/procesar_datos" method="post" target="_blank" enctype="multipart/form-data" autocomplete="on" accept-charset="UTF-8" novalidate>
    <label for="nombre">Nombre:</label>
    <input type="text" id="nombre" name="nombre">
    <label for="email">Correo electrónico:</label>
    <input type="email" id="email" name="email">
    <label for="archivo">Subir archivo:</label>
    <input type="file" id="archivo" name="archivo">
    <input type="submit" value="Enviar">
</form>
```
* *El formulario recoge datos (nombre, correo, archivo), los envía a un servidor cuando se presiona "Enviar", y abre la respuesta en una nueva pestaña.*
### Ejemplo Básico: Formulario de Contacto
```html
<form action="/enviar" method="post">
    <label for="name">Nombre:</label>
    <input type="text" id="name" name="name"><br><br>
    <label for="email">Correo:</label>
    <input type="email" id="email" name="email"><br><br>
    <input type="submit" value="Enviar">
</form>
```
* *Pues aqui te pide tu nombre, el correo y te muestra un boton para enviar* 