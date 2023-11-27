```jsx
console.log("Hello World");
```

*Este es un código simple en JavaScript que muestra un mensaje "Hola Mundo" en la consola cuando se ejecuta. En lugar de utilizar la función "alert" que muestra una ventana de alerta, utilizamos la función "console.log" para imprimir el mensaje en la consola del navegador o del entorno de desarrollo.*

*Este es un código simple en JavaScript que muestra una ventana de alerta con el mensaje "Hello World" cuando se ejecuta. "alert" es una función incorporada en JavaScript que se utiliza para mostrar ventanas de alerta en un navegador web.*

```jsx
let aux = document.querySelector('#theTitle');
alert(aux.id);
```

*Este fragmento de código JavaScript está haciendo lo siguiente:*

1. *Utiliza el método `document.querySelector` para seleccionar el primer elemento HTML en el documento que coincide con el selector especificado. En este caso, el selector es '#theTitle', que selecciona el elemento con el ID 'theTitle'.*
2. *Guarda la referencia a este elemento en la variable `aux`.*
3. *Luego, muestra una ventana de alerta con el ID del elemento seleccionado utilizando `alert(aux.id)`. Si el elemento con ID 'theTitle' existe en el documento, su ID ('theTitle') se mostrará en la ventana de alerta. Si no existe tal elemento, `aux` será `null` y `aux.id` dará un error.*

```jsx
let myDiv = document.querySelector('#myDiv');
myDiv.style.backgroundColor = "yellow";
```

*Este fragmento de código JavaScript está haciendo lo siguiente:*

1. *Utiliza el método `document.querySelector` para seleccionar el primer elemento HTML en el documento que coincide con el selector especificado. En este caso, el selector es '#myDiv', que selecciona el elemento con el ID 'myDiv'.*
2. *Guarda la referencia a este elemento en la variable `myDiv`.*
3. *Luego, cambia el color de fondo del elemento seleccionado a amarillo utilizando `myDiv.style.backgroundColor = "yellow";`. Si el elemento con ID 'myDiv' existe en el documento, su color de fondo se cambiará a amarillo. Si no existe tal elemento, `myDiv` será `null` y `myDiv.style.backgroundColor = "yellow";` dará un error.*

```jsx
let aux = document.querySelector("#wulu");
aux.style.float = "right"
```

*Este fragmento de código JavaScript está haciendo lo siguiente:*

1. *Utiliza el método `document.querySelector` para seleccionar el primer elemento HTML en el documento que coincide con el selector especificado. En este caso, el selector es '#wulu', que selecciona el elemento con el ID 'wulu'.*
2. *Guarda la referencia a este elemento en la variable `aux`.*
3. *Luego, cambia la propiedad CSS `float` del elemento seleccionado a "right" utilizando `aux.style.float = "right";`. Si el elemento con ID 'wulu' existe en el documento, su propiedad `float` se cambiará a "right", lo que significa que se moverá hacia la derecha de su contenedor. Si no existe tal elemento, `aux` será `null` y `aux.style.float = "right";` dará un error.*

```
let p = document.createElement("p");
p.innerHTML = "Hello World";
p.style.background = "yellow"; 
document.body.appendChild(p);
```

*Este fragmento de código JavaScript está haciendo lo siguiente:*

1. *Crea un nuevo elemento de párrafo (`<p>`) utilizando `document.createElement("p")` y lo guarda en la variable `p`.*
2. *Establece el contenido HTML interno del nuevo elemento de párrafo en "Hello World" utilizando `p.innerHTML = "Hello World"`.*
3. *Cambia el color de fondo del nuevo elemento de párrafo a amarillo utilizando `p.style.background = "yellow"`.*
4. *Finalmente, añade el nuevo elemento de párrafo al final del cuerpo del documento HTML utilizando `document.body.appendChild(p)`. Esto hará que el nuevo párrafo aparezca en la página web con el texto "Hello World" y un fondo amarillo.*

```jsx
document.body.innerHTML = '<img src="<https://via.placeholder.com/350x150>"/>';

```

*Este fragmento de código JavaScript está haciendo lo siguiente:*

1. *Utiliza la propiedad `innerHTML` del objeto `document.body` para establecer el contenido HTML del cuerpo del documento.*
2. *El contenido que se está estableciendo es una etiqueta de imagen (`<img>`), que tiene su atributo `src` establecido en "https://via.placeholder.com/350x150". Este URL es un enlace a una imagen de marcador de posición de 350x150 píxeles.*

*Cuando este código se ejecuta, reemplaza todo el contenido del cuerpo del documento HTML con la imagen de marcador de posición.*