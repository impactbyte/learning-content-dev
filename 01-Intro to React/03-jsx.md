Sebelum mengetahui apa itu JSX? Coba perhatikan kode yang ada di dalam file `App.jsx`

```jsx
function App () {
  return (
    <div>
      <h1>Hello, World!</h1>;
      <h2>Selamat Datang Terra</h2>
    </div>
  )
} 
```

Aneh bukan? Di sana terdapat sintax HTML di dalam JavaScript. Yup itulah **JSX**.

**JSX** adalah adalah ekstensi sintaksis yang digunakan dalam React, sehingga memungkinkan menulis markup yang mirip HTML di dalamn file JavaSctipt.

**Dengan JSX, kita bisa dengan mudah membuat tampilan dan menyisipkan konten seperti sedang menggunakan HTML**.

Kita juga bisa menyisipkan kode JavaScript ke dalam **JSX** dengan menambahkan **kurung kurawal `{}`** seperti ini

```jsx
const App = () => {
  let nama = 'Terra'

  return (
    <div>
      <h1>Hello, World!</h1>;
      <h2>Selamat Datang {nama}</h2>
    </div>
  )
} 
```

Beberapa peraturan untuk menggunakan JSX
1. Satu element yang di-return

    Komponen tidak dapat me-_return_ lebih dari satu element. Maka dari itu harus dibungkus suatu element atau dengan **React fragment**.

    ```jsx
    <div>
      {/* beberapa element di dalam */}
    </div>
    ```
    Atau dengan **React fragment**
    ```jsx
    <>
      {/* beberapa element di dalam */}
    </>
    ```
2. Semua tag harus ditutup
    
    Sudah sewajarnya jika menulis tag akan ada tag pembuka dan tag penutup. Untuk tag yang bersifat single tag pun juga harus ditutup, contoh:
    ```jsx
      <>
        <p></p>
        <img />
        <br />
      </p>
    ```

3. Penggunaan camelCase

    JSX pada dasarnya adalah JavaScript, maka jika ada penulisan yang memiliki penamaan lebih dari 1 kata, maka gunakan format `camelCase`, contoh:
    ```jsx
      <img 
        src=""
        className="" //camelCase
        onClick={} // camelCase
      />
    ```


> **NOTE**</br>
> Perlu diperhatikan bahwa **JSX** akan di-`return` untuk dapat ditampilkan.

# Quiz

### 5 point
Apa kegunaan utama JSX dalam React?
- [x] Memungkinkan penulisan kode HTML di dalam JavaScript
- [ ] Menggantikan JavaScript dengan HTML
- [ ] Meningkatkan performa aplikasi React
- [ ] Mengurangi kompleksitas kode JavaScript

### 15 point
Perhatikan kode berikut
```jsx
const App = () => {
  let buah = ['pisang', 'mangga', 'jeruk']

  return (
    <div>
      <h1>Saya suka buah (buah[1])</h1>;
    </div>
  )
} 
```
Mana kah bagian yang bermasalah?
- [ ] penggunaan `buah[1]`
- [ ] penggunaan kurung `( )`
- [ ] penggunaan `return`
- [ ] Tidak ada yang bermasalah