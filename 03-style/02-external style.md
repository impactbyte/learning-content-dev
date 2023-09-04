Tidak hanya _**inline style**_ yang dapat kita gunakan, tapi _**external style**_ juga bisa kita gunakan pada React. Contohnya seperti ini:

```jsx
// App.jsx
import "style.css";

function App() {
  return (
    <div>
      <p className="text">Ini adalah teks dengan inline style.</p>
    </div>
  );
}
```

```css
/* style.css */
.text {
  color: "blue",
  font-size: "16px",
  background-color: "lightgray",
};
```
Penggunaannya mirip seperti saat kita menggunakan HTML dan CSS secara terpisah.

Pertama kita siapkan file css-nya. Lalu pada file _component_, kita `import` _file styling_. Berikutnya tinggal bermain dengan __selector__ _(tag, id, class)_ sesuai dengan kebutuhan. 

Jika ingin menggunakan _selector class_, gunakan `className`. Ini disebabkan karena JavaScript sudah memiliki _key word_ `class`, maka dari itu di JSX kita menggantinya dengan `className`.

> **NOTE**</br>
> Jika memberikan _**external style**_ pada _parent component_, maka _child component_ dapat menggunakan _style_ tersebut tanpa perlu di `import`.