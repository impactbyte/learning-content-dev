Membuat komponen menggunakan bentuk `function` (__functional component__) merupakan cara yang paling umum digunakan saat ini. 

Pembuatan yang cukup mudah, penulisan yang simple dan memiliki fitur _hooks_ (akan dibahas pada kelas React Lanjutan)

```jsx
// App.jsx
import Footer from './components/Footer';

function App() {
  return (
    <div>
      <h1>Halo Semua!</h1>
      <p>Selamat Datang di aplikasi React Pertamaku</p>

      <Footer />
    </div>
  );
}

export default App;
```

```jsx
// /components/Footer.jsx
function Footer() {
  return (
    <footer>
      <p>By Terra</p>
    </footer>
  );
}

export default Footer;
```

Perhatikan kode di atas, komponen `App` berperan sebagai _parent component_, sedangkan komponen `Footer` sebagai _child component_.

> **NOTE**</br>
> Nama component pada React disarankan untuk menggunakan `TitleCase`.

Selain itu, ada juga pembuatan komponen menggunakan `class` (_class component_). **Cara ini sudah ditinggalkan**, tapi mungkin saja kamu akan menemuinya pada kode React yang sudah lawas. Berikut contoh sintax **class component**
```jsx
class App extends React.Component {
  render() {
    return (
      <h1>Halo Semua!</h1>
      <p>Selamat Datang di aplikasi React Pertamaku</p>
    );
  }
}
```