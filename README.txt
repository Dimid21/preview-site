# Klinik Teduh — Static HTML (Siap Pakai dengan Gambar)

Multi-halaman (index, layanan, jadwal, artikel, lokasi, karir, kontak) + contoh gambar siap pakai di folder `assets/`.
Tahun: 2025

## Cara Menjalankan (lokal)
1) Klik ganda `index.html` (preview cepat), atau
2) Jalankan server lokal dari folder ini:
   - Python: `python -m http.server 5500` → buka http://localhost:5500/index.html
   - Node: `npx http-server . -p 5500`

## Cara Ganti Gambar
- Letakkan gambar Anda di `assets/`, misalnya `assets/hero.jpg`.
- Di file HTML, ganti `src="assets/hero.jpg"` dengan file Anda.
- Untuk rasio tetap + cover:
  ```html
  <div class="aspect-[16/10] rounded-xl overflow-hidden">
    <img src="assets/hero.jpg" alt="Foto Klinik" class="w-full h-full object-cover" />
  </div>
  ```
- Logo rekanan: ganti `<img src="assets/logo-1.png" ...>` dengan logo Anda (PNG transparan atau SVG).

## Struktur
- index.html — Beranda (hero + highlight)
- layanan.html — Layanan & klinik
- jadwal.html — Jadwal dokter (placeholder tabel)
- artikel.html — Kartu artikel (3 contoh)
- lokasi.html — 3 lokasi (tiap lokasi punya gambar, tombol Peta & WA)
- karir.html — Banner + CTA lowongan
- kontak.html — Kontak + Form "Buat Janji"
- assets/ — Gambar contoh (hero, klinik, layanan, 10 logo rekanan)

Selamat mencoba!
