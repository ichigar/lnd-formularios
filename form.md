# ¿Qué es form en HTML?
#### El form en HTML es un contenedor que contiene campos para que las personas ingresen datos (como su nombre, correo, etc.) y luego lo envia al servidor servidor.
![Mi imagen local](img/form.png)
## Estructura Básica

    <form action="/donde-enviar" method="post">
    <!-- Campos del formulario van aquí -->
    </form>
* *action es adónde se envia los datos y method de cómo se envían (post o get).*

### Ejemplo Básico: Formulario de Contacto

    <form action="/enviar" method="post">
    <label for="name">Nombre:</label>
    <input type="text" id="name" name="name"><br><br>
    
    <label for="email">Correo:</label>
    <input type="email" id="email" name="email"><br><br>
    
    <input type="submit" value="Enviar">
    </form>
* *Pues aqui te pide tu nombre, el correo y te muestra un boton para enviar* 