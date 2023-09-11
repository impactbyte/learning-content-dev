
Pada topik sebelumnya kita sudah belajar tentang bagaimana caranya menyimpan data dinamis menggunakan _state_. 

**Lalu bagaimana caranya membuat state?**

Di sini kita membutuhkan `useState` yang berasal dari `react`.

```jsx
// di luar komponen
import { useState } from "react"

// di dalam komponen
const [state, setState] = useState("value")
```

`useState` akan mengembalikan data dalam bentuk _array_, sehingga ketika dideklarasi bisa kita tulis dengan cara _destructure_ seperti ini  `[state, setState]`. Dari hasil _destructure_ kita mendapatkan `state` yang bernilai data yang ingin disimpan, dan `setState` adalah function untuk mengubah data tersebut.

Contoh:

```jsx
import { useState } from "react"

function Profile () {
  const [name, setName] = useState("Terra")

  return (
    <div>
      <img />
      <h2>{name}</h2>
    <div>
  )
}
```

Pada kode di atas, kita membuat state `name` yang bernilai `"Terra"`. Kemudian `name` ditampilkan pada tag `<h2>`.

Lalu gimana cara mengubah _state_-nya? 

Untuk mengubah state, kita perlu 
```
setState(newValue)
```
Contoh:
```jsx
setName("Alpha")
```
Mengubah state akan kita pelajari kembali pada **lesson Event Handling**


# Quiz

Bagaimana cara mengimpor useState dalam sebuah komponen React?
- [ ] import useState from "react"
- [x] import { useState } from "react"
- [ ] import useState from "react-state"
- [ ] import { useState } from "react-dom"