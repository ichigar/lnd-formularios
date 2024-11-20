# Óscar Castro Hernández

## Etiqueta: OPTGROUP
* Uso: El elemento `<optgroup>` en HTML5 se utiliza para agrupar un conjunto de elementos `<option>` dentro de una lista desplegable  `<select>`, permitiendo así organizar opciones relacionadas bajo una misma etiqueta.
+ Ejemplo de uso:

```HTML
<select>
  
<optgroup label="Cítricos">
 
  <option value="limon">Limón</option>
    
  <option value="naranja">Naranja</option>
    
  <option value="pomelo">Pomelo</option>
  
</optgroup>`

<optgroup label="No cítricos">
   
  <option value="manzana">Manzana</option>
   
  <option value="pera">Pera</option>
  
  <option value="banana">Banana</option>
 
</optgroup>

</select>
```

+ Atributos: La etiqueta `<optgroup>` en HTML5 tiene los siguientes atributos:

    + Disabled: Este atributo deshabilita todas las opciones dentro del grupo, impidiendo que el usuario seleccione ninguna opción dentro del grupo.

    + Label: Este atributo especifica el título o títulos del grupo. Este es un atributo obligatorio.

+ Ejemplo de Atributos:
```HTML
<form>
    <label for="select-car-make">Seleccione la marca de su automóvil:</label>
    <select id="select-car-make" name="car-make">
        <optgroup label="Europeas">
            <option value="bmw">BMW</option>
            <option value="audi">Audi</option>
            <option value="mercedes">Mercedes-Benz</option>
        </optgroup>
        <optgroup label="Asiáticas" disabled>
            <option value="toyota">Toyota</option>
            <option value="honda">Honda</option>
            <option value="hyundai">Hyundai</option>
        </optgroup>
        <optgroup label="Norteamericanas">
            <option value="ford">Ford</option>
            <option value="gm">General Motors</option>
            <option value="dodge">Dodge</option>
        </optgroup>
    </select>
</form>
```