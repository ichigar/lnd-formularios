Samuel Cabrera

```html
<body>
    <h2>Formulario de Inicio de Sesión</h2>
    <form action="/login" method="post">
        <label for="password">Contraseña:</label>
        <input type="password" id="password" name="password" required>
        <br><br>
        <button type="submit">Iniciar Sesión</button>
    </form>
</body>

```

## ¿Como funciona la etiqueta 'input typr=password"'
La etiqueta '<input type="password">' es un elemento fundamental en HTML, especialmente en contextos donde se necesita proteger la información confidencial del usuario, como en formularios de inicio de sesión y creación de cuentas. Su principal característica es que oculta el texto mientras el usuario escribe, reemplazándolo por puntos o asteriscos. Esto es particularmente útil en situaciones públicas, donde otras personas podrían ver la pantalla, garantizando así un nivel básico de privacidad visual.

Además de la ocultación del texto en pantalla, el campo de tipo password permite aplicar validaciones de seguridad, como requisitos de longitud mínima '(minlength)' o carácter obligatorio '(required)'. Estos controles ayudan a asegurar que el usuario introduzca contraseñas más seguras, lo cual es fundamental para reducir riesgos de accesos no autorizados. Asimismo, esta entrada funciona de forma óptima con conexiones HTTPS, que cifran los datos transmitidos, protegiendo la información del usuario mientras se envía al servidor.

En combinación con medidas de seguridad en el backend y el uso de HTTPS, el '<input type="password">' ayuda a garantizar un flujo seguro de información desde el usuario hasta el sistema. Esto convierte a esta etiqueta en un recurso esencial en cualquier entorno que requiera una experiencia segura y de confianza, tanto para usuarios como para aplicaciones. En definitiva, este campo mejora la experiencia del usuario al proporcionar privacidad básica y soportar mecanismos de seguridad avanzada para el manejo de contraseñas.

## Atributos
'type="password"': Especifica que el campo ocultará el texto ingresado, mostrando puntos o asteriscos.
'id': Asigna un identificador único al campo, usado comúnmente para vincularlo con una etiqueta <label> o para manipularlo con JavaScript.
```html
<input type="password" id="clave">
```

```html
<input type="password" name="password">
```

required: Indica que el campo es obligatorio y el formulario no puede enviarse si está vacío
```html
<input type="password" required>
```

minlength: Especifica el número mínimo de caracteres que el usuario debe ingresar
```html
<input type="password" minlength="8">
```
maxlength: Limita el número máximo de caracteres que se pueden escribir.

```html
<input type="password" maxlength="16">
```
pattern: Permite definir una expresión regular para validar el formato del texto ingresado.
```html
<input type="password" pattern="[A-Za-z0-9]{8,}" title="Debe contener al menos 8 caracteres, combinando letras y números">
```
placeholder: Muestra un texto de ejemplo o sugerencia dentro del campo.
```html
<input type="password" placeholder="Escribe tu contraseña">
```
autocomplete: Controla si el navegador debe autocompletar el campo con valores previamente guardados. Opciones:
on: Habilita el autocompletado.
off: Desactiva el autocompletado (útil para seguridad).
```html
<input type="password" autocomplete="off">
```
readonly: Hace que el campo sea solo de lectura, evitando modificaciones.
```html
<input type="password" readonly>
```
disabled: Desactiva el campo, impidiendo que se pueda interactuar con él.
```html
<input type="password" disabled>
```
autofocus: Coloca automáticamente el cursor en este campo al cargar la página
```html
<input type="password" autofocus>
```
inputmode: Define el tipo de teclado virtual que se mostrará en dispositivos táctiles. Aunque no siempre es necesario para contraseñas, puede configurarse como text o numeric en casos especiales.
```html
<input type="password" inputmode="text">
```
size: Especifica el ancho visible del campo en caracteres (no afecta el límite de caracteres).
```html
<input type="password" size="20">
```
data-*: Atributos personalizados para almacenar información adicional (usados junto con JavaScript).
```html
<input type="password" data-role="secure-field">
```
## Ejemplo completo
```html
<form action="/submit-password" method="post">
    <label for="password">Contraseña:</label>
    <input type="password" id="password" name="password" required 
           minlength="8" maxlength="16" placeholder="Escribe tu contraseña"
           pattern="[A-Za-z0-9]{8,}" autocomplete="off">
    <button type="submit">Enviar</button>
</form>

```