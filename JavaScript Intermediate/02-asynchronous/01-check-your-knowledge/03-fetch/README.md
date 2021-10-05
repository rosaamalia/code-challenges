### Soal 1
Which of the following is NOT used to create a request using `fetch()` and explain why?
A. `.this()`

B. `.then()`

C. `.json()`

D. `JSON.stringify()`
### Jawaban 1
Jawab di bawah ini
...

### Soal 2
A Promise is a(n)
A. object

B. method

C. state

D. function
### Jawaban 2
Jawab di bawah ini
...

### Soal 3
What is wrong with the following code?
```js
async function getData() {
  try {
    let response = await fetch('https://api-to-call.com/endpoint', { 
      method: 'POST', 
      body: JSON.stringify({id: 200}), 
      dataType: 'json'
  });
  let jsonResponse = await JSON.stringify(response);
  return jsonResponse;
  } catch (error) {
    console.log(error);
  }
}
```
### Jawaban 3
Jawab di bawah ini
...

### Soal 4
What is wrong with the following code?
```js
async function getData() {
  try {
    let response = await fetch('https://api-to-call.com/endpoint', 'POST', JSON.stringify({id: 200}), 'json');
    let jsonResponse = await response.json();
    return jsonResponse;
  } catch (error) {
    console.log(error);
  }
}
```
Jawaban 4
Jawab di bawah ini
...