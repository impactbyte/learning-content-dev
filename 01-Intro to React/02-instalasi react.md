Pada topik ini, kita akan mencoba untuk melakukan instalasi project React menggunakan **Vite**.
**Vite** adalah alat pengembangan yang cepat dan ringan untuk proyek JavaScript. Berikut langkah-langkah untuk menginstall React dengan Vite:

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
- **public/**: Berisi file yang akan disalin ke root direktori output saat proyek Anda dibangun. `index.html` adalah file utama yang akan digunakan oleh Vite.
- **src/**: Berisi kode sumber proyek Anda.
App.jsx: Ini adalah komponen utama React yang akan di-render dalam index.jsx.
- **.gitignore**: Berisi daftar file/direktori yang akan diabaikan oleh Git. 
- **package.json**: File konfigurasi proyek dan daftar dependensi.
- **README.md**: Berisi informasi/penjelasan tentang proyek yang kita buat.
- **vite.config.js**: Berisi konfigurasi Vite.

# Quiz

### 5 Point
Langkah mana yang benar saat ingin membuat proyek baru dengan template Vite?
- [ ] Menjalankan perintah `npm init` dalam terminal.
- [ ] Menjalankan perintah `npm create react-app nama-proyek`.
- [x] Menjalankan perintah `npm create vite@latest nama-proyek`.
- [ ] Menjalankan perintah `create-vite-app nama-proyek`.

### 10 Point
Jika Anda ingin menjalankan aplikasi React setelah melakukan instalasi menggunakan Vite, perintah apa yang harus dijalankan?

- [ ] npm start
- [ ] npm run build
- [ ] npm run serve
- [x] npm run dev