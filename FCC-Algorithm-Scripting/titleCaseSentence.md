--------------------------------------------------------------------------------
**Return the provided string with the first letter of each word capitalized.
Make sure the rest of the word is in lower case. For the purpose of this
exercise, you should also capitalize connecting words like "the" and "of".**

# SPLIT A STRING

```javascript
function titleCase(str) {
  var tempArr=str.split(" ");

  return tempArr;
}
titleCase("I'm a little tea pot");//Array [ "I'm", "a", "little", "tea", "pot" ]
```

### NOT WORKING TRY TO TURN TO LOWERCASE

```javascript
function titleCase(str) {
  var tempArr=str.split(" ");
  var result="";

  for(var i=0;i<tempArr.length;i++){
       tempArr[i].toLowerCase();
       tempArr[i].split("");
       tempArr[i][0].toUpperCase();
  }
  result=tempArr.join(" ");
  return result;
}
titleCase("I'm A litTle tea pot");
```

### WORKING HALF WAY THROUGH

*Declare an extra value to turn all the letters to lowercase from the begin*

```javascript
function titleCase(str) {
  var strL=str.toLowerCase();
  var tempArr=strL.split(" ");

  return tempArr;
}
titleCase("I'm A litTle tea pot");
```
### FOUND THE ANSWER IN STACKOVERFLOW

```javascript
function titleCase(str) {
   var splitStr = str.toLowerCase().split(' ');//
   for (var i = 0; i < splitStr.length; i++) {
       // You do not need to check if i is larger than splitStr length,
       // as your for does that for you
       // Assign it back to the array
       // Η μέθοδος substring επιλέγει το κομμάτι από τον χαρακτήρα στη θέση 1
       //και μετά.
   splitStr[i] = splitStr[i].charAt(0).toUpperCase() + splitStr[i].substring(1);
   }
   // Directly return the joined string
   return splitStr.join(' ');
}
titleCase("I'm a little tea pot");
```javascript

*Χρήση charAt  και  substring δύο μεθόδων String.prototype*

```javascript
function titleCase(str) {
  var tempArr=str.split(" ");
  var result="";

  for(var i=0;i<tempArr.length;i++){
       tempArr[i].toLowerCase();
       tempArr[i].split("");
       tempArr[i][0].toUpperCase();
  }
  result=tempArr.join(" ");
  return result;
}
titleCase("I'm A litTle tea pot");
```
