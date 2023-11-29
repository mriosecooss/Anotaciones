```jsx
console.log("Hello World");
```

*Este es un código simple en JavaScript que muestra un mensaje "Hola Mundo" en la consola cuando se ejecuta. En lugar de utilizar la función "alert" que muestra una ventana de alerta, utilizamos la función "console.log" para imprimir el mensaje en la consola del navegador o del entorno de desarrollo.*

*Este es un código simple en JavaScript que muestra una ventana de alerta con el mensaje "Hello World" cuando se ejecuta. "alert" es una función incorporada en JavaScript que se utiliza para mostrar ventanas de alerta en un navegador web*

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

```jsx
let beginning = "<ul>";
let listString = "<li>First Item</li><li>Second Item</li><li>Third Item</li>";
let ending = "</ul>";
```

*Este fragmento de código JavaScript está creando una lista HTML no ordenada como una cadena de texto.*

1. *La variable `beginning` se inicializa con el valor `"<ul>"`, que es la etiqueta de apertura para una lista no ordenada en HTML.*
2. *La variable `listString` se inicializa con el valor `"<li>First Item</li><li>Second Item</li><li>Third Item</li>"`. Esto es una cadena de texto que contiene tres elementos de lista (`<li>`), cada uno con un texto diferente ("First Item", "Second Item", "Third Item").*
3. *La variable `ending` se inicializa con el valor `"</ul>"`, que es la etiqueta de cierre para una lista no ordenada en HTML.*

*Cuando se concatenan estas tres variables (`beginning + listString + ending`), se obtiene una cadena de texto que representa una lista no ordenada completa en HTML con tres elementos.*

```jsx
let li = document.querySelector("#secondElement")
li.parentNode.removeChild(li)
```

*Este fragmento de código JavaScript está eliminando un elemento específico de una lista HTML en el documento.*

1. *La primera línea `let li = document.querySelector("#secondElement")` está seleccionando el primer elemento HTML en el documento que coincide con el selector "#secondElement". Este selector apunta al elemento con el ID "secondElement". La referencia a este elemento se guarda en la variable `li`.*
2. *La segunda línea `li.parentNode.removeChild(li)` está eliminando el elemento seleccionado del documento. `li.parentNode` obtiene el nodo padre del elemento seleccionado, que sería el elemento de lista (`<ul>` o `<ol>`) que contiene el elemento de lista (`<li>`) seleccionado. Luego, `removeChild(li)` elimina el elemento seleccionado de este nodo padre.*

*Por lo tanto, si en tu documento HTML tienes un elemento con el ID "secondElement", este fragmento de código lo eliminará del documento.*

```jsx
let list = document.querySelector('#parentLi');
let secondLi = list.childNodes[3];
list.removeChild(secondLi);
```

*Este fragmento de código JavaScript está eliminando un elemento específico de una lista HTML en el documento.*

1. *La primera línea `let list = document.querySelector('#parentLi');` está seleccionando el primer elemento HTML en el documento que coincide con el selector '#parentLi'. Este selector apunta al elemento con el ID 'parentLi'. La referencia a este elemento se guarda en la variable `list`.*
2. *La segunda línea `let secondLi = list.childNodes[3];` está seleccionando el cuarto hijo del elemento seleccionado anteriormente. En JavaScript, la propiedad `childNodes` devuelve una colección de nodos hijos, y los índices de esta colección comienzan en 0. Por lo tanto, `childNodes[3]` selecciona el cuarto nodo hijo. Esta referencia se guarda en la variable `secondLi`.*
3. *La tercera línea `list.removeChild(secondLi);` está eliminando el nodo hijo seleccionado del elemento de lista. `removeChild(secondLi)` elimina el nodo hijo `secondLi` del nodo padre `list`.*

*Por lo tanto, si en tu documento HTML tienes un elemento con el ID 'parentLi' y este elemento tiene al menos cuatro hijos, este fragmento de código eliminará el cuarto hijo de ese elemento.*

```jsx
let button = document.getElementById("superDuperButton");
button.addEventListener("click", function() {
	
	let newDiv = document.createElement("div");
	newDiv.style.backgroundColor = "yellow";
	newDiv.innerHTML = "Hello World";
	document.body.appendChild(newDiv);
});
```

