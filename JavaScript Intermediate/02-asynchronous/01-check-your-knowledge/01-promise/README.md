### Soal 1
How many parameters does a Promise constructor take?
```js
const example = new Promise( ... );
```
### Jawaban 1
Jawab di bawah ini
...

### Soal 2
What state will this promise be in after 0 seconds?
```js
const thePromise = () => {
  return new Promise((resolve, reject) => {
    if (true) {
      setTimeout( () => resolve('success'), 3000);
    } else {
      setTimeout( () => resolve('failed'), 5000);
    }
  });
};
```
### Jawaban 2
Jawab di bawah ini
...

### Soal 3
True or False: The `.then()` method returns a Promise.
### Jawaban 3
Jawab di bawah ini
...

### Soal 4
Which of the executor function’s parameters is called if the asynchronous task completes successfully?
```js
const thePromise = new Promise( (function1, function2) => { . . . } );
```
### Jawaban 4
Jawab di bawah ini
...

### Soal 5
What will be printed to the console after running the code provided?
```js
let status = state => {
  return new Promise(function(resolve, reject) {
    if (state) { 
      resolve('success'); 
    } else { 
      reject('error');
    }
  });
}
 
let promiseChain = status(true);
 
promiseChain
.then( data => {  
   console.log(data + " 1");
   return status(true);
})
.then( data => {
   console.log(data+ " 2");
   return status(true);
});
```
### Jawaban 5
Jawab di bawah ini
...

### Soal 6
Which one of the following is NOT a state that a Promise resolves to?
A. Pending

B. Undefined

C. Fulfilled

D. Rejected
### Jawaban 6
Jawab di bawah ini ...

### Soal 7
What is the value of the argument that is passed to the `onReject()`?
```js
let onFulfill = value => {console.log(value)};
let onReject = reason => {console.log(reason)};
 
const thePromise =  new Promise( (resolve, reject) => {
  if (false) {
    resolve('success value');
  } else {
    reject();
  }
});
 
thePromise.then(onFulfill, onReject);
```
### Jawaban 7
Jawab di bawah ini ...

### Soal 8
What value is printed to the console?
```js
const asyncGreeting = new Promise((resolve, reject) => {
  setTimeout(resolve, 1000, 'Hello!');
});

console.log(typeof asyncGreeting);
```
### Jawaban 8
Jawab di bawah ini
...