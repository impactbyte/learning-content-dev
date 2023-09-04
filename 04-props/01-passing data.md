

**Props** adalah singkatan dari _Properties_. **Props** berguna untuk **mengoper data** dari _parent component_ ke _child component_. Bersifat satu arah (_parent_ ke _child_) dan dapat menjadikan komponen  lebih dinamis.

Supaya lebih jelas, coba kamu perhatikan kode dan gambar di bawah ini. 

![gambar]()

Misalnya kamu ingin menampilkan `Card` dengan data yang berbeda. Mungkin cara yang terpikirkan saat ini adalah dengan membuat komponen `Card1`, `Card2`, `Card3` dan seterusnya sebanyak yang kamu butuhkan. Lalu gimana kalau datanya ada 100 atau mungkin 1000??

Dari pada kamu membuat 1000 `Card` yang berbeda, kamu hanya butuh 1 component `Card` yang dapat menerima data. Sehingga menjadi seperti ini:

```jsx
// App.jsx
function App(){
  return (
    <>
      <Card img="spongebob.png" name="Spongebob" />
      <Card img="patrick.png" name="Patrick" />
      <Card img="squidward.png" name="Squidward" />
    </>
  )
}

// Card.jsx
function Card(props) {
  return (
    <div>
      <img src={props.img} />
      <h2>{props.name}</h2>
    </div>
  );
}
```

Pada kode di atas, kita panggil `Card`, lalu berikan _props_ `img` dan `name`. Di dalam komponen `Card`, tambahkan parameter `props` untuk dapat menangkap data _props_ yang sudah dioper.

Tidak hanya data `string` yang dapat kamu kirim, tapi kamu dapat mengirim data `number`, `boolean`, `array`, `object` dan bahkan sebuah component. Contoh:

```jsx

// App.jsx
// mengoper object sebagai props
function App(){
  return (
    <>
      <Card character={{name: "Spongebob", img: "spongebob.jpg"}} />
    </>
  )
}

// Card.jsx
function Card(props) {
  return (
    <div>
      <img src={props.character.img} />
      <h2>{props.character.name}</h2>
    </div>
  );
}
```


> **Note**</br>
> Cara kerja props mirip seperti memberikan argument pada function, yang nantinya akan diterima sebagai parameter
