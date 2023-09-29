## We've initialized an array arr. Use splice() to remove elements from arr, so that it only contains elements that sum to the value of 10.

```javascript
const arr = [2, 4, 5, 1, 7, 5, 2, 1];

arr.shift()
//splice elimina desde la (posicion, cantidad de elementos), y devuelve los elementos eliminados.
arr.splice(3,10)
console.log(arr);
```


## htmlColorNames should return ["DarkSalmon", "BlanchedAlmond", "LavenderBlush", "PaleTurquoise", "FireBrick"],  You should not use shift() or unshift() , You should not use array bracket notation.

```javascript
function htmlColorNames(arr) {
  const startIndex = 0;
  const amountToDelete = 2;
  arr.splice(startIndex, amountToDelete, "DarkSalmon", "BlanchedAlmond");
  return arr;
}

console.log(htmlColorNames(['DarkGoldenRod', 'WhiteSmoke', 'LavenderBlush', 'PaleTurquoise', 'FireBrick']));
```



## forecast should return ["warm", "sunny"],The forecast function should utilize the slice() method
```javascript
function forecast(arr) {
  //this remove the first 2 elements, and then remove from position 4 to nexts.
  return arr.slice(2,4)
}

// Only change code above this line
console.log(forecast(['cold', 'rainy', 'warm', 'sunny', 'cool', 'thunderstorms']))
```

## copyMachine([true, false, true], 2) should return [[true, false, true], [true, false, true]], copyMachine([1, 2, 3], 5) should return [[1, 2, 3], [1, 2, 3], [1, 2, 3], [1, 2, 3], [1, 2, 3]]
```javascript
function copyMachine( [...arr], num ) {
  let newArr = []
  while (num >= 1) {
    newArr.push( arr)
    num--;
  }
  return newArr;
}
console.log(copyMachine( [1, 2, 3], 2));
```