# Uang Berdua: cara menerbitkan

Isi folder ini:

| Berkas | Fungsi |
|---|---|
| `index.html` | Aplikasinya |
| `config.js` | Konfigurasi Firebase (sudah diisi, sama dengan Jadwal Berdua) |
| `sw.js` | Supaya halaman tetap terbuka saat offline |
| `firestore.rules` | Aturan keamanan (sama dengan Jadwal Berdua, tidak perlu diunggah) |

## A. Firebase: tidak ada yang perlu dikerjakan

Aplikasi ini memakai proyek Firebase yang sama dengan Jadwal Berdua (`jadwal-for-oktober`). Firestore, Anonymous sign-in, dan Rules-nya sudah aktif, dan Rules yang lama sudah mencakup data uang.

Kalau suatu saat ingin proyek Firebase terpisah, ikuti Bagian A di PANDUAN Jadwal Berdua lalu ganti isi `config.js`.

## B. Hosting di GitHub Pages

1. Buka https://github.com/new dan buat repository **Public** (misal `uang-berdua`).
2. Klik **uploading an existing file**, seret `index.html`, `config.js`, dan `sw.js`, lalu **Commit changes**.
3. Buka **Settings > Pages**. Pada **Branch** pilih `main` dan `/ (root)`, klik **Save**.
4. Tunggu 1-2 menit. Alamatnya: `https://NAMA-AKUN.github.io/uang-berdua/`

## C. Mulai dipakai

1. Buka alamat itu. Di perangkat yang sudah pernah membuka Jadwal Berdua akan muncul tombol **Pakai ruang Jadwal Berdua**: tekan itu, maka ruang, profil, dan nama kalian langsung ikut. Kalau tidak muncul, tekan **Buat ruang baru** lalu pilih **Profil 1**.
2. Buka **Atur**, isi nama dan anggaran bulananmu, lalu **Salin** tautan ruang.
3. Kirim tautan itu ke pacarmu (dan ke HP-mu sendiri). Dia memilih **Profil 2**.
4. Di HP: menu browser > **Tambahkan ke layar utama**.

## Cara mencatat

- Tekan **+ Catat**, isi jumlah dan kategori. Selesai.
- **Untuk siapa** menentukan hitungan di antara kalian:
  - *Untuk yang bayar sendiri*: pengeluaran pribadi, tidak memengaruhi saldo berdua.
  - *Berdua, dibagi dua*: masing-masing menanggung setengah; yang tidak membayar jadi berutang setengahnya.
  - *Untuk pasangannya (ditalangi)*: seluruhnya jadi utang pasangan.
- Halaman **Berdua** menunjukkan siapa perlu membayar siapa. Setelah transfer, tekan **Catat pelunasan** supaya saldonya kembali impas.
- Ketuk transaksi mana pun untuk mengubah atau menghapusnya. Kalian berdua bisa mengubah semua transaksi.

## Tabungan dan investasi

- Di halaman **Tabungan**, tekan **Buat tujuan baru**: beri nama, pilih jenis (tabungan, dana darurat, reksa dana, saham, emas, deposito/SBN, kripto), pemiliknya (kamu, pasangan, atau berdua), lalu target dan tenggat kalau ada.
- **Setor** dan **Tarik** mencatat uang yang masuk dan keluar dari tujuan itu. Setoran muncul sebagai "Ditabung" di Ringkasan dan mengurangi "Sisa" bulan itu, tetapi tidak dihitung sebagai pengeluaran atau anggaran.
- Untuk jenis investasi, tekan **Perbarui nilai** dan isi nilai totalnya saat ini (dari aplikasi sekuritas atau bank). Aplikasi lalu menampilkan untung atau ruginya terhadap modal yang disetor. Nilai ini diisi manual, tidak mengambil harga pasar otomatis.
- Untuk tujuan berdua, terlihat berapa setoran masing-masing.

## Foto profil dan latar

- **Atur > Profilmu > Pilih foto**: tiap orang mengunggah fotonya sendiri dari perangkatnya. Kalau belum diunggah dan ruangnya sama dengan Jadwal Berdua, foto dari sana yang dipakai.
- **Atur > Latar halaman**: pilih salah satu latar bawaan atau **Unggah foto latar**. Latar berlaku untuk kalian berdua dan langsung berganti di semua perangkat.
- Foto diperkecil otomatis sebelum disimpan (profil 160 px, latar maksimal 1280 px).

## Hal yang perlu diketahui

- **Tautan ruang adalah kuncinya.** Siapa pun yang punya tautan itu bisa membaca dan mengubah catatan uang kalian.
- **Kalian saling melihat semuanya**, termasuk pengeluaran pribadi masing-masing.
- **Kuota Firebase dipakai bersama Jadwal Berdua.** Untuk pemakaian berdua, batas gratisnya jauh dari tercapai.
- **Ringkasan memuat 13 bulan terakhir.** Transaksi bersama dan pelunasan dimuat seluruhnya, jadi saldo utang tetap utuh. **Unduh CSV** di halaman Atur mengekspor data yang termuat itu.
- **Offline:** catatan saat offline tersimpan di perangkat dan terkirim otomatis begitu tersambung lagi.
- **Mengubah aplikasi:** unggah ulang berkas yang berubah ke repository. Data di Firebase tidak terpengaruh.
