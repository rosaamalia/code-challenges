## Expected Result
![expected-result](https://skilvul-prod-01.s3.ap-southeast-1.amazonaws.com/lesson/full-stack-assignment/code-challenge-async-fetch-1.png)

## Specs
Buatlah aplikasi website sesuai desain dan contoh data di atas dimana kita akan mengambil data dari External API **Random User Generator** untuk mengambil data multiple user.

- Gunakan template yang sudah disediakan pada file `index.html` dan `style.css`. Jangan melakukan perubahan apapun pada kedua file tersebut.
- Kita akan melakukan `fetch` data dari https://randomuser.me/documentation#multiple
- Gunakan endpoint berikut `https://randomuser.me/api/?results=2`
- Buatlah code kamu pada `app.js`
- Buat 2 function di dalam file `app.js` yaitu `getUsers()` dan `renderUsers()`
- Pada function `getUsers()` lakukan proses get data dari Endpoint yang disediakan dan funtion harus mengembalikan data Array of Object yang berisi data 2 user
- Pada function `renderUsers()` lakukan proses rendering data untuk menampilkan konten pada file `.html` yang sudah disediakan.
- Panggil function `renderUsers()` di dalam file `app.js`