Sebelum mengetahui apa itu JSX? Coba perhatikan kode yang ada di dalam file `App.jsx`

![Gambar]()

Aneh bukan? Di sana terdapat sintax HTML di dalam JavaScript. Yup itulah **JSX**

**JSX** adalah singkatan dari **JavaScript XML**. Ini adalah ekstensi sintaksis yang digunakan dalam React untuk memungkinkan penulisan kode HTML di dalam JavaScript.

```jsx
const App = () => {
  return (
    <div>
      <h1>Hello, World!</h1>;
      <h2>Selamat Datang Terra</h2>
    </div>
  )
} 
```

Kita tidak perlu repot lagi memikirkan DOM node mana yang nantinya akan dimanipulasi. 

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

> **NOTE**</br>
> Perlu diperhatikan bahwa **JSX** akan di-`return` untuk dapat ditampilkan.

