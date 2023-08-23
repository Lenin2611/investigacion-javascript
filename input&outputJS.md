# Input & Output en JavaScript

## Input: 

JavaScript `JS` puede capturar entradas del usuario a través de elementos de formulario HTML  `<form>` y eventos de interacción. Algunos ejemplos son: 

- ### Campos de Texto

  ```javascript
  <!DOCTYPE html> 
  <html> 
  <head> 
      <title>Campos de Texto</title> 
  </head> 
  <body> 
  	<input type="text" id="nombre">
  <button onclick="obtenerNombre()">Obtener Nombre</button>
  
  <script>
  function obtenerNombre() {
    const nombre = document.getElementById("nombre").value;
    alert("Nombre ingresado: " + nombre);
  }
  </script>
  </body> 
  </html>
  ```

  

- ### Campos  Numéricos

  ```javascript
  <!DOCTYPE html> 
  <html> 
  <head> 
      <title>Campos Numéricos</title> 
  </head> 
  <body> 
  	<input type="number" id="edad">
  <button onclick="verificarEdad()">Verificar Edad</button>
  
  <script>
  function verificarEdad() {
    const edad = document.getElementById("edad").value;
  
    if (edad === "") {
      alert("Por favor, ingresa una edad.");
    } else if (isNaN(edad)) {
      alert("Ingresa un valor numérico válido.");
    } else {
      if (edad >= 18) {
        alert("Eres mayor de edad.");
      } else {
        alert("Eres menor de edad.");
      }
    }
  }
  </script>
  </body> 
  </html>
  ```

  

- ### Selectores

  ```javascript
  <!DOCTYPE html> 
  <html> 
  <head> 
      <title>Selectores</title> 
  </head> 
  <body> 
  	<select id="color">
    <option value="rojo">Rojo</option>
    <option value="verde">Verde</option>
    <option value="azul">Azul</option>
  </select>
  <button onclick="obtenerColor()">Obtener Color</button>
  
  <script>
  function obtenerColor() {
    const selectorColor = document.getElementById("color");
    const colorSeleccionado = selectorColor.value;
    alert("Color seleccionado: " + colorSeleccionado);
  }
  </script>
  </body> 
  </html>
  ```

  

- ### Casillas de verificación

  ```javascript
  <!DOCTYPE html> 
  <html> 
  <head> 
      <title>Casillas de Verificación</title> 
  </head> 
  <body> 
  	<input type="checkbox" id="suscribirse"> Suscribirse al boletín
  <button onclick="verificarSuscripcion()">Verificar Suscripción</button>
  
  <script>
  function verificarSuscripcion() {
    const checkbox = document.getElementById("suscribirse");
    const estaSuscripto = checkbox.checked;
    
    if (estaSuscripto) {
      alert("Estás suscrito al boletín.");
    } else {
      alert("No estás suscrito al boletín.");
    }
  }
  </script>
  </body> 
  </html>
  ```

  

- ### Eventos de Mouse

  ```javascript
  <!DOCTYPE html> 
  <html> 
  <head> 
      <title>Eventos de Mouse</title> 
  </head> 
  <body> 
  	<button id="boton">Haz Clic</button>
  
  <script>
  const boton = document.getElementById("boton");
  
  boton.addEventListener("click", function() {
    alert("¡Haz hecho clic en el botón!");
  });
  </script>
  </body> 
  </html>
  ```

  

- ### Eventos de Teclado

  ```javascript
  <!DOCTYPE html> 
  <html> 
  <head> 
      <title>Eventos de Teclado</title> 
  </head> 
  <body> 
  	<input type="text" id="inputTexto">
  
  <script>
  const inputTexto = document.getElementById("inputTexto");
  
  inputTexto.addEventListener("keypress", function(event) {
    alert("Tecla presionada: " + event.key);
  });
  </script>
  </body> 
  </html>
  ```

- ### Solicitudes HTTP

- ### Interacciones con Bases de Datos

## Output: 

JavaScript `JS` puede mostrar información al usuario a través de ventanas emergentes como alertas `alert`, en la consola de desarrollador con `console.log()`, modificando el `HTML`, `DOM` y `CSS`, y crear ventanas emergentes.