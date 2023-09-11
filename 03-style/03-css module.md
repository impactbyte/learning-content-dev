Ketika menggunakan _external style_, mungkin kita akan menemukan masalah seperti ini:

```css
/* style.css */
.text {
  color: "blue",
  font-size: "16px",
  background-color: "lightgray",
};
```
```jsx
// Navbar.jsx
import "style.css";

function Navbar() {
  return (
    <div>
      <p className="text">teks dengan external style</p>
    </div>
  );
}
```
```jsx
// Card.jsx
function Card() {
  return (
    <div>
      <span className="text">Card Text</span>
    </div>
  );
}
```
Di atas terdapat 2 komponen yang berbeda. Komponen Navbar diberi style menggunakan external style sedangkan Card tidak memiliki style apapun.

Element `<span>` pada `Card` memiliki `className='text'`. Walaupun `Card` tidak melakukan `import` _style_, akan tetapi secara otomatis _text_ tersebut akan memilki _style_ dari `style.css`. Hal ini disebabkan karena external style bersifat global. 

Jika kamu ingin memberikan style khusus pada suatu komponen dan bersifat tersisolasi. Kita dapat menggunakan cara css module.

**CSS Modules adalah sebuah metode untuk mengatur styling yang memungkinkan kita untuk mengisolasi styles dalam sebuah komponen**. 

Ini bermanfaat untuk menghindari konflik nama kelas (class name) dan memastikan bahwa style hanya berlaku untuk komponen tertentu.

Sehingga 
```css
/* Navbar.css */
.text {
  color: "blue",
  font-size: "16px",
  background-color: "lightgray",
};
```
```jsx
// Navbar.jsx
import styles from './Navbar.css';

function Navbar() {
  return (
    <div>
      <p className={styles.text}>css module</p>
    </div>
  );
}
```

Jika diperhatiakan, kodenya hampir mirip dengan yang sebelumnya. Perbedaan terdapat pada cara `import` dan pada pemberian nama `className`.

import dilakukan dengan memberikan nama `styles`. Kemudian className diisi dengan `styles.text` yang mana `.text` diambil dari styling yang sudah disiaplkan. 

Dengan cara di atas, styling akan terisiolasi dan tidak akan mempengaruhi komponen yang lain dengan `className` yang sama.

# Quiz

Apa manfaat utama dari penggunaan "CSS Modules" dalam React?
- [ ] Meningkatkan konflik nama kelas
- [x] Mengisolasi style sehingga tidak mempengaruhi komponen lain
- [ ] Memungkinkan penggunaan external style secara lebih fleksibel
- [ ] Mengubah gaya penulisan CSS menjadi camelCase