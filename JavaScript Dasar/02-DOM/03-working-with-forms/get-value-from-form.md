## Specs

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset=utf-8 />
    <title>Return first and last name from a form</title>
  </head>
  <body>
    <form id="form1" onsubmit="getFormvalue()">
      First name: <input type="text" name="fname" value="Marc"><br>
      Last name: <input type="text" name="lname" value="Marquez"><br>
      <input type="submit" value="Submit">
    </form>
  </body>
</html>
```

Buatlah sebuah function `getFormValue` tanpa parameter untuk mengembalikan nilai yang diinputkan oleh user pada `console`

## Expected Result
- User menginput data form
![fill-form](https://skilvul-prod-01.s3.ap-southeast-1.amazonaws.com/lesson/full-stack-assignment/code-challenge-dom-form-1.png)
- Tampilkan pada console
![fill-form](https://skilvul-prod-01.s3.ap-southeast-1.amazonaws.com/lesson/full-stack-assignment/code-challenge-dom-form-2.png)