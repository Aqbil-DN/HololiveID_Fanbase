# Hololive ID Fanbase Web

## 📌 Deskripsi Proyek (Tentang Web Ini)
Proyek ini adalah sebuah website statis yang didedikasikan sebagai **Fanbase Hololive Indonesia**. Website ini dirancang untuk menampilkan berbagai informasi seputar talent Hololive ID (Mulai dari Generasi 1 hingga Generasi 3), pencapaian, video klip, ilustrasi fan art, hingga halaman komunitas bagi para penggemar.

Website ini awalnya dibuat sebagai Tugas Besar oleh **Kelompok 1** yang beranggotakan:
- Aqbil
- Roger
- Filbert
- Habil

## 💻 Teknologi yang Digunakan
Website ini dibangun murni menggunakan teknologi *front-end* tanpa *framework* yang berat, sehingga sangat ringan dan mudah dimodifikasi:
- **HTML5:** Untuk struktur dasar halaman web.
- **CSS3:** Untuk *styling*, *layout*, dan responsivitas web.
- **JavaScript (Vanilla & jQuery):** Untuk interaksi halaman dan DOM manipulation.
- **Slick Carousel:** Library pihak ketiga untuk membuat *slider* atau *carousel* interaktif (foto/video).
- **Font Awesome:** Digunakan untuk menampilkan ikon-ikon pada website.

## 📂 Struktur Folder dan File
Struktur repositori pada proyek ini disusun sebagai berikut:

- `index.html` & `*.html` lainnya: File utama HTML yang mencakup halaman utama (`index.html`), halaman tentang talent (`talent.html`, `airaniIofifteen.html`, dll), pendaftaran (`join.html`), fan art (`fanart.html`), dan `about.html`.
- `*.css`: File CSS spesifik yang terhubung dengan setiap halaman HTML individu.
- `CSS/`: Folder berisi CSS global seperti `navigation-bar.css`, `footer.css`, dan typography (`font-worksans.css`).
- `JS/`: Folder berisi file JavaScript *custom* (contohnya `home.js`).
- `Assets/`: Folder sentral untuk menyimpan aset multimedia, termasuk:
  - Gambar/Ilustrasi/Thumbnail
  - Video klip
  - Audio latar (BGM)
  - Logo Sosial Media
- `Fonts/`: Folder untuk menyimpan *font* lokal.
- `Slick/`: Folder bawaan *library* Slick Carousel beserta aset *styling*-nya.

## 🚀 Cara Setup dan Menjalankan Web
Karena ini adalah *static website*, kamu **tidak memerlukan instalasi dependensi (seperti `npm install`) atau konfigurasi *backend* yang rumit**.

### Cara 1: Buka Langsung (Direct Open)
Ini adalah cara yang paling cepat dan sederhana:
1. *Clone* repositori ini ke komputer lokal kamu:
   ```bash
   git clone https://github.com/Aqbil-DN/HololiveID_Fanbase.git
   ```
2. Buka folder hasil *clone* tersebut.
3. Cari file bernama `index.html` lalu klik ganda (double-click) untuk membukanya langsung di *browser* (Chrome, Firefox, Edge, dll).

### Cara 2: Menggunakan Local Server (Sangat Direkomendasikan)
Menjalankan menggunakan Local Server lebih disarankan untuk mencegah terjadinya masalah `CORS` pada saat browser mencoba membaca *file asset* seperti video atau audio.

**Opsi A: Menggunakan ekstensi Live Server (Visual Studio Code)**
1. Buka folder repositori proyek ini menggunakan **Visual Studio Code (VSCode)**.
2. Pastikan kamu sudah menginstal *extension* bernama **Live Server** di VSCode.
3. Buka file `index.html`.
4. Klik kanan di dalam *code editor* dan pilih **"Open with Live Server"** (atau klik tombol **Go Live** di pojok kanan bawah VSCode). Website akan otomatis terbuka di *browser*.

**Opsi B: Menggunakan Node.js**
1. Buka *terminal* (Command Prompt/PowerShell) dan arahkan ke folder proyek.
2. Pastikan kamu telah menginstal [Node.js](https://nodejs.org/).
3. Jalankan perintah berikut:
   ```bash
   npx http-server
   ```
   atau
   ```bash
   npx serve
   ```
4. Buka alamat `http://localhost:8080` atau alamat yang tertera pada *terminal* di *browser* kamu.

**Opsi C: Menggunakan Python**
1. Buka *terminal* dan arahkan ke folder proyek.
2. Jika komputer kamu memiliki Python terinstal, jalankan perintah berikut:
   ```bash
   python -m http.server 8000
   ```
3. Buka `http://localhost:8000` di *browser*.
