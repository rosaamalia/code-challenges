## Specs

Buatlah sebuah function untuk generate random `integer` dar 2 buah input `integer` yaitu nilai minimum `min` dan maksimum `max`. Nilai random harus berada pada range tersebut.

- Jika nilai `min` dan `max` adalah `null`, maka function mengembalikan hasil `0`
- Jika nilai `max` adalah `null`, jadikan nilai `min` menjadi `0` dan `max` mengambil nilai dari `min`

## Expected Result
- `console.log(rand(20,1));`
- Output: `4`

- `console.log(rand(1,10));`
- Output: `1`

- `console.log(rand(6));`
- Output: `2`

- `console.log(rand());`
- Output: `0`