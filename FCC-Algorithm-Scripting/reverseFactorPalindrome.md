
# ΑΝΑΣΤΡΟΦΗ STRING

### 1η έκδοση

```javascript
function reverseString(str) {
  var pinakas=[];
  pinakas=str.split("");
  var revPinakas;
  revPinakas=pinakas.reverse();
  str=revPinakas.join("");  // αν δεν βάλω ("") και το αφήσω () θα προσθέσει
  return str;               // (,) ανάμεσα στους χαρακτήρες
}
reverseString("hello");     //"olleh"
```

### 2η έκδοση δήλωση και ανάθεση σε μια γραμμή......

```javascript
function reverseString(str) {
        var pinakas=str.split("");
        var revPinakas=pinakas.reverse();
        str=revPinakas.join("");
        return str;
 }

 reverseString("hello");
```

# ΠΑΡΑΓΟΝΤΟΠΟΙΗΣΗ ΑΡΙΘΜΟΥ (FACTORING)

```javascript
function factorialize(num) {
  if (num===0){
    num=1;
  }else{
       for(var i=num-1;i>=1;i--){
          num*=i;
        }
       }
   return num;
 }
factorialize(5);      //120
```

# ΕΛΕΓΧΟΣ ΠΑΛΙΝΔΡΟΜΗΣΕΩΝ (PALINDROMES)

**Παλινδρόμηση είναι μια φράση ή λέξη που διαβάζεται το ίδιο κανονικά ή ανάποδα,
αγνοώντας κενούς χαρακτήρες, σύμβολα στίξης και σύμβολα.**

*Παράδειγμα επιστροφής σωστού ή λάθους αν μια έκφραση είναι παλινδρόμηση αφού
αφαιρέσουμε τους μη αλφαριθμητικούς χαρακτήρες:*

```javascript
function palindrome(str) {
     //turn all letters to lowercase
       var strL=str.toLowerCase();
     //extract non alphanumerics
       var stripStr=strL.replace(/[^0-9a-z]/g,"");

     //reverse string
       var tempArray=strL.split("");
       var revArray=tempArray.reverse();
       strL=revArray.join("");

       var newStr=strL.replace(/[^0-9a-z]/g,"");

     if(stripStr==newStr)
        return true;
     else return false;
   }
palindrome("eye");
```
