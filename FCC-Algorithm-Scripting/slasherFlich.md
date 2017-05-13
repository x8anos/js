## Slasher Flick

**Return the remaining elements of an array after chopping off n elements from
the head. The head means the beginning of the array, or the zeroth index.**

*Here are some helpful links:*

[Array.prototype.slice()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/slice?v=example)

[Array.prototype.splice()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/splice?v=example)

```javascript
function slasher(arr, howMany) {
  arr.splice(0,howMany);
  return arr;
}
slasher([1, 2, 3], 2);
```
// splice() is changing the contents of an array in contrast to slice()
