## ΕΠΑΛΗΘΕΥΣΗ ΚΑΤΑΛΗΞΗΣ

**Έλεγξε αν ένα string καταλήγει με το δοσμένο string στόχο, για δύο arguements,
το μεν πρώτο το βασικό string (str) και το δεύτερο ο στόχος (target).**

Να μην λυθεί με την .endsWith() μέθοδο, η οποία εισήχθηκε με την  ES2015,
αλλά να χρησιμοποιηθεί μια μέθοδος substring της JavaScript.

Χρήσιμες μέθοδοι:

    String.prototype.substr()

    String.prototype.substring()


```javascript
function confirmEnding(str, target) {
  tLen=target.length;   //το μήκος του στόχου
  sLen=str.length;      //το μήκος του βασικού string
  var temp=str.substring(str.length-tLen); //το τέλος του βασικού για μήκος...
  if (temp===target)
    return true;
  else
  return false;
}

confirmEnding("Frederico Garcia", " Garcia");
```
