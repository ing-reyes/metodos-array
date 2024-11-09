# Métodos de Arrays

1. __push()__ Añade uno o más elementos al final de un array y devuelve la nueva longitud del array.

Sintaxis: 
```
array.push(elemento1, elemento2, ..., elementoN)
```

Ejemplo:
```
let arr = [1, 2, 3];
arr.push(4);
console.log(arr); // [1, 2, 3, 4]
```

2. __pop()__ Elimina el último elemento de un array y lo devuelve.

Sintaxis: 
```
array.pop()
```
Ejemplo:
```
let arr = [1, 2, 3];
let removed = arr.pop();
console.log(removed); // 3
console.log(arr); // [1, 2]
```

3. __shift()__ Elimina el primer elemento de un array y lo devuelve.

Sintaxis: 
```
array.shift()
```
Ejemplo:

```

let arr = [1, 2, 3];
let removed = arr.shift();
console.log(removed); // 1
console.log(arr); // [2, 3]
```

4. __unshift()__ Añade uno o más elementos al principio de un array y devuelve la nueva longitud del array.

Sintaxis: 
```
array.unshift(elemento1, elemento2, ..., elementoN)
```

Ejemplo:

```
let arr = [2, 3];
arr.unshift(1);
console.log(arr); // [1, 2, 3]
```

5. __concat()__ Combina dos o más arrays en uno solo.

Sintaxis: 
```
array.concat(array2, array3, ..., arrayN)
```

Ejemplo:

```
let arr1 = [1, 2];
let arr2 = [3, 4];
let result = arr1.concat(arr2);
console.log(result); // [1, 2, 3, 4]
```

6. __join()__ Une todos los elementos de un array en una cadena de texto, separados por el delimitador especificado.

Sintaxis: 
```
array.join(separador)
```

Ejemplo:
```
let arr = ['apple', 'banana', 'cherry'];
let result = arr.join(', ');
console.log(result); // "apple, banana, cherry"
```

7. __slice()__ Extrae una porción superficial de un array sin modificar el array original. Devuelve un nuevo array.

Sintaxis: 

```
array.slice(inicio, fin)
```

Ejemplo:


```
let arr = [1, 2, 3, 4, 5];
let newArr = arr.slice(1, 3);
console.log(newArr); // [2, 3]
```

8. __splice()__ Cambia el contenido de un array eliminando, reemplazando o añadiendo elementos.

Sintaxis: 

```
array.splice(inicio, cantidadEliminada, elemento1, elemento2, ..., elementoN)
```

Ejemplo:


```
let arr = [1, 2, 3, 4, 5];
arr.splice(2, 2, 'a', 'b');
console.log(arr); // [1, 2, 'a', 'b', 5]
```

9. __forEach()__ Ejecuta una función en cada elemento del array.

Sintaxis: 

```
array.forEach(function(element, index, array))
```

Ejemplo:


```
let arr = [1, 2, 3];
arr.forEach(item => console.log(item));
// Salida:
// 1
// 2
// 3
```

10. __map()__ Crea un nuevo array con los resultados de aplicar una función a cada elemento del array original.

Sintaxis: 

```
array.map(function(element, index, array))
```

Ejemplo:

```
let arr = [1, 2, 3];
let result = arr.map(x => x * 2);
console.log(result); // [2, 4, 6]
```

11. __filter()__ Crea un nuevo array con todos los elementos que pasen una condición especificada en una función.

Sintaxis: 

```
array.filter(function(element, index, array))
```

Ejemplo:

```

let arr = [1, 2, 3, 4, 5];
let result = arr.filter(x => x % 2 === 0);
console.log(result); // [2, 4]
```

12. __reduce()__ Aplica una función a un acumulador y a cada elemento del array (de izquierda a derecha) para reducirlo a un solo valor.

Sintaxis: 

```
array.reduce(function(acumulador, element, index, array))
```

Ejemplo:


```
let arr = [1, 2, 3];
let result = arr.reduce((acc, curr) => acc + curr, 0);
console.log(result); // 6
```

13. __find()__ Devuelve el primer elemento que cumpla con la condición especificada en la función proporcionada.

Sintaxis: 

```
array.find(function(element, index, array))
```

Ejemplo:

```
let arr = [1, 2, 3, 4];
let result = arr.find(x => x > 2);
console.log(result); // 3
```

14. __indexOf()__ Devuelve el primer índice en el que un cierto elemento aparece en el array, o -1 si no se encuentra.

Sintaxis: 
```
array.indexOf(elemento, fromIndex)
```
Ejemplo:
```
let arr = [1, 2, 3];
let index = arr.indexOf(2);
console.log(index); // 1
```
15. __includes()__ Comprueba si un array contiene un elemento determinado, devolviendo true o false.

Sintaxis: 
```
array.includes(elemento)
```

Ejemplo:

```
let arr = [1, 2, 3];
let result = arr.includes(2);
console.log(result); // true
```

16. __sort()__ Ordena los elementos de un array en su lugar (modificando el array original).

Sintaxis: 

```
array.sort(function(a, b))
```

Ejemplo:

```

let arr = [3, 1, 2];
arr.sort();
console.log(arr); // [1, 2, 3]
```

17. __reverse()__ Invierte el orden de los elementos de un array en su lugar.

Sintaxis: 

```
array.reverse()
```

Ejemplo:

```
let arr = [1, 2, 3];
arr.reverse();
console.log(arr); // [3, 2, 1]
```

18. __some()__ Verifica si al menos un elemento del array cumple con la condición proporcionada.

Sintaxis: 

```
array.some(function(element, index, array))
```
Ejemplo:


```
let arr = [1, 2, 3];
let result = arr.some(x => x > 2);
console.log(result); // true
```
19. __every()__ Verifica si todos los elementos del array cumplen con la condición especificada.

Sintaxis: 

```
array.every(function(element, index, array))
```

Ejemplo:

```

let arr = [1, 2, 3];
let result = arr.every(x => x > 0);
console.log(result); // true
```

20. __findIndex()__ Devuelve el índice del primer elemento que cumpla con la condición proporcionada en la función.

Sintaxis: 

```
array.findIndex(function(element, index, array))
```
Ejemplo:


```
let arr = [1, 2, 3, 4];
let index = arr.findIndex((value)=>value===2)
console.log(index) // 1
```