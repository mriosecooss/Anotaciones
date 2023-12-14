<h1>#01 Hello World</h1>

```js
import React from "react";
import ReactDOM from "react-dom";

// If we have a variable
let age = "12";
let name = "John";

// We can use it in our html like this
let output = (
    <span>
        James is <strong>12</strong> years old
    </span>
);

// Use react-dom to render it
ReactDOM.render(output, document.querySelector("#myDiv"));
```

Este código es un ejemplo básico de cómo se puede usar React y ReactDOM para renderizar contenido HTML en una página web.

Primero, se importan los módulos necesarios, que son `React` y `ReactDOM`. `React` es una biblioteca de JavaScript para construir interfaces de usuario y `ReactDOM` es una biblioteca que proporciona métodos específicos del DOM para React.

Luego, se definen dos variables, `age` y `name`.

Después, se crea una variable `output` que contiene un elemento JSX. En este caso, `output` es un elemento `span` que contiene un texto y un elemento `strong`.

Finalmente, se utiliza `ReactDOM.render()` para renderizar el elemento JSX `output` en el DOM. El primer argumento de `ReactDOM.render()` es el elemento que quieres renderizar y el segundo argumento es la ubicación en el DOM donde quieres renderizar ese elemento. En este caso, se está buscando un elemento con el ID `myDiv` y se está colocando el contenido de `output` dentro de ese elemento.

```js
import React from "react"; // Main React.js library
import ReactDOM from "react-dom"; // We use ReactDOM to render into the DOM

// Only update the value of this array

const navlinkItems = [];
const content = <ul className="nav">{navlinkItems}</ul>;

ReactDOM.render(content, document.querySelector("#myDiv"));
```

Se define una constante `navlinkItems` que es un array vacío.

Después, se crea una constante `content` que contiene un elemento JSX. En este caso, `content` es un elemento `ul` que tiene la clase "nav" y contiene el array `navlinkItems`. Sin embargo, dado que `navlinkItems` es un array vacío, no se renderizará nada dentro del elemento `ul`.

---
<h1>#02 Hello World JSX</h1>

```js
// If we have a variable
let age = "12";
let name = "John";

// We can use it in our html like this
let output = (
    <span>{name} is {age} years old
    </span>
);
```

Se definen dos variables, `age` y `name`, que contienen una cadena de texto cada una. `age` es "12" y `name` es "John".

Las llaves `{}` en JSX se utilizan para insertar expresiones de JavaScript en el código. Dentro de las llaves, puedes poner cualquier expresión de JavaScript válida. En este caso, se están utilizando para insertar las variables `name` y `age` en el texto.

---
<h1>#03 Rendering from objects</h1>

```js
const customer = {
    first_name: "Bob",
    last_name: "Dylan",
};

//Your code inside these <div> tags

const output = (
    <div>
        <h1>My name is {customer.first_name}</h1>
        <h2>My last name is {customer.last_name}</h2>
    </div>
);
```

Se define una constante `customer` que es un objeto con dos propiedades: `first_name` y `last_name`. `first_name` es "Bob" y `last_name` es "Dylan".

Las llaves `{}` en JSX se utilizan para insertar expresiones de JavaScript en el código. Dentro de las llaves, puedes poner cualquier expresión de JavaScript válida. En este caso, se están utilizando para insertar las propiedades `first_name` y `last_name` del objeto `customer` en el texto.

---
<h1>#04 Building a layout</h1>

```js
const data = {
    image: "../../.learn/assets/Dylan.png?raw=true",
    cardTitle: "Bob Dylan",
    cardDescription:
        "Bob Dylan (born Robert Allen Zimmerman, May 24, 1941) is an American singer-songwriter, author, and artist who has been an influential figure in popular music and culture for more than five decades.",
    button: {
        url: "https://en.wikipedia.org/wiki/Bob_Dylan",
        label: "Go to wikipedia",
    },
};

// Modify the 'content' variable below to display the desired bootstrap card
let content = (
    <div className="card m-5">
        <img alt="Card image cap" src={data.image} className="card-img-top" />
        <div className="card-body">
            <h5 className="card-title">{data.cardTitle}</h5>
            <p className="card-text">{data.cardDescription}</p>
            <a href={data.button.url} className="btn btn-primary">
                {data.button.label}
            </a>
        </div>
    </div>
);
```

Este fragmento de código es un ejemplo de cómo se pueden usar objetos y JSX para crear una tarjeta de Bootstrap en React.

Primero, se define una constante `data` que es un objeto con varias propiedades. Las propiedades `image`, `cardTitle` y `cardDescription` son cadenas de texto que representan la imagen de la tarjeta, el título de la tarjeta y la descripción de la tarjeta, respectivamente. La propiedad `button` es otro objeto que contiene una URL y una etiqueta para un botón.

Luego, se crea una variable `content` que contiene un elemento JSX. Este elemento JSX es una tarjeta de Bootstrap que utiliza las propiedades del objeto `data` para llenar su contenido.

El elemento `img` utiliza la propiedad `image` de `data` para su atributo `src`, que es la ruta de la imagen que se mostrará en la tarjeta. El elemento `h5` utiliza la propiedad `cardTitle` de `data` para su contenido, que es el título que se mostrará en la tarjeta. El elemento `p` utiliza la propiedad `cardDescription` de `data` para su contenido, que es la descripción que se mostrará en la tarjeta. Finalmente, el elemento `a` utiliza la propiedad `url` del objeto `button` en `data` para su atributo `href`, que es el enlace al que llevará el botón, y la propiedad `label` del objeto `button` en `data` para su contenido, que es la etiqueta que se mostrará en el botón.

Por lo tanto, el resultado de `content` será una tarjeta de Bootstrap que muestra una imagen, un título, una descripción y un botón con un enlace a la página de Wikipedia de Bob Dylan. Este elemento se puede renderizar en el DOM utilizando `ReactDOM.render()`.

---
<h1>#05 Building from arrays</h1>

```js
```