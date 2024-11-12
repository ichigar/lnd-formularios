## `<input type="number">`

El elemento HTML `<input type="number">` es un tipo de entrada de datos utilizado en formularios para permitir a los usuarios ingresar valores numéricos. Este tipo de campo tiene varias ventajas, como la validación automática y la presentación de controles de incremento y decremento (flechas hacia arriba y hacia abajo) en la interfaz del usuario. A continuación, se detallan los atributos que puede incluir un campo `<input type="number">`, junto con ejemplos que muestran cómo se utilizan:

### Atributos

#### `min` 

Define el valor mínimo permitido. Este atributo asegura que el valor ingresado no sea menor que el especificado.

Ejemplo: `<input type="number" min="1">`

#### `max`

Define el valor máximo permitido. Este atributo evita que el usuario ingrese un valor mayor al especificado.

Ejemplo: `<input type="number" max="100">`

#### `step`

Especifica los intervalos de valores que se pueden seleccionar. Útil cuando se quieren valores en un rango específico.

Ejemplo: `<input type="number" step="5">`

El usuario solo podrá ingresar valores como 0, 5, 10, 15, etc.

#### `value`

Establece un valor por defecto para el campo numérico al cargar la página.

Ejemplo: `<input type="number" value="10">`

El campo mostrará el valor 10 por defecto.

#### `required`

Indica que el campo es obligatorio y no puede estar vacío cuando se envía el formulario.

Ejemplo: `<input type="number" required>`

#### `placeholder`

Proporciona una pista al usuario sobre qué tipo de datos deben ingresarse. Es un texto que aparece en el campo hasta que el usuario ingresa un valor.

Ejemplo: `<input type="number" placeholder="Ingrese su edad">`

Muestra el texto "Ingrese su edad" hasta que el usuario escriba algo.

#### `name`

Define el nombre del campo. Permite identificar el dato en el lado del servidor al procesar el formulario.

Ejemplo: `<input type="number" name="edad">`

#### `id` y `class`

Estos atributos permiten estilizar y referenciar el campo usando CSS o JavaScript.

Ejemplo: `<input type="number" id="cantidad" class="input-numero">`

### Ejemplos prácticos

#### Campo de edad con restricciones

```html
<label for="edad">Edad:</label>
<input type="number" id="edad" name="edad" min="1" max="120" placeholder="Ingrese su edad" required>
```
#### Campo de selección de cantidad en pasos de 5

```html
<label for="cantidad">Cantidad:</label>
<input type="number" id="cantidad" name="cantidad" min="0" max="50" step="5" value="10">
```

Este campo permite al usuario seleccionar una cantidad de 0 a 50, con incrementos de 5, comenzando en 10 por defecto.

