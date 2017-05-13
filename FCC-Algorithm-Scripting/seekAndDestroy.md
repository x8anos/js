# Seek and destroy

**You will be provided with an initial array (the first argument in the
destroyer function), followed by one or more arguments. Remove all elements from
the initial array that are of the same value as these arguments.**

*Here are some helpful links:*

[Arguments object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions/arguments)

[Array.prototype.filter()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/filter?v=example)

```javascript
  function destroyer(arr) {
      // Remove all the values
      return arr;
    }

    destroyer([1, 2, 3, 1, 2, 3], 2, 3);
```
