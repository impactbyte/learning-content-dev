Menangani klik mouse pada suatu element, kita bisa menggunakan props `onClick`. Bisa diletakkan pada semua element yang ingin beri klik. 

Contohnya seperti ini:

```jsx
function App() {
  const [greeting, setGreeting] = useState("Say")

  function handleClick() {
    setGreeting("Hello")
  }

  return (
    <>
      <h1 onClick={handleClick}>{greeting}</h1>
    </>
  );
}
```

Pada kode di atas, terdapat element `<h1>` yang menampilkan tulisan `"Say"`. Ketika tulisan tersebut diklik, maka akan berubah menjadi `"Hello"`.

Tulisan `<h1>` di atas berasal dari _state_ `greeting` dan  dapat diklik karena memiliki `onClick` yang akan memanggil function `handleClick`. Ketika diklik maka _function_ `handleClick` dijalankan untuk mengubah _state_ `"Say"` menjadi `"Hello"` menggunakan `setGreeting("Hello")`.

---
Untuk mengasah pemahaman mu, silahkan ikuti eksperimen berikut.

<!-- Latihan buat counter -->