# Falcy bouncer

**Remove all falsy values from an array.Falsy values in JavaScript are false,
null, 0, "", undefined, and NaN.**

*Here are some helpful links:*

[Boolean Objects](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean)

[Array.prototype.filter()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/filter?v=example)

```javascript
function bouncer(arr) {
 //create an inner function to check if not falcy
   function removeFalcy(value){
       return value;
   }  
  var filtered=arr.filter(removeFalcy);
  return filtered;
}

bouncer([7, "ate", "", false, 9]);
```