*Este fragmento de código JavaScript está creando un nuevo elemento `<div>` con un fondo amarillo y el texto "Hello World" cada vez que se hace clic en un botón específico.*

1. *La primera línea `let button = document.getElementById("superDuperButton");` está seleccionando el elemento HTML en el documento con el ID "superDuperButton", que se espera que sea un botón. La referencia a este botón se guarda en la variable `button`.*
2. *Luego, `button.addEventListener("click", function() {...});` está añadiendo un escuchador de eventos al botón. Este escuchador de eventos se activará cada vez que se haga clic en el botón.*
3. *Dentro de la función del escuchador de eventos, se crea un nuevo elemento `<div>` utilizando `document.createElement("div")` y se guarda en la variable `newDiv`.*
4. *Luego, se establece el color de fondo del nuevo `<div>` en amarillo con `newDiv.style.backgroundColor = "yellow";` y se establece su contenido HTML en "Hello World" con `newDiv.innerHTML = "Hello World";`.*
5. *Finalmente, `document.body.appendChild(newDiv);` añade el nuevo `<div>` al final del cuerpo del documento HTML. Como resultado, cada vez que se hace clic en el botón, aparecerá un nuevo `<div>` con un fondo amarillo y el texto "Hello World" en la página web.*

```jsx
let button = document.getElementById("superDuperButton");
button.addEventListener("click", function () {

	let newLi = document.createElement("li");
	newLi.innerHTML = "New item";
	let myList = document.getElementById("myList");
	myList.appendChild(newLi);
});
```

*Este fragmento de código JavaScript está creando un nuevo elemento de lista (`<li>`) con el texto "New item" y lo añade a una lista existente cada vez que se hace clic en un botón específico.*

1. *La primera línea `let button = document.getElementById("superDuperButton");` está seleccionando el elemento HTML en el documento con el ID "superDuperButton", que se espera que sea un botón. La referencia a este botón se guarda en la variable `button`.*
2. *Luego, `button.addEventListener("click", function() {...});` está añadiendo un escuchador de eventos al botón. Este escuchador de eventos se activará cada vez que se haga clic en el botón.*
3. *Dentro de la función del escuchador de eventos, se crea un nuevo elemento de lista (`<li>`) utilizando `document.createElement("li")` y se guarda en la variable `newLi`.*
4. *Luego, se establece el contenido HTML del nuevo elemento de lista en "New item" con `newLi.innerHTML = "New item";`.*
5. *Después, se selecciona el elemento con el ID "myList" utilizando `document.getElementById("myList")` y se guarda en la variable `myList`. Se espera que este elemento sea una lista (`<ul>` o `<ol>`).*
6. *Finalmente, `myList.appendChild(newLi);` añade el nuevo elemento de lista al final de la lista existente. Como resultado, cada vez que se hace clic en el botón, se añadirá un nuevo elemento de lista con el texto "New item" a la lista en la página web.*

```
let myString = "<p>Hello!</p> <strong>My friend</strong>, we are in the year " + new Date().getFullYear();
document.write(myString);
```

*Este fragmento de código JavaScript está creando una cadena de texto que incluye etiquetas HTML y el año actual, y luego escribe esa cadena en el documento HTML.*

1. *La primera línea `let myString = "<p>Hello!</p> <strong>My friend</strong>, we are in the year " + new Date().getFullYear();` está creando una cadena de texto que comienza con algunas etiquetas HTML (`<p>` y `<strong>`) y texto. Luego, concatena el año actual obtenido de `new Date().getFullYear()`. `new Date()` crea un nuevo objeto de fecha con la fecha y hora actuales, y `getFullYear()` obtiene el año de esa fecha.*
2. *La segunda línea `document.write(myString);` escribe la cadena de texto en el documento HTML. `document.write()` es una función JavaScript que escribe una cadena de texto en un documento HTML. En este caso, la cadena de texto incluye etiquetas HTML, por lo que cuando se escribe en el documento, el navegador interpretará estas etiquetas y las renderizará como HTML.*

*Por lo tanto, cuando se ejecuta este código, verás un párrafo que dice "Hello!" seguido de "My friend" en negrita, y luego "we are in the year " seguido del año actual, todo en la misma línea en tu página web.*

