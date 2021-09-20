## Specs

Buatlah sebuah function yang menerima 3 buah input.
- `str` (required) => Sebuah kalimat/frase berupa `string`
- `length` (`default = 100`) => Jumlah batasan sebuah teks ditampilkan. Nilai `default` akan dijalankan jika user tidak memasukkan argumen ini pada function.
- `ending` (`default = ...`) => Karakter `string` yang digunakan untuk menandakan bahwa kalimat/frtase tersebut dihide karena melebihi batas maksimal teks yang ditampilkan.

## Expected Result

- `console.log(text_truncate('We are doing JS string exercises.'))`
- output: `We are doing JS string exercises.`

- `console.log(text_truncate('We are doing JS string exercises.',19))`
- output: `We are doing JS ...`

- `console.log(text_truncate('We are doing JS string exercises.',15,'!!'))`
- output: `We are doing !!`