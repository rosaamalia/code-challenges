## Specs

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset=utf-8 />
    <title>Remove items from a dropdown list</title>
  </head>
  <body>
    <form>
      <select id="colorSelect">
        <option>JavaScript</option>
        <option>Python</option>
        <option>Go</option>
        <option>Ruby</option>
      </select>
      <input type="button" onclick="removeProgrammingLanguage()" value="Select and Remove">
    </form>
  </body>
</html>
```

Buatlah sebuah function bernama `removeProgrammingLanguage` tanpa parameter untuk menghapus element yang dipilih saat user klik `button` `select and Remove`.

## Expected Results
- User memilih list yang ingin di hapus
![step-1](https://skilvul-prod-01.s3.ap-southeast-1.amazonaws.com/lesson/full-stack-assignment/code-challenge-dom-delete-items-1.png)
- User klik `button` `Select and Remove`
![step-2](https://skilvul-prod-01.s3.ap-southeast-1.amazonaws.com/lesson/full-stack-assignment/code-challenge-dom-delete-items-2.png)
- Item `python` sudah berhasil terhapus dari list dropdown
![step-3](https://skilvul-prod-01.s3.ap-southeast-1.amazonaws.com/lesson/full-stack-assignment/code-challenge-dom-delete-items-3.png)