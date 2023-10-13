Pada topik ini, kita akan mencoba untuk melakukan instalasi project React menggunakan **Vite**. **Vite** adalah alat pengembangan yang cepat dan ringan untuk proyek JavaScript. 

> **NOTE**</br>
> Pastikan kamu sudah mengistall aplikasi NodeJS.

Berikut langkah-langkah untuk menginstall React dengan Vite:

1. Buka terminal atau command prompt.
2. Navigasi ke direktori proyek yang diinginkan.
3. Jalankan perintah berikut untuk membuat proyek baru dengan _template_ Vite:
```bash
npm create vite@latest nama-proyek
```
4. pilih **React** dan **JavaScript** sebagai _library_ dan bahasa yang akan digunakan

5. Masuk ke direktori proyek yang baru saja dibuat:
```bash
cd nama-proyek
``````
6. Install _dependencies_ dengan menjalankan perintah:
```bash
npm install
```
7. Lalu jalankan aplikasi React dengan perintah:
```bash
npm run dev
```
Maka akan muncul tampilan website React.
![]()

**Selamat!!! aplikasi react pertama kalian sudah berhasil dijalankan..**

Kita juga bisa membuka proyek React yang sudah di-install dengan menggunakan code editor. Kurang lebih seperti ini lah struktur proyek React yang di install menggunakan Vite.

```
my-react-project/
├── node_modules/
├── public/
│   └── vite.svg
├── src/
│   ├── assets/
│   ├── App.jsx
│   ├── main.jsx
│   └── style.css
├── .gitignore
├── index.html
├── package.json
├── README.md
└── vite.config.js
```

Wow terlihat menyeramkan ya karena ada banyak file asing yang mungkin belum kita kenal. Tapi jangan khawatir, kita hanya fokus pada direktori `src/`.

Berikut adalah penjelasan singkat dari struktur proyek di atas:
- **node_modules/**: Berisi semua paket yang di-instal oleh NPM.
- **public/**: Berisi file yang akan disalin ke root direktori output saat proyek di-_build_. `index.html` adalah file utama yang akan digunakan oleh Vite.
- **src/**: Berisi kode sumber proyek.
`App.jsx` adalah komponen utama React yang akan di-render dalam `main.jsx`.
- **.gitignore**: Berisi daftar file/direktori yang akan diabaikan oleh Git. 
- **package.json**: File konfigurasi proyek dan daftar dependensi.
- **README.md**: Berisi informasi/penjelasan tentang proyek yang kita buat.
- **vite.config.js**: Berisi konfigurasi Vite.

# Quiz

### 5 point
Manakah perintah yang benar
- [ ] npm create vite-latest 
- [ ] npm build vite@latest nama-proyek
- [ ] npm create vite@latest nama-proyek
- [ ] npm create vite@latest nama-proyek

### 5 point
Jika Anda ingin menjalankan aplikasi React, perintah apa yang harus dijalankan?

- [ ] npm start
- [ ] npm run build
- [ ] npm run serve
- [x] npm run dev

### 10 point
Mengapa penggunaan NodeJS disebutkan dalam pembelajaran ini?

- [ ] NodeJS adalah alat pengembangan yang berbasis JavaScript.
- [x] NodeJS digunakan untuk menjalankan perintah-perintah dalam proses instalasi proyek React.
- [ ] NodeJS digunakan untuk mengelola tampilan website React.
- [ ] NodeJS digunakan untuk membuat server