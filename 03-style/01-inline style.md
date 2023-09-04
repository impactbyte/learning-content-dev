_Styling_ merupakan hal yang **tidak bisa dipisahkan** dari _web development_. Dengan memberikan styling, tampilan website menjadi lebih indah.

Sama seperti penggunaan _styling_ pada HTML, kita juga bisa memberikan _styling_ dalam bentuk _**inline style**_ pada React.

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

_Key_ pada objek _style_ yang memiliki lebih dari satu kata,  ditulis dengan gaya penulisan **_camelCase_** contohnya seperti `fontSize`, dan `backgroundColor`. Kenapa **_camelCase_**?? Berhubung kita menulisnya di dalam JSX yang merupakan JavaScript, maka kita harus mengikuti kaidah penulisan pada bahasa tersebut.
