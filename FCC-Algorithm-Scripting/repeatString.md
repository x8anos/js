## ΕΠΑΝΑΛΗΨΗ STRING

**Επανέλαβε ένα δοσμένο string (πρώτο arguement) num φορές(δεύτερο arguement).
Επέστρεψε ένα άδειο string αν num δεν είναι θετικός αριθμός.**

Θα σε βοηθήσει:

[Global String Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)

```javascript
function repeatStringNumTimes(str, num) {
// repeat after me
var arr=[];
if (num>0){
  for (var i=0;i<=num-1;i++){
    arr[i]=str;
  }
 var joinedStr=arr.join("");
   return joinedStr;
}else str="";
   return str;
}

repeatStringNumTimes("abc", 4);
```
