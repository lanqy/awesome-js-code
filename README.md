# awesome-js-code
An awesome list of js code

## Shuffle

```js
// Code stolen from http://bost.ocks.org/mike/shuffle/
// Was looking for a good example of a Fisher–Yates shuffle
function shuffle(array) {
  let m = array.length;
  let t;
  let i;

  // While there remain elements to shuffle…
  while (m) {
    // Pick a remaining element
    i = Math.floor(Math.random() * m--);

    // And swap it with the current element.
    t = array[m];
    array[m] = array[i];
    array[i] = t;
  }

  return array;
}
```

## Generate random number between two numbers

```js
function _random(min, max) { // Generate random number between two numbers
    return Math.floor(Math.random() * (max - min + 1) + min);
}
```
