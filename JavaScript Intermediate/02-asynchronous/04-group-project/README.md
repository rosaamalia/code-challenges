## Expected Result

![expected-result](https://skilvul-prod-01.s3.ap-southeast-1.amazonaws.com/lesson/full-stack-assignment/code-challenge-asynchronous-06.gif)

## Specs
Pada kesempatan kali ini kita akan melanjutkan *code challege* sebelumnya yaitu `03-group-project`, kali ini kita akan menammbahkan 2 fitur baru yaitu:
- hapus data komentar yang sudah ada
- menambahkan data komentar baru

> perlu diperhatikan bahwa setiap perubahan yang kalian buat itu hanya akan memberikan sebuah *response*, dan setiap data yang kalan tambahkan atau hapus tidak akan disimpan pada *server* `jsonplaceholder API` jadi kita hanya membutuhkan response dari *API call* tersebut

Berikut merupakan langkah-langkah yang dapat kalian gunakan untuk menyelesaikan permasalahan diatas:
- tambahkan sebuah `button` pada fungsi `createListElement` dengan cara merubah fungsi tersebut menjadi baris kode dibawah

  ```Javascript
  const createListElement = (comment) => {
    const elListItem = document.createElement("div");
    elListItem.insertAdjacentHTML(
      "beforeend",
      `<div class="list-group-item d-flex justify-content-between">
        <div class="ms-2 me-auto">
          <div class="fw-bold">
            ${comment.email}
          </div>
          <span>${comment.body}</span>
        </div>
        <button
          type="button"
          class="btn btn-sm btn-outline-danger text-uppercase delete-btn"
          comment-id="${comment.id}"
        >
          delete
        </button>
      </div>`
    );

    return elListItem;
  };
  ```
- buat fungsi `createComment` didalam file `helpers.js`, berikut merupakan deskripsi dari fungsi tersebut:
  - name => `createComment`
  - description => fungsi ini akan melakukan *API call* untuk membuat sebuah *comment* baru
  - parameter
    - comment [`Object`] => comment merupakan data komentar yang akan kita kirim ke `jsonplaceholder API`, ia memiliki bentuk sebagai berikut
      ```Javascript
      {
        "postId": 2, // Number -> id dari sebuah post
        "name": "John Watson", // String -> nama dari penulis komentar
        "email": "john_watson@mail.com", // String -> email dari penulis komentar
        "body": "hello this is my first comment" // String -> komentar yang kita lontarkan pada sebuah post
      }
      ```
  - response
    - success => `status: 201`
    - fail => `status: 400 OR 500`

- buat fungsi `removeComment` didalam file `helpers.js`, berikut merupakan deskripsi dari fungsi tersebut:
  - name => `removeComment`
  - description => fungsi ini akan melakukan *API call* untuk menghapus sebuah *comment*
  - parameter
    - post_id [`Number`] => id dari post yang akan kita hapus
  - response
    - success => `status: 200`
    - fail => `status: 400 OR 500`
- tambahkan `button` `create new comment` dengan cara memasukan baris kode berikut tepat dibawah element dengan `id="list-group"`
  ```HTML
  <button
    id="btn-new-comment"
    class="btn btn-outline-primary w-100 text-capitalize"
    data-bs-toggle="modal"
    data-bs-target="#new-comment-modal"
  >
    create new comment
  </button>
  ```
- tambahkan `modal` dengan cara memasukan baris kode berikut dibawah element dengan `id="komentar-berita"`
  ```HTML
  <div
    class="modal fade"
    id="new-comment-modal"
    tabindex="-1"
    aria-labelledby="new-comment-modal"
    aria-hidden="true"
    >
    <div class="modal-dialog">
      <div class="modal-content">
        <div class="modal-header">
          <h5 class="modal-title" id="exampleModalLabel">New Comment</h5>
          <button
            type="button"
            class="btn-close"
            data-bs-dismiss="modal"
            aria-label="Close"
          ></button>
        </div>
        <div class="modal-body">
          <form id="form-new-comment">
            <div class="mb-3">
              <label for="name" class="form-label">
                Name
              </label>
              <input
                type="name"
                name="name"
                class="form-control"
                id="namme"
              />
            </div>
            <div class="mb-3">
              <label for="email" class="form-label">
                Email address
              </label>
              <input
                type="email"
                name="email"
                class="form-control"
                id="email"
              />
            </div>
            <div class="mb-3">
              <label for="body" class="form-label">
                Comment
              </label>
              <textarea
                name="body"
                id="body"
                class="form-control"
              ></textarea>
            </div>
            <div>
              <button
                type="button"
                class="btn btn-outline-secondary"
                data-bs-dismiss="modal"
              >
                Close
              </button>
              <button
                type="submit"
                class="btn btn-success text-capitalize"
              >
                submit
              </button>
            </div>
          </form>
        </div>
      </div>
    </div>
  </div>
  ```
- 