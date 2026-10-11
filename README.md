# Kalkulator Pajak PPh & PPN (PWA - Progressive Web App)

Aplikasi web mobile & desktop untuk menghitung **PPh 23, PPh 21, PPh 4 ayat (2)**, dan **PPN dengan DPP Nilai Lain / Besaran Tertentu** lengkap dengan opsi **Gross-Up**, status **NPWP**, dan pilihan **Include/Exclude PPN**.

## Fitur Utama
1. **Multi-Pajak Lengkap:**
   - **PPh 23:** Jasa Badan/Umum (2% ber-NPWP, 4% tanpa NPWP).
   - **PPh 21:** Tenaga Ahli / Bukan Pegawai (DPP 50% × Tarif Lapisan 5%, 15%, 25%).
   - **PPh 4 ayat (2):** Jasa Konstruksi (1.75%, 2.65%, 4%, 3.5%, 6%) & Sewa Tanah/Bangunan (10%).
   - **PPN (DPP Nilai Lain & Standar):**
     - **Jasa Pengiriman Paket / Ekspedisi:** DPP 10% → Tarif Efektif 1,1% (PMK 71/PMK.03/2022).
     - **Biro Perjalanan Wisata / Agen Tur:** DPP 10% → Tarif Efektif 1,1% (PMK 71/PMK.03/2022).
     - **Freight Forwarding / Pengurusan Transportasi:** DPP 10% → Tarif Efektif 1,1% (PMK 71/PMK.03/2022).
     - **Penjualan Kendaraan Bermotor Bekas:** DPP 10% → Tarif Efektif 1,1% (PMK 65/PMK.03/2022).
     - **Penjualan Emas Perhiasan:** Pabrikan (1,1%) & Pedagang (1,65%) (PMK 48/2023).
     - **Pemakaian Sendiri / Pemberian Cuma-cuma:** DPP = HPP / Biaya Pokok (PMK 121/2015).
     - **Penyerahan Antar Cabang / Pusat-Cabang:** DPP = Harga Pokok Penjualan.
     - **DPP Nilai Lain Kustom:** Persentase DPP fleksibel (bebas diatur sesuai kebutuhan kontrak).
     - **PPN Standar:** DPP Penuh 100% (Kode Transaksi 010).
2. **Skema Fleksibel Transaksi:**
   - *PPh:* Opsi Gross-Up (pajak ditanggung) vs Non Gross-Up (potong dari vendor).
   - *PPN:* Opsi Exclude PPN (harga belum pajak) vs Include PPN (harga sudah termasuk pajak).
   - *Pilihan Tarif PPN:* 11% (berlaku saat ini) dan 12% (UU HPP).
   - *Panduan e-Faktur:* Menampilkan rekomendasi Kode Transaksi Faktur Pajak (Kode 040 untuk DPP Nilai Lain).
3. **Format Rupiah Otomatis:** Tombol instan (+1 Jt, +5 Jt, +10 Jt, Reset).
4. **Fitur Salin Ringkasan:** 1-klik untuk menyalin format memo rapi siap kirim ke WhatsApp / email.
5. **Penyimpanan Riwayat:** 10 perhitungan terakhir tersimpan otomatis di perangkat (`localStorage`).
6. **Mobile App / PWA:**
   - Dapat dipasang (*Add to Home Screen*) di Android & iPhone.
   - Berfungsi 100% secara offline tanpa kuota internet.

---

## Cara Mencoba di Laptop Sekarang

Cukup buka file `index.html` langsung di browser Anda (Google Chrome / Safari / Edge).

Atau jalankan server lokal sederhana dengan terminal:
```bash
cd /Users/herryoe/.gemini/antigravity/scratch/kalkulator-pph-pwa
python3 -m http.server 8080
```
Lalu buka `http://localhost:8080` di browser.

---

## Cara Membagikan ke Tim Secara 100% GRATIS

Agar seluruh anggota tim bisa membuka dari HP masing-masing tanpa biaya langganan:

### Opsi A: Menggunakan GitHub Pages (Gratis Selamanya)
1. Buat repository baru di [github.com](https://github.com) (misal: `kalkulator-pph`).
2. Upload semua file dalam folder ini (`index.html`, `manifest.json`, `sw.js`, `icon.svg`).
3. Buka menu **Settings** > **Pages** > pada Source pilih branch `main` lalu **Save**.
4. Dalam 1 menit, GitHub akan memberikan link website gratis (contoh: `https://username.github.io/kalkulator-pph/`).
5. Bagikan link tersebut ke grup WhatsApp tim!

### Opsi B: Menggunakan Netlify Drop (Tanpa Koding / Akun)
1. Buka [app.netlify.com/drop](https://app.netlify.com/drop).
2. Tarik (*drag & drop*) folder `kalkulator-pph-pwa` ke halaman tersebut.
3. Netlify langsung memberikan link aktif dalam hitungan detik.

---

## Cara Pasang di HP (Bagi Pengguna)

1. Buka link aplikasi di browser HP.
2. **Android (Chrome):** Tekan tombol titik tiga di kanan atas > pilih **"Tambahkan ke Layar Utama" (Add to Home Screen)** atau klik tombol **"+ Pasang App"**.
3. **iPhone (Safari):** Tekan tombol Share (ikon kotak panah ke atas) > pilih **"Add to Home Screen"**.
4. Ikon aplikasi akan muncul di beranda HP dan siap digunakan kapan saja!
