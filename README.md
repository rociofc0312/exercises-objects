# exercises-objects

## Contador de propiedades

Dado un objeto como parámetro, contar la cantidad de propiedades que este
contiene y retornarlo.

Ejemplo:

```javascript
const output = objectPropertiesCounter({ 'name': 'John', 'lastname': 'Doe' });
console.log(ouput); // => 2
```

## addArrayProperty

Escribe una función llamada `addArrayProperty(obj, key, array)`.

Dado un objeto, una llave y un array, `addArrayProperty` asigna una nueva
propiedad sobre el objeto en la lave dada, con el array dado como valor.

Ejemplo de entrada:

```js
const myObj = {};
const myStr = 'myProperty';
const myArray = [1, 3];
addArrayProperty(myObj, myStr, myArray);
console.log(myObj.myProperty); // => [1, 3]
```

## removeStringValuesLongerThan

Escribe una función llamada `removeStringValuesLongerThan`.

Dado un número y un objeto, `removeStringValuesLongerThan` elimina cualquier
propiedad en el objeto dado cuyos valores son cadenas de texto más largas que el
número dado.

Ejemplo de entrada:

```js
const obj = {
  name: 'Montana',
  age: 20,
  location: 'Texas',
};
removeStringValuesLongerThan(6, obj);
console.log(obj); // => { age: 20, location: 'Texas' }
```

## getSumOfAllElementsAtProperty

Escribe una función llamada `getSumOfAllElementsAtProperty`.

Dado un objeto y una key, `getSumOfAllElementsAtProperty` devuelve la suma de
todos los elementos del array.

Notas:

- Si el array está vacío, debe devolver `0`.
- Si la propiedad en la key dada no es un array, debe devolver `0`.
- Si no hay ninguna propiedad en la key dada, debe devolver `0`.

```js
const obj = {
  key: [4, 1, 8],
};
const output = getSumOfAllElementsAtProperty(obj, 'key');
console.log(output); // => 13
```

## addFullNameProperty

Escribe una función llamada `addFullNameProperty(person)`.

Dado un objeto `person` con una propiedad `firstName` y una propiedad
`lastName`, `addFullNameProperty(person)` debe retornar un nuevo objeto con las
mismas propiedades que el objeto recibido pero con una propiedad más `fullName`,
cuyo valor debe ser una cadena (string) con el nombre y el apellido separados
por un espacio.

```js
const person = {
  firstName: 'Jade',
  lastName: 'Smith',
};
const personWithFullName = addFullNameProperty(person);
console.log(personWithFullName.fullName); // => 'Jade Smith'
console.log(personWithFullName.firstName); // => 'Jade'
console.log(personWithFullName.lastName); // => 'Smith'
```

## transformFirstAndLast

Escribe una función `transformFirstAndLast` que toma un array y devuelve un
objeto con:

1. el primer elemento del array como la llave del objeto, y
2. el último elemento del array como valor de esa llave.

Ejemplo de entrada:

```js
['Queen', 'Elizabeth', 'Of Hearts', 'Beyonce']
```

Valor de retorno de la función (salida):

```js
{
  Queen: 'Beyonce'
}
```

No cambies el array de entrada. Piensa que todos los elementos del array de
entrada serán del tipo `string`.

Ten en cuenta que el array de entrada puede tener un número variable de
elementos. Tu código debería acomodarse de manera flexible.

Ejemplo, debe manejar la entrada como:

```js
['Kevin', 'Bacon', 'Amor', 'Hart', 'Costner', 'Spacey']
```

Valor de retorno de la función (salida):

```js
{
  Kevin: "Spacey"
}
```

## fromListToObject

Escribe una función `fromListToObject` que toma un array de matrices, y
devuelve un objeto con cada par de elementos en la array como un par
llave-valor.

Ejemplo de entrada:

```js
[['make', 'Ford'], ['model', 'Mustang'], ['year', 1964]]
```

Valor de retorno de la función (salida):

```js
{
  make: 'Ford'
  model: 'Mustang',
  year: 1964
}
```

No cambies la cadena de entrada. Piensa que todos los elementos del array serán
del tipo `string`.

Ten en cuenta que la entrada puede tener un número diferente de elementos que
la muestra dada. Por ejemplo, si la entrada tiene 6 valores en lugar de 4, tu
código debería adaptarse de manera flexible.

## listAllValues

Escribe una función llamada `listAllValues` que devuelve un array de todos los
valores del objeto de entrada.

Ejemplo de entrada:

```js
{
  name: 'Krysten',
  age: 33,
  hasPets: false
}
```

Valor de retorno de la función (salida):

```js
['Krysten', 33, false]
```

Ten en cuenta que la entrada puede tener un número diferente de llaves y
valores que la muestra dada.

Por ejemplo, también debe manejar una entrada como:

```js
{
  a: 'a',
  number: 11,
  hungry: true,
  grammyWins: 1
}
```

Valor de retorno de la función (salida):

```js
['a', 11, true, 1]
```

