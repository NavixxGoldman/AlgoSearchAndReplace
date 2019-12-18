# AlgoSearchAndReplace
Algorithm of Search and Replace in Javascript

Perform a search and replace on the sentence using the arguments provided and return the new sentence.

First argument is the sentence to perform the search and replace on.

Second argument is the word that you will be replacing (before).

Third argument is what you will be replacing the second argument with (after).

#Note
Preserve the case of the first character in the original word when you are replacing it. For example if you mean to replace the word "Book" with the word "dog", it should be replaced as "Dog"

```javascript
function myReplace(str, before, after) {
  if (/^[A-Z]/.test(before)){
    
    let x=after[0].toUpperCase();
    let y= after.replace(after[0],x);
    
    str = str.replace(before, y);
  return str;
  }
   str = str.replace(before, after);
  return str;
}

console.log(myReplace("He is Sleeping on the couch", "Sleeping", "sitting"));
```
