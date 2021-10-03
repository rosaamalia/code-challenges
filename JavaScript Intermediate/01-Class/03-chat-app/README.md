## Specs

A chat appss named **SkilChat** takes a plain text message and shifts each letter forward in the alphabet by a given number. For example, a shift cipher with a shift of 1 would turn the string `'hello'` to `'ifmmp'`.

Create a class `SkilChat` that takes the numerical value of the shift as a constructor parameter. The class should have two methods:

`encrypt`: takes a plain text string and returns a capitalized string with each letter shifted forward in the alphabet based on the set shift value.
`decrypt`: takes an encrypted message and returns a lower case string with each letter shifted back in the alphabet based on the set shift value.
In both methods, any character outside the alphabet should remain the same.
But if a character is shifted outside the alphabet in either direction it should be wrapped around to the other side. For example, encrypting a `y` with a shift of `4` results in `C` and decrypting an `A` with a shift of `1` result in `z`.

## Expected Result
```js
const mySkilChat = new SkilvulChat(2);
mySkilChat.encrypt('I love JavaScript!'); // returns 'K NQXG LCXCUETKRV!'
mySkilChat.decrypt('K <3 OA ECV'); // returns 'i <3 my cat'
```

## Notes
Feel free to reference the [Unicode Table](https://en.wikipedia.org/wiki/List_of_Unicode_characters) as well as the [JavaScript String methods](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String) including: `toUpperCase()`, `toLowerCase()`, `charCodeAt()` and `fromCharCode()`