Dalam membuat halaman website, sudah pasti kita akan mengamati, menganalisa, membagi dan menentukan bagian-bagian serta element dari design yang sudah disiapkan.

Perhatikan design berikut
![gambar]()

Berdasarkan design di atas, ternyata terdiri dari beberapa bagian atau **_component_**
![gambar]()

_**Component**_ pada React adalah **bagian-bagian dari halaman website**. Seperti `Navbar`, `Footer`, `Button`, dan sebagainya. Kita  bebas menentukan seberapa besar atau kecil komponen yang akan dibuat sesuai dengan kebutuhan.

Dengan memisahkan _pages_ menjadi beberapa _component_, dapat memberikan keuntungan seperti:
- _Component_ dapat digunakan berkali-kali
- Kode menjadi lebih mudah dibaca dan dikelola
- Lebih mudah melacak bug

Dari kode yang awalnya menumpuk seperti ini:

```html
<div>
  <!-- Navbar -->
  <header>
    <nav>
      <ul>
        <li><li>
        <li><li>
        <li><li>
      </ul>
    </nav>
  </header>

  <!-- Hero section -->
  <main>
    <section>
    </section>

    <section>
    </section>
  </main>
</div>
```
Menjadi seperti ini

```html
<div>
  <Navbar />
  <Hero />
</div>
```

Wow!!! menarik bukan?

Selanjutnya kita akan belajar bagaimana caranya membuat komponen pada React