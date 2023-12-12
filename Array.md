# Declarar

```jsx
let myArray = []; // Lista vacia
let myArray = ["Apple", "Orange", "Donkey"]; // Con 3 elementos tipo string
let myArray = new Array(1,2,3,4,5); // ¡No uses esto! Lee a continuación para saber por qué
```

# Acceder

```jsx
console.log(myArray[0]); // Esto imprimirá el 1er elemento en la consola.
let aux = myArray[5];
console.log(aux); // Esto imprimirá el 6to elemento en la consola.
console.log(myArray[myArray.length-1]); // Esto imprimirá el último elemento de la lista.
```

# Actualizar

```jsx
myArray[5] = 'Cualquier Valor';
// Esto establecerá el valor 'Cualquier Valor' en el sexto elemento del array.
```

# Añadir

```jsx
let myArray = ['Pedro', 'Juan', 'Maria'];
myArray.push('Chris');
console.log(myArray); // Esto imprimirá ['Pedro', 'Juan', 'Maria', 'Chris'];
```

# Añadir en posición especifica

```jsx
let myArray = ['Pedro', 'Juan', 'Maria'];
let myNewArray = [];
myNewArray.push('Pedro');
myNewArray.push('Chris');
myNewArray.push('Juan');
myNewArray.push('Maria');
console.log(myNewArray); // Esto imprimirá  ['Pedro', 'Chris', 'Juan', 'Maria'];
```

# Eliminar elementos (Ultima posición)

```jsx
let myArray = ['Pedro', 'Chris', 'Juan', 'Maria'];
myArray.pop();
console.log(myArray); // Esto imprimirá ['Pedro', 'Chris', 'Juan'];

// Si deseas eliminar 'Chris', necesitas hacer lo siguiente: 
let myNewArray = [];
    myNewArray.push('Pedro');
    myNewArray.push('Juan');
    myNewArray.push('Maria');
    console.log(myNewArray); // Esto imprimirá ['Pedro', 'Juan', 'Maria']
```

# Eliminar elementos (Primera posición)

```jsx
let myArray = ['Juan', 'Maria'];
myArray.unshift('Pedro');
myArray.unshift('Chris', 'Bob');
console.log(myArray); // Esto imprimirá ['Chris', 'Bob', 'Pedro', 'Juan', 'Maria'];

// Si deseas eliminar 'Chris', necesitas hacer lo siguiente: 
let myArray = ['Chris', 'Bob', 'Pedro', 'Juan', 'Maria'];
    myArray.shift();
    console.log(myArray); // Esto imprimirá ['Bob', 'Pedro', 'Juan', 'Maria'];
```

# Iterar (Bucle)

```jsx
let myArray = [3423,5,4,47889,654,8,867543,23,48,56432,55,23,25,12];
for (i = 0; i < myArray.length; i++) {
console.log(myArray[i]); // Esto imprimirá el valor del elemento en la posición [i]
}
```

# For… In…

```jsx
let myArray = [3423,5,4,47889,654,8,867543,23,48,56432,55,23,25,12];
for (let index in myArray) {
console.log(myArray[index]);
}
// Esto imprime el valor del elemento en la posición [index
```

# Slice (From position to position) Splice (From position - How many positions)

```jsx
let y = [14, 3, 3245, 234, 52, 345, 3, 45, 23, 77];
y.splice(2,4,'a'); // devuelve [3245, 234, 52, 345]
console.log(y); // --> [14, 3, 'a', 3, 45, 23, 77]

let y = [14, 3, 3245, 234, 52, 345, 3, 45, 23, 77];
y.splice(2,0,'a'); // devuelve [] 
console.log(y); // --> [14, 3, 'a', 3245, 234, 52, 345, 3, 45, 23, 77]
```

# Ordenando (Logicamente)

```jsx
let fruits = ["Banana", "Orange", "Apple", "Mango"];
fruits.sort();
console.log(fruits); // --> ['Apple', 'Banana', 'Mango', 'Orange']
```

# Ordenando (Reversa)

```jsx
let frutas = ['Banana', 'Orange', 'Apple', 'Mango'];
frutas.sort();
console.log(frutas); // --> ['Apple', 'Banana', 'Mango', 'Orange']
frutas.reverse();
console.log(frutas); // --> ['Orange', 'Mango', 'Banana', 'Apple']
```

# Ordenando numeros

```jsx
let puntos = [40, 100, 1, 5, 25, 10];
puntos.sort(function(a, b) {return a - b});
console.log(puntos); // --> [1, 5, 10, 25, 40, 100]
```

# Ordenando Objetos

```jsx
let autos = [
{tipo:'Volvo', año:2016},
{tipo:'Saab', año:2001},
{tipo:'BMW', año:2010}];
autos.sort(function(a, b) {return a.año - b.año});
console.log(autos); // --> [ {tipo: 'Saab', año: 2001}, {tipo: 'BMW', año: 2010}, {tipo: 'Volvo', año: 2016} ]
```
