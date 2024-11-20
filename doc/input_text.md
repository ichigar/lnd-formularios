# ¿Qué es < input type="text" > en HTML?
El elemento < input > con el atributo type="text" es un campo de entrada estándar en HTML que permite a los usuarios ingresar texto. Es ampliamente utilizado en formularios web para recopilar datos como nombres, correos electrónicos u otra información de texto.
# Cuál es el uso de < input type="text" > en HTML?
Se emplea cuando se necesita un campo simple de entrada de texto que acepte caracteres alfanuméricos. Este tipo de entrada es común en:
* Formularios de contacto.
* Campos de búsqueda.
* Registro o inicio de sesión.
* Cualquier situación donde se requiera ingresar datos en formato texto. 

# Atributos que suelen acompañar a type="text" con ejemplos
 * maxlength: Define el número máximo de caracteres que se pueden ingresar.
 * placeholder: Texto guía dentro del campo antes de que el usuario escriba.
 * required: Hace que el campo sea obligatorio antes de enviar el formulario.
 * readonly: Impide que el usuario edite el contenido.
 * disabled: Desactiva el campo para que no se pueda interactuar con él.

```HTML
<form>
    <label for="nombre">Nombre:</label>
    <input type="text" id="nombre" name="nombre" placeholder="Escribe tu nombre" required maxlength="50"> 
</form>
<form>
    <label for="busqueda">Buscar:</label>
    <input type="text" id="busqueda" name="busqueda" placeholder="¿Qué necesitas buscar?">
</form>
<form>
    <label for="comentario">Comentario:</label>
    <input type="text" id="comentario" name="comentario" value="Texto predeterminado" readonly>
    <button type="submit">Enviar</button>
</form>
```
<form>
    <label for="nombre">Nombre:</label>
    <input type="text" id="nombre" name="nombre" placeholder="Escribe tu nombre" required maxlength="50"> 
</form>
<form>
    <label for="busqueda">Buscar:</label>
    <input type="text" id="busqueda" name="busqueda" placeholder="¿Qué necesitas buscar?">
</form>
<form>
    <label for="comentario">Comentario:</label>
    <input type="text" id="comentario" name="comentario" value="Texto predeterminado" readonly>
    <button type="submit">Enviar</button>
</form>