Membuat komponen menggunakan bentuk `function` (__functional component__) merupakan cara yang paling umum digunakan saat ini. 

Pembuatan yang cukup mudah, penulisan yang simple dan memiliki fitur _hooks_. 

Berikut skema dasar pembuatan _functional component_:
```jsx
function NamaKomponen() {
  return (
    <div>
      {/* isi konten */}
    </div>
  );
}

export default NamaKomponen;
```
Dari skema di atas, komponen diberi format penulisan `TitleCase`, dan di dalamnya me-_return_ sebuah JSX element.

Berikut contoh penggunaannya:


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

# Quiz

### 5 Point
Apa yang paling umum digunakan saat ini dalam pembuatan komponen di React?
- [x] Functional Component
- [ ] Class Component
- [ ] Static Component
- [ ] Dynamic Component

### 15 Point
```jsx
function Navbar() {
  return (
    <div>
      <img src="logo.png" />
    </div>
    
    <ul>
      <li>Home</li>
      <li>About</li>
      <li>Contact</li>
    </ul>
  );
}

export default Navbar;
```
Apa yang salah dari kode di atas?
- [ ] di dalam return ada HTML
- [ ] function belum di panggil
- [ ] list tidak mengarah pada halaman manapun
- [x] return lebih dari satu element