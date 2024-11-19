## `<Input type= "email">`

El elemento `<input type="email">` en HTML se usa para crear un campo de entrada donde el usuario debe ingresar una dirección de correo electrónico. Este tipo de entrada ofrece características útiles gracias a sus atributos.

### Atributos

1. required
Indica que el campo de correo electrónico es obligatorio. El formulario no se podrá enviar si este campo está vacío.
Ejemplo: `<input type="email" name="email" required>`

2. placeholder
Muestra un texto de ayuda dentro del campo antes de que el usuario escriba algo. Suele usarse para indicar el formato que se espera.
Ejemplo: `<input type="email" name="email" placeholder="correo@ejemplo.com">`

3. value
Define un valor predeterminado para el campo. Este valor aparecerá como contenido del campo cuando se cargue la página.
Ejemplo: `<input type="email" name="email" value="usuario@ejemplo.com">`

4. pattern
Permite definir una expresión regular personalizada que el correo debe cumplir. Aunque `<input type="email">` ya valida el formato básico, puedes usar pattern para especificar formatos más avanzados.
Ejemplo: `<input type="email" name="email" pattern="[a-z0-9._%+-]+@[a-z0-9.-]+\.[a-z]{2,}$"`

5. maxlength
Limita el número máximo de caracteres que el usuario puede escribir en el campo.
Ejemplo: `<input type="email" name="email" maxlength="50">`

### Ejemplos prácticos:

1. Atributo value: Predefinir un valor

`<form>`
  
  `<label for="email">Correo Electrónico:</label>`
 
  `<input type="email" id="email" name="email" value="usuario@ejemplo.com">`
 
  `<button type="submit">Enviar</button>`

`</form>`

2. Atributo pattern: Validación avanzada de formato

`<form>`

  `<label for="email">Correo Electrónico Corporativo:</label>`

  `<input type="email" id="email" name="email" pattern="[a-zA-Z0-9._%+-]+@ejemplo.com$" title="Por favor, usa un correo de dominio @ejemplo.com" required>`

  `<button type="submit">Enviar</button>`
  
`</form>`
