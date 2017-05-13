## Mutations

**Return true if the string in the first element of the array contains all of
the letters of the string in the second element of the array.**

*For example, ["hello", "Hello"], should return true because all of the letters
in the second string are present in the first, ignoring case. The arguments
["hello", "hey"] should return false because the string "hello" does not contain
a "y". Lastly, ["Alien", "line"], should return true because all of the letters
in "line" are present in "Alien".*

*Here are some helpful links:*

[String.prototype.indexOf()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/indexOf)

```javascript
function mutation(arr) {
   var check;
   var j=0; // counts characters
   var arr0=arr[0].toLowerCase();
   var arr1=arr[1].toLowerCase();
   var tempArr=arr1.split("");  
   for(var i=0;i<tempArr.length;i++){
      if(arr0.indexOf(tempArr[i])>=0){
       j++;
    }
  }
  if(j==tempArr.length){
    check=true;
  }else check=false;
  return check;
}
mutation(["hello", "hey"]);
```
