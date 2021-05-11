# regex
Understanding use of regex methods.

1 [.test() method](#test-method)
2 [.match() method](#match-method)



## .test() method
Test method returns true/false. 
`Regex.test("Content of String")` 

### Plain search with .test() method
* Regex with case sensitive and find a match with a whole word.

```javascript
let myText = "Yes it is";
let myRegex = /Yes/;
let result = myRegex.test(myText);
//true

let anotherRegex = /yes/;
let anotherResult = myRegex.test(anotherRegex);
// false
```
* Regex with case insensitive and find a match with a whole word
* To make it add an `i` at the end of regex. Here `i` is 'ignore case'.

```javascript
let myText = "Yes it is";
let anotherRegex = /yes/i;
let anotherResult = anotherRegex.test(myText);
//true
```

### Conditional search with 'Or' `|` operator with .test() method
Here regex will return true if any of the given word matches

```javascript
let myText = "Yes, it is okay";
let myRegex = /yes|no|okay/;
let result = myRegex.test(myText);
// true . for matching one of the items 'okay'

```


## .match() method
