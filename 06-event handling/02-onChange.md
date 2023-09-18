`onChange` adalah _prop_ yang umum digunakan pada elemen seperti `<input>`, `<textarea>` dan `<select>`. Ini memungkinkan kita menangani perubahan nilai pada elemen tersebut. Contohnya:

```jsx
function App() {
  function handleChange(event) {
    console.log(event.target.value);
  }

  return <input type="text" onChange={handleChange} />;
}
```

Pada kode di atas, akan menampilkan tulisan pada `console` jika kamu mengetik sesuatu pada text input.

Text input di atas diberi `onChange` yang akan menjalankan `handleChange` jika terjadi perubahan pada text input tersebut.

`handleChange` memiliki parameter `event` yang berasal dari `onChange`. Parameter ini digunakan untuk menangkap hasil ketikan pada text input dengan cara memanggil `event.target.value`

Kamu juga bisa menyimpan hasil ketikan tersebut kedalam sebuah state, contohnya seperti ini:

```jsx
function App() {
  const [nama, setNama] = useState("");

  function handleChange(event) {
    setNama(event.target.value);
  }

  return (
    <>
      <input 
        type="text" 
        name="nama" 
        onChange={handleChange} 
      />
      <h1>{nama}</h1>
    </>
  );
}
```
Pada kode di atas, hasil ketika akan disimpan ke dalam _state_ menggunakan `setNama`. Dengan begitu `<h1>` dapat menampilkan data hasil ketikan tersebut dengan adanya _state_

---
Untuk mengasah pemahaman mu, silahkan ikuti eksperimen berikut.

1. Buat komponen `Login`.
2. Memiliki `text input`, yaitu `username` dan `password`.
3. Memiliki `button` login.
4. Simpan data `username` dan `password` ke dalam state.
5. Tampilkan `username` dan `password` ke console ketika tombol login di tekan

Hasilnya seperti ini



# Quiz

### 5 point
 Apa tujuan penggunaan prop `onChange` dalam elemen seperti `<input>`,`<textarea>`, dan `<select>` dalam React?

- [ ] Untuk mengubah gaya tampilan elemen tersebut.
- [x] Untuk menangani perubahan nilai pada elemen tersebut.
- [ ] Untuk menampilkan elemen tersebut ke layar.
- [ ] Untuk menghapus elemen tersebut dari tampilan.