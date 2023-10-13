Pada topic sebelumnya, kita sudah mencoba me-_render_ JSX serta menyisipkan kode JavaScript ke dalamnya. Berikutnya kita akan mencoba **_conditonal_ dan _loop_ rendering pada JSX**

### Conditional

Opsi pertama kita bisa menggunakan perintah _**conditional**_ seperti `if else` dan `switch` yang diberi `return` seperti contoh di bawah.

```jsx
function App() {
  let isLoggedIn = true;

  if (isLoggedIn) {
    return <h1>Welcome back!</h1>;
  } else {
    return <h1>Please log in.</h1>;
  }
}
```

Atau juga bisa menggunakan _**ternary operator**_ jika ingin menyisipkan **_conditional_** kedalam JSX seperti ini.

```jsx
function App() {
  let isLoggedIn = true

  return (
    {isLoggedIn ?
      <h1>Welcome back!</h1> 
      : 
      <h1>Please log in.</h1>;
    }
  )
}
```

> **Note**</br>
> _**ternary operator**_ lebih sering digunakan untuk melakukan pengkondisian pada JSX

### Loop

Loop rendering bisa kita lakukan dengan menggunakan `map()`. Perlu diingat bahwa `map()` hanya dapat digunakan untuk data array

```jsx
function App() {
  let listBuah = ["jeruk", "rambutan", "pepaya"]

  return (
    <ul>
      {listBuah.map((item, index) => (
        <li key={index}>{item}</li>
      ))}
    </ul>
  );
}
```
Pada kode di atas:
- listBuah di-_loop_ menggunakan `map()`. 
- `map()` diisi dengan _callback function_ yang mengembalikan element `<li>`
- Atribute/Props `key` pada `<li>` digunakan sebagai pembeda antara `<li>` buah yang satu dengan yang lain
- Maka jeruk, rambutan, dan pepaya akan muncul dengan tampilan list


## Latihan
Untuk mengasah pemahaman mu, silahkan ikuti eksperimen berikut.

1. Tampilkan data array hewan dengan map
1. Jika array kosong tampilkan "Data tidak ada"
1. Bereksperimen lah jika data kosong ataupun ada isinya

Hasilnya seperti ini


# Quiz

### 5 point
Apa yang digunakan sebagai atribut/props untuk membedakan elemen-elemen dalam loop rendering pada JSX?
- [ ] Index
- [x] Key
- [ ] Value
- [ ] Item

### 5 point
Bentuk _conditional_ apa yang digunakan di dalam JSX?
- [ ] if else
- [ ] switch case
- [x] ternary operator
- [ ] map