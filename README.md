# Misi Armor Wang: Neo-KL 2099

Kuiz formatif Matematik **Tahun 4 KSSR Semakan 2017, Tajuk 3.0 Wang**. Murid menjawab dengan **isyarat tangan**: angkat tapak tangan menghadap kamera, halakan ke jawapan dan tahan sehingga cas penuh. Tembakan Plasma Tapak Tangan akan mengunci jawapan.

Tugasan: *Design Your Own Money Assessment Challenge* (Topik 5: Reka Bentuk Aktiviti Pengajaran dan Pentaksiran Wang).

---

## 1. Fail dalam folder ini

| Fail | Kegunaan |
|---|---|
| `index.html` | Keseluruhan aplikasi (HTML, CSS dan JavaScript dalam satu fail). |
| `README.md` | Panduan ini. |

Tiada pemasangan, tiada pelayan khas dan tiada kunci API diperlukan.

---

## 2. Tukar nama anda (kredit)

Buka `index.html` dengan Notepad atau VS Code. Cari baris ini (berhampiran permulaan bahagian `<script>`):

```js
const KREDIT = 'Dibina oleh [NAMA GURU PELATIH] | IPG Kampus [NAMA KAMPUS]';
```

Gantikan `[NAMA GURU PELATIH]` dan `[NAMA KAMPUS]`, kemudian simpan. Kredit akan muncul di bahagian bawah skrin, pada laporan misi dan pada cetakan.

---

## 3. Cara menjalankan di komputer sendiri

> **Penting:** Kamera **tidak boleh** digunakan jika anda klik dua kali pada `index.html` (alamat bermula dengan `file://`). Pelayar hanya membenarkan kamera melalui `http://localhost` atau laman `https://`.

### Pilihan A: Python

1. Buka folder ini dalam File Explorer.
2. Klik pada bar alamat folder, taip `powershell`, tekan Enter.
3. Taip arahan ini:

```powershell
python -m http.server 8080
```

4. Buka Google Chrome atau Microsoft Edge, pergi ke **http://localhost:8080**

### Pilihan B: Node.js

```powershell
npx serve -l 8080
```

Kemudian buka **http://localhost:8080**

Untuk berhenti, tekan `Ctrl + C` dalam tetingkap PowerShell.

---

## 4. Cara menerbitkan secara dalam talian (HTTPS)

### Netlify Drop (paling mudah, tanpa akaun GitHub)

1. Pergi ke https://app.netlify.com/drop
2. Seret **folder** `MISI ARMOR WANG` ke dalam kotak di laman itu.
3. Netlify memberi pautan `https://....netlify.app`. Kongsi pautan ini di Google Classroom.

### GitHub Pages

1. Cipta repositori baharu di GitHub (contoh: `misi-armor-wang`), tetapkan sebagai **Public**.
2. Klik **Add file > Upload files**, muat naik `index.html` dan `README.md`, klik **Commit changes**.
3. Pergi ke **Settings > Pages**. Di bawah *Branch*, pilih `main` dan folder `/ (root)`, klik **Save**.
4. Tunggu 1 hingga 2 minit. Pautan anda: `https://NAMA-ANDA.github.io/misi-armor-wang/`

---

## 5. Cara bermain (untuk murid)

1. Taip nama (pilihan), klik **MULAKAN MISI**.
2. Klik **Benarkan** (Allow) apabila pelayar meminta kamera.
3. **Latihan Tembakan:** tembak 3 sasaran (SEDIA, BIDIK, TEMBAK), kemudian cuba **genggam tangan** untuk JEDA.
4. **10 misi wang:** angkat tapak tangan, halakan ke jawapan, tahan kira-kira 1.5 saat.
5. Maklum balas muncul secara automatik. Soalan seterusnya muncul sendiri (tiada butang "Seterusnya").
6. **Laporan Misi:** lihat skor, lencana dan miskonsepsi, kemudian pilih jawapan refleksi.

Pastikan ruang di sekeliling murid selamat semasa menggerakkan tangan.

### Tanpa kamera

| Kaedah | Cara |
|---|---|
| Tetikus | Gerakkan ke jawapan, **tahan butang kiri** sehingga cas penuh. |
| Skrin sentuh | **Tekan dan tahan** pada jawapan. |
| Papan kekunci | Tekan `1` hingga `4` untuk memilih sasaran, **tahan Enter** untuk mengecas. `Space` = jeda / sambung. |

---

## 6. Kekunci pintas guru

| Kekunci | Fungsi |
|---|---|
| `G` | Buka / tutup **Panel Guru** (kunci jawapan, rubrik, senarai semak, tetapan, data sesi) |
| `S` | Langkau latihan tembakan |
| `F` | Paparan nyahpepijat (FPS, masa pengesanan, pose, arah tapak tangan, cas, kualiti, semakan aritmetik) |
| `D` | **Mod Simulasi Tangan**: tetikus menjadi tangan maya (tahan butang kiri = tapak terbuka, butang kanan atau Shift = genggam, `B` = tunjuk belakang tangan) |
| `P` | (semasa `F` hidup) terbalikkan semakan arah tapak tangan |
| `M` | Senyap / bunyi |
| `Esc` | Tutup Panel Guru |

Tambah `?debug` pada hujung alamat (contoh `http://localhost:8080/?debug`) untuk membuka paparan nyahpepijat secara automatik.

---

## 7. Panel Guru

- **Kunci Jawapan:** Standard Pembelajaran, jawapan betul, langkah penyelesaian dan miskonsepsi bagi setiap pengganggu (kod M1 hingga M16 dengan tip pemulihan).
- **Rubrik:** Cemerlang / Baik / Sedang Membangun / Perlu Bimbingan bagi Kefahaman, Aplikasi dan Penaakulan, serta pemetaan item kepada TP.
- **Senarai Semak:** 6 item pemerhatian guru (boleh ditanda di skrin dan dicetak).
- **Tetapan:** masa cas, masa maklum balas, Mod Mudah, rombak pilihan, kelantangan, muzik, suara ARIA, gegaran skrin, Mod Prestasi Rendah, papar FPS. Tetapan disimpan dalam pelayar ini.
- **Data Sesi:** keputusan sesi dalam pelayar ini, analisis item, **Muat Turun CSV** dan **Cetak** (kunci jawapan, rubrik dan senarai semak pada kertas A4 putih).

Data murid hanya disimpan dalam memori pelayar. Data hilang apabila halaman ditutup atau dimuat semula, kecuali anda memuat turun fail CSV.

---

## 8. Ujian ringkas sebelum digunakan di kelas

1. Buka melalui `http://localhost:8080` atau pautan HTTPS.
2. Tekan `F`. Pastikan baris *Semakan aritmetik* menunjukkan **LULUS**.
3. Angkat tapak tangan. Pastikan *Pose* menjadi `OPEN` dan hologram sarung tangan muncul pada tangan anda.
4. Tutup Mod Mudah dalam Panel Guru, kemudian tunjukkan tapak tangan dan belakang tangan. Nilai *Tapak menghadap* sepatutnya positif (YA) untuk tapak tangan dan negatif (TIDAK) untuk belakang tangan. Jika terbalik, tekan `P` (atau biarkan Mod Mudah hidup).
5. Genggam tangan semasa maklum balas. Kiraan detik sepatutnya berhenti (JEDA). Buka tapak tangan untuk sambung.
6. Pastikan FPS sekurang-kurangnya 30. Jika rendah, hidupkan **Mod Prestasi Rendah**.

---

## 9. Masalah biasa

| Masalah | Penyelesaian |
|---|---|
| Skrin "PERLU LOCALHOST ATAU HTTPS" | Anda membuka fail terus (`file://`). Jalankan pelayan tempatan (bahagian 3) atau terbitkan di Netlify / GitHub Pages. |
| "Kebenaran kamera ditolak" | Klik ikon kamera atau mangga di sebelah alamat laman, pilih **Benarkan**, kemudian klik **CUBA LAGI**. |
| "Kamera sedang digunakan" | Tutup Zoom, Google Meet, Teams atau tab lain yang menggunakan kamera, kemudian **CUBA LAGI**. |
| "Kamera tidak dijumpai" | Semak sambungan kamera web atau penutup kamera komputer riba. |
| "Model AI gagal dimuatkan" | Internet diperlukan semasa pembukaan pertama. Pastikan `cdn.jsdelivr.net` dan `storage.googleapis.com` tidak disekat oleh rangkaian sekolah. |
| Tangan tidak dikesan | Pastikan bilik terang, tangan berada 50 cm hingga 1.5 m dari kamera, dan seluruh tapak tangan kelihatan. |
| Tembakan tidak berlaku | Pastikan kelima-lima jari dibuka luas. Hidupkan Mod Mudah. Kurangkan *Masa cas* dalam Tetapan. |
| Penuding bergetar | Pegang tangan lebih stabil, atau dekatkan tangan ke kamera. |
| Permainan perlahan | Hidupkan **Mod Prestasi Rendah**, tutup tab lain, guna Chrome atau Edge terkini. |
| Tiada bunyi | Tekan `M` atau butang BUNYI. Semak kelantangan komputer dan *Kelantangan utama* dalam Tetapan. |
| Suara ARIA tidak boleh dihidupkan | Pelayar tiada suara Bahasa Melayu (ms-MY). Fungsi ini dimatikan secara automatik. |
| Masih tiada kamera | Klik **TERUSKAN DENGAN TETIKUS**. Semua soalan, maklum balas dan laporan tetap berfungsi. |

---

## 10. Privasi

Semua pemprosesan video berlaku dalam pelayar murid. Tiada video dirakam, dimuat naik atau disimpan. Model AI dimuat turun dari CDN awam (jsDelivr dan Google) tetapi imej kamera tidak dihantar ke mana-mana.

## 11. Teknologi

- MediaPipe Tasks Vision `@mediapipe/tasks-vision@1.2.3` (HandLandmarker, mod VIDEO, GPU dengan sandaran CPU)
- Web Audio API (semua bunyi disintesis, tiada fail audio)
- HTML, CSS dan JavaScript biasa. Fon: Orbitron dan Rajdhani (Google Fonts).

Semua nama, watak (ARIA), reka bentuk armor (NEXUS-4), bandar (Neo-KL 2099) dan token wang dalam aplikasi ini adalah ciptaan asal. Token wang adalah rekaan bergaya, bukan gambar wang kertas atau syiling sebenar.