```jsx
let countries = ["USA", "France", "Italy", "Brazil", "Colombia", "Belize", "Venezuela"];

let selectElement = document.getElementById("mySelect");

for (let i = 0; i < countries.length; i++) {
  let option = document.createElement("option");
  option.value = countries[i];
  option.innerHTML = countries[i];
  selectElement.appendChild(option);
}

selectElement.addEventListener("change", function () {
  let selectedCountry = selectElement.value;
  alert(selectedCountry);
});
```

*Este fragmento de código JavaScript está creando dinámicamente una lista desplegable (o select) de países en un documento HTML y muestra una alerta con el país seleccionado cuando el usuario cambia la selección.*

1. *La primera línea `let countries = ["USA", "France", "Italy", "Brazil", "Colombia", "Belize", "Venezuela"];` está declarando un array de cadenas de texto, cada una representando un país.*
2. *Luego, `let selectElement = document.getElementById("mySelect");` selecciona el elemento HTML con el ID "mySelect", que se espera que sea un elemento `<select>`. La referencia a este elemento se guarda en la variable `selectElement`.*
3. *El bucle `for` que sigue crea un nuevo elemento `<option>` para cada país en el array `countries`. Para cada opción, se establece el valor y el contenido HTML en el país correspondiente, y luego se añade al elemento `<select>`.*
4. *Finalmente, `selectElement.addEventListener("change", function () {...});` añade un escuchador de eventos al elemento `<select>`. Este escuchador de eventos se activará cada vez que el usuario cambie la selección en la lista desplegable. Cuando esto sucede, se muestra una alerta con el país seleccionado.*

*Por lo tanto, cuando se ejecuta este código, se creará una lista desplegable de países en la página web. Cuando el usuario seleccione un país de la lista, se mostrará una alerta con el nombre del país seleccionado.*

```jsx
const inputField = document.getElementById("addToDo");
const todoList = document.querySelector("ul");

function addTask() {
    const taskText = inputField.value.trim(); 

    if (taskText !== "") {

        const listItem = document.createElement("li");
        listItem.innerHTML = `<span><i class="fa fa-trash"></i></span> ${taskText}`;
        todoList.appendChild(listItem);
        inputField.value = "";
    }
}

function deleteTask(event) {
    const clickedElement = event.target;
    if (clickedElement.classList.contains("fa-trash")) {
        const listItem = clickedElement.parentElement.parentElement;
        todoList.removeChild(listItem);
    }
}

inputField.addEventListener("keypress", function (e) {
    if (e.key === "Enter") {
        addTask();
    }
});

todoList.addEventListener("click", deleteTask);
```

*Este fragmento de código JavaScript está implementando una funcionalidad básica de una lista de tareas o "to-do list". Permite a los usuarios agregar nuevas tareas y eliminar tareas existentes.*

1. *Las primeras dos líneas seleccionan dos elementos del documento HTML: un campo de entrada de texto (`inputField`) donde los usuarios pueden escribir nuevas tareas, y una lista (`todoList`) donde se mostrarán las tareas.*
2. *La función `addTask()` se utiliza para agregar una nueva tarea a la lista. Primero, obtiene el texto de la tarea del campo de entrada y elimina cualquier espacio en blanco al principio y al final del texto con `trim()`. Si el texto de la tarea no está vacío, crea un nuevo elemento de lista (`<li>`) con el texto de la tarea y un icono de basura (que se utilizará para eliminar la tarea), y luego añade este elemento a la lista. Finalmente, borra el texto del campo de entrada.*
3. *La función `deleteTask(event)` se utiliza para eliminar una tarea existente de la lista. Se activa cuando se hace clic en la lista de tareas. Si el elemento en el que se hizo clic es el icono de basura, encuentra el elemento de lista correspondiente y lo elimina de la lista.*
4. *Finalmente, se añaden dos escuchadores de eventos: uno al campo de entrada que activa `addTask()` cuando se presiona la tecla Enter, y otro a la lista de tareas que activa `deleteTask()` cuando se hace clic en ella.*

*Por lo tanto, cuando se ejecuta este código, los usuarios pueden agregar nuevas tareas a la lista escribiendo en el campo de entrada y presionando Enter, y pueden eliminar tareas existentes haciendo clic en el icono de basura junto a cada tarea.*
