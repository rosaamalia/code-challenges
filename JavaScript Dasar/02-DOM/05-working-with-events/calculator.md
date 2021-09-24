## Specs

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8" />
    <title>Calculator</title>
  </head>
  <body>
    <label
      >Square this number:
      <input type="number" id="square-input" size="2" />
    </label>
    <button id="square-button">Calculate</button>
    <br /><br />

    <label
      >Half this number:
      <input type="number" id="half-input" size="2" />
    </label>
    <button id="half-button">Calculate</button>
    <br /><br />

    <label
      >Calculate area of circle with radius:
      <input type="number" id="area-input" size="2" />
    </label>
    <button id="area-button">Calculate</button>
    <br /><br />
    <div id="solution"></div>
  </body>
  ```

- Add a script tag and make function of every operation
- For each operation, create an event listener for the button, and when it's clicked, find the value of the appropriate input and show the result of the calculation in the solution div.

## Expected Result
- Initial page
![expected-result-1](https://skilvul-prod-01.s3.ap-southeast-1.amazonaws.com/lesson/full-stack-assignment/code-challenge-dom-event-1.png)
- Square Number
![expected-result-2](https://skilvul-prod-01.s3.ap-southeast-1.amazonaws.com/lesson/full-stack-assignment/code-challenge-dom-event-2.png)
- Half Number
![expected-result-3](https://skilvul-prod-01.s3.ap-southeast-1.amazonaws.com/lesson/full-stack-assignment/code-challenge-dom-event-3.png)  