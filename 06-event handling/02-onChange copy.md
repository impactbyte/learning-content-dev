`onChange` adalah prop yang umum digunakan pada elemen seperti `<input>`, `<textarea>` dan `<select>`. Ini memungkinkan kita menangani perubahan nilai pada elemen tersebut. Contohnya:

```jsx
function InputExample() {
  function handleInputChange(event) {
    console.log('Nilai baru: ', event.target.value);
  }

  return <input type="text" onChange={handleInputChange} />;
}```