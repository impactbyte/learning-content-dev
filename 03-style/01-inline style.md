Pemberian styling dengan cara **_inline_** merupakan salah satu yang cukup mudah dilakukan ketika digunakan pada HTML. 

**_inline style_** dapat diterapkan pada React, tapi ada beberapa hal yang harus diperhatikan.

Pertama yang perlu disiapkan adalah _prop_ `style`. _Prop_ ini berisi objek JavaScript dengan _key_ dan _value_ _styling_ yang akan kita berikan. Contoh:

```jsx
function App() {
  const styles = {
    color: "blue",
    fontSize: "16px",
    backgroundColor: "lightgray",
  };

  return (
    <div>
      <p style={styles}>Ini adalah teks dengan inline style.</p>
    </div>
  );
}
```

Atau juga bisa seperti ini:

```jsx
function App() {
  return (
    <div>
      <p
        style={{
          color: "blue",
          fontSize: "16px",
          backgroundColor: "lightgray",
        }}
      >
        Ini adalah teks dengan inline style.
      </p>
    </div>
  );
}
```

_Key_ pada objek _style_ yang memiliki lebih dari satu kata, ditulis dengan gaya penulisan **_camelCase_** contohnya seperti `fontSize`, dan `backgroundColor`. Kenapa **_camelCase_**?? Berhubung kita menulisnya di dalam JSX yang merupakan JavaScript, maka kita harus mengikuti kaidah penulisan pada bahasa tersebut.

# Quiz

### 5 point

Apa yang perlu diperhatikan ketika menulis properti pada objek style?

- [ ] Menggunakan properti yang memiliki lebih dari satu kata dengan kebab-case
- [x] Menggunakan properti yang memiliki lebih dari satu kata dengan camelCase
- [ ] Menggunakan properti yang hanya terdiri dari satu kata
- [ ] Tidak perlu memperhatikan properti ketika menggunakan style

### 10 point

Apa yang salah dari kode di bawah
```jsx
<span
  style={{
    padding: 16px,
    fontSize: 1.3rem,
    backgroundColor: lightgray,
  }}
>
  Kirim
</span>
```

- [ ] Tidak menggunakan CapitalCase
- [ ] Tidak menggunakan class
- [ ] Tidak menggunakan css terpisah
- [x] Tidak menggunakan kutip pada value
