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

**JSX** adalah singkatan dari **JavaScript XML**. Ini adalah ekstensi sintaksis yang digunakan dalam React untuk memungkinkan penulisan kode HTML di dalam JavaScript.

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

# Quiz

Apa kegunaan utama JSX dalam React?
- [x] Memungkinkan penulisan kode HTML di dalam JavaScript
- [ ] Menggantikan JavaScript dengan HTML
- [ ] Meningkatkan performa aplikasi React
- [ ] Mengurangi kompleksitas kode JavaScript