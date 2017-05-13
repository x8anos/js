## CHUNKY MONKEY

**Write a function that splits an array (first argument) into groups the length
of size (second argument) and returns them as a two-dimensional array.**

*Here are some helpful links:*

[Array.prototype.push()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/push?v=example)

[Array.prototype.slice()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/slice?v=example)

```javascript
function chunkArrayInGroups(arr, size) {
  var sl=[];                                  
  var j=0;
  for(var i=0;i<arr.length/size;i++){
      sl.push(arr.slice(j,size*(i+1)));
      j+=size;         
  }
   return sl;
}

chunkArrayInGroups(["a", "b", "c", "d"], 2);
```
