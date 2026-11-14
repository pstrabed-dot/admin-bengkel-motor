# Admin Bengkel Motor

Aplikasi pencatatan bengkel motor kecil — dibuat sesederhana mungkin untuk pemilik
bengkel yang tidak terlalu paham teknologi. Semua memakai Bahasa Indonesia,
tombol besar, dan nyaman dibuka dari HP.

## Fitur

- **Beranda "Pekerjaan Hari Ini"** — hitungan Menunggu / Dikerjakan / Belum Lunas,
  dan pencarian berdasarkan plat nomor, nama pelanggan, atau nomor HP.
- **Pelanggan & Kendaraan** — nama dan nomor HP pelanggan; tiap pelanggan bisa
  punya lebih dari satu motor (plat nomor, merk/tipe, tahun).
- **Pencatatan servis** — keluhan, pekerjaan yang dilakukan, sparepart,
  biaya sparepart + biaya jasa (total terhitung otomatis), KM, dan catatan
  servis berikutnya.
- **Status sekali ketuk** — Menunggu → Dikerjakan → Selesai → Diambil.
  Tanggal selesai terisi otomatis saat status menjadi Selesai.
- **Lunas / Belum Lunas** — daftar piutang dan rekap uang masuk per bulan
  di menu Riwayat.
- **Nota servis** — tampil rapi dengan rincian biaya dan stempel LUNAS bila
  sudah lunas. Bisa dikirim ke pelanggan via WhatsApp atau disalin sebagai teks.
- **Ubah dan hapus** — pelanggan, kendaraan, dan servis bisa diubah dan
  dihapus (hapus selalu minta konfirmasi dulu).

## Cara pakai

1. Buka `index.html` di browser (HP atau laptop).
2. Menu **Pelanggan** → tambah pelanggan, lalu tambah motornya.
3. Menu **Beranda** → ketuk **＋ Servis Baru**, pilih kendaraan, isi keluhan
   dan biaya, simpan.
4. Ketuk tombol status untuk memajukan pekerjaan, dan **Tandai Lunas**
   setelah pelanggan membayar.
5. Ketuk **🧾 Nota** untuk melihat nota, mengirimnya via WhatsApp, atau
   menyalin teksnya.

## Cara mempublikasikan lewat GitHub Pages

1. Push folder ini ke repositori GitHub (misalnya `admin-bengkel-motor`).
2. Di GitHub, buka **Settings → Pages**.
3. Pada **Build and deployment → Source**, pilih **Deploy from a branch**.
4. Pilih branch **main** dan folder **/(root)**, lalu **Save**.
5. Tunggu sebentar — aplikasi bisa dibuka di
   `https://<username>.github.io/admin-bengkel-motor/`.

## Catatan penting soal data

- Semua data (pelanggan, kendaraan, servis) tersimpan di **localStorage
  browser** masing-masing perangkat. Artinya:
  - Data tidak hilang saat aplikasi ditutup atau browser dimatikan.
  - Data **tidak ikut pindah** kalau dibuka di HP/laptop lain atau browser
    lain — tiap perangkat punya catatannya sendiri.
  - Jangan hapus data browser (clear site data) untuk situs ini, karena
    catatan bengkel ikut terhapus.
- Aplikasi mulai kosong, tanpa data contoh. Isi dengan data bengkel sendiri.
- File ini mandiri: satu file `index.html` saja sudah cukup untuk menjalankan
  aplikasi. Font memakai Google Fonts bila ada internet, dan otomatis memakai
  font sistem bila offline.
