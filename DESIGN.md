# DESIGN.md — Villa Frengky (demo pitch oleh Lamanara)

Status: PLANNING (belum dibangun). Demo gratis untuk prospek WhatsApp, dijanjikan "beberapa hari ke depan" (chat 13 Nov 2026).

---

## 0. Brief

| | |
|---|---|
| Bisnis | Villa Frengky: satu rumah minimalis (tipe 36) disewakan harian di Perumahan Fiorence Hills, Temas, Kota Batu |
| Data dari owner (chat) | 2 kamar tidur + 1 extra bed, muat 6 orang. Weekday Rp500 ribu, weekend Rp650 ribu per malam. Fasilitas: WiFi, air panas, dapur, TV, kulkas, BBQ, parkir mobil. Lokasi: "cari Villa Frengky di Google Maps" |
| Data publik (cek dulu ke owner) | Google Maps: 4,5 (16 ulasan), pin −7.8862, 112.5353. OTA (Traveloka, dll.) menulis alamat Perumahan Fiorence Hills Regency B-17, Jl. Dewi Sartika Gg. 3H; jarak ke Jatim Park 2 ±0,7 km, Jatim Park 1 ±1 km, BNS ±1,4 km, Museum Angkut ±1,8 km; check-in 14.00, check-out 12.00/13.00; tidak boleh hewan |
| Tamu | Keluarga kecil dari Surabaya/Jatim yang mau liburan hemat ke Jatim Park & BNS, bawa mobil, mau masak sendiri |
| Satu aksi utama | Cek tanggal → chat WhatsApp owner dengan pesan yang sudah terisi (tanggal, malam, jumlah tamu, total) |
| Trust drivers | Foto rumah yang asli, harga jelas weekday/weekend, dekat Jatim Park, rating Google asli, WA yang dibalas, dapur & air panas, parkir mobil |
| Adjektif | bersih, praktis, dekat · anti: "resort mewah" |
| Aset | 7 foto asli (depan ×2, ruang keluarga ×2, dapur, kamar, taman belakang). Tidak ada logo, tidak ada IG, tidak ada foto kamar mandi/area BBQ |

**Paket yang cocok:** Landing Page (Rp1,2 jt). Hanya satu unit, jadi halaman per kamar di Company Profile tidak perlu.

---

## 1. Papan referensi (dilihat langsung, 13 Nov 2026)

| Referensi | Yang diambil |
|---|---|
| [Google Maps: Villa Frengky](https://www.google.com/maps/place/Villa+Frengky/@-7.8862358,112.5352731,17z) | Fakta & ulasan asli: bersih, dapur lengkap, air panas, dekat Jatim Park. Ada juga keluhan "kecil" dan "masuk gang sempit", jadi ekspektasi harus dijujurkan di web |
| [Forest Villa Batu](https://www.forestvillabatu.com/) | Pola pasar Batu: search bar (tanggal, lokasi, orang), harga weekday/weekend ditulis dua baris, tombol selalu ke WA. Kelemahan: Inter 700 di mana-mana, emoji jadi ikon, kartu seragam |
| [villabatumalang.com](https://villabatumalang.com/villa-perdana-batu/) | Pola agregator SEO: judul berisi kapasitas + kamar. Kelemahan: blok teks panjang, foto tanpa tata letak |
| [Pusat Villa](https://www.pusatvilla.com/2024/01/villa-perdana-11-rooms-and-private-pool.html) | Halaman listing satu villa: foto besar + thumbnail, harga /malam, tombol Booking WA, fakta ikon (kamar, kamar mandi, lantai), tabel fasilitas "Yes" (jangan ditiru) |
| [Airbnb listing Batu](https://www.airbnb.com/rooms/1752871) | Standar komponen: grid foto 1+4 + "Lihat semua foto", baris fakta "15 tamu · 5 kamar · 6 kasur · 4 kamar mandi", kartu booking sticky (check-in / checkout / tamu) |
| [Booking.com listing Batu](https://www.booking.com/hotel/id/batu-villa-3-bed-rooms-amp-just-2-min-walk-to-jatim-park-1.html) | Tab anchor (Ringkasan, Harga, Fasilitas, Aturan, Ulasan), "lokasi sangat bagus – lihat peta" di dekat judul, skor ulasan di samping foto |
| [Omah Lereng (karya Lamanara)](https://omah-lereng.vercel.app/) | Dipakai sebagai pembanding supaya demo ini tidak terlihat seperti template yang sama (hijau + Bricolage + Plus Jakarta) |

Catatan jujur: hanya 2 referensi best-in-class yang dilihat (Airbnb, Booking.com) karena Mobbin sedang tidak tersambung. Bagian craft cukup memakai keduanya.

**Konvensi yang dipertahankan:** foto dulu, fakta kapasitas, harga weekday/weekend, daftar fasilitas, jarak ke Jatim Park/BNS, aturan check-in, tombol WA di mana-mana.
**Batas kualitas:** listing OTA memberi grid foto rapi, fakta satu baris, kotak booking yang menghitung total.
**Celah:** situs villa lokal tidak menghitung total harga, foto acak, emoji sebagai ikon, tidak jujur soal ukuran rumah atau akses. Villa Frengky bisa unggul dengan cara jujur, cepat, dan langsung menghitung total.

---

## 2. Taste

| Situs | Ground | Ink | Aksen/tombol | Display | Text | Radius | Foto |
|---|---|---|---|---|---|---|---|
| Forest Villa Batu | #fbfaf5 / #fff | #18231c | #2f6b46 hijau | Inter 700, 84px | Inter | 0 / pill | sunset, kolam, cerah |
| villabatumalang | #fff | abu gelap | emas/coklat | sans tengah | Roboto-ish | kecil | kolam, flash |
| Pusat Villa | #fff | abu | oranye | sans 600 | sans | 16–pill | eksterior, watermark |
| Airbnb | #fff | #222 | rose | Cereal 500 | Cereal | 12 | foto host, apa adanya |
| Booking.com | #fff | #1a1a1a | biru/kuning | sans 700 | sans | 4–8 | foto host |
| Omah Lereng | #fff | #1b1f1d | hijau tua | Bricolage 500 | Plus Jakarta | 8–pill | stok, dramatis |

- **Pasar sepakat pada** latar putih, satu warna aksen, banyak foto, tombol WhatsApp.
- **Yang terbaik** punya grid foto rapi, fakta satu baris, kotak booking dengan total.
- **Kompetitor terlalu sering memakai** hijau tua + krem ("villa alam") dan emoji. Villa Frengky adalah rumah perumahan modern putih-arang, jadi palet diambil dari rumahnya, bukan dari hutan.

### Palet (dari rumah aslinya)
| Token | Hex | Peran | Porsi | Asal |
|---|---|---|---|---|
| ground | #FFFFFF | latar | 60% | dinding putih |
| band | #F4F2EE | satu band (harga/lokasi), latar sheet | 15% | lantai granit |
| ink | #22272B | teks, header | 15% | kanopi baja arang |
| muted | #5F6670 | teks sekunder | — | list abu fasad |
| accent | #9A5636 | tombol utama, link, tanggal terpilih | 10% | batu alam di kolom + bata taman |

Kontras: ink/putih 15,1 · muted/putih 5,8 · muted/band 5,2 · putih di atas aksen 5,6 · aksen/band 5,0. Semua ≥ 4,5. Ikon WhatsApp tetap memakai warna aslinya (glyph putih di dalam tombol aksen, logo hijau resmi di bar mobile).

### Tipografi
- Kandidat display: **Familjen Grotesk**, Schibsted Grotesk, Hanken Grotesk. Kandidat teks: **Figtree**, Instrument Sans, Onest.
- **Pilihan: Familjen Grotesk 500 (display) + Figtree 400/600 (teks).** Grotesk bergaya papan nama terasa ramah dan "rumah", tidak "resort", dan berbeda dari Omah Lereng. Bobot 500 mengikuti Airbnb (bukan 700 seperti Forest Villa).
- Skala 1,25: 14 · 16 · 18 · 22 · 28 · 36 · 48 · 60 (maksimal 8 ukuran). Body 17px, leading judul 1,05–1,1, tracking −0,01em.
- Uji di layar 390px: "Rumah liburan keluarga di Temas, Kota Batu" maksimal 2 baris pada 36px.
- Muat 2 family, maksimal 4 file (Google Fonts, display=swap).

### Arah foto
Pakai **hanya 7 foto asli** sebagai satu set. Tidak ada stok, sesuai pelajaran dari Omah Lereng. Cahaya siang yang netral. Rapikan dulu: potong bar hitam WhatsApp, luruskan garis vertikal, naikkan exposure sedikit, samakan white balance. Foto WhatsApp sekitar 720px, jadi **jangan dipasang full-bleed 1440**. Hero dibuat split atau grid 1+4. Minta owner mengirim file asli "sebagai dokumen" agar resolusinya penuh.

### Dial
DESIGN_VARIANCE 4 · MOTION_INTENSITY 3 · VISUAL_DENSITY 5. Radius 10px (kartu/sheet), 8px (tombol), pill hanya untuk chip tanggal. Shadow hanya pada sheet booking.

---

## 3. Struktur halaman (satu halaman, urutan pertanyaan tamu)

1. **Header**: wordmark teks "Villa Frengky", anchor (Foto · Fasilitas · Harga · Lokasi · Tanya jawab), tombol "Cek tanggal".
2. **Hero (split 7/5)**: kiri judul + fakta + bar booking, kanan foto depan (yang ada mobil di carport).
   - h1: *Rumah liburan keluarga di Temas, Kota Batu*
   - Kalimat fakta: *2 kamar tidur + 1 extra bed, muat 6 orang. Dapur, air panas, carport. Mulai Rp500.000 per malam.*
   - Bar tersegmentasi: Check-in – Check-out | Tamu | **Cek & booking via WhatsApp**
   - Di bawahnya satu baris: ★ 4,5 di Google Maps (16 ulasan), link ke Maps.
3. **Grid foto 1+4** + tombol "Lihat 7 foto" (lightbox layar penuh, swipe, Esc). Di bawahnya baris fakta: *6 tamu · 2 kamar tidur · 1 extra bed · carport 1 mobil*.
4. **Isi rumah** (2–3 baris split foto/teks, suara owner, tanpa caption):
   - Ruang keluarga berplafon tinggi, sofa, TV
   - Dapur yang bisa dipakai masak (kompor, kulkas)
   - Taman belakang berumput untuk BBQ malam
5. **Fasilitas**: satu daftar ikon Lucide (WiFi, Air panas, Dapur, TV, Kulkas, Alat BBQ, Parkir mobil). Tanpa kartu, tanpa "Yes".
6. **Harga & booking (momen andalan)**: kalender rentang tanggal dengan harga per malam di bawah tiap tanggal (500rb / 650rb, weekend diberi tanda). Stepper tamu maksimal 6. Rincian: weekday × n + weekend × n = total. Tombol sticky "Kirim ke WhatsApp" dengan pesan terisi. Muncul sebagai drawer di desktop dan bottom sheet di HP.
7. **Lokasi**: embed peta pin + satu kalimat jarak (Jatim Park 2, Jatim Park 1, BNS, Museum Angkut). Satu kalimat jujur soal akses: *masuk gang perumahan, mobil bisa sampai carport* (konfirmasi ke owner).
8. **Ulasan**: skor Google + 2 kutipan pendek asli (setelah owner setuju), link "Baca 16 ulasan di Google".
9. **Aturan menginap**: strip ringkas: check-in 14.00, check-out 12.00, tidak boleh hewan, DP via transfer. Semua ditandai data-assumed sampai owner konfirmasi.
10. **Tanya jawab** (satu kolom, accordion): ada AC? (Batu sejuk, tanya owner) · extra bed bayar? · bisa lebih dari 6 orang? · parkir berapa mobil? · dekat masjid/minimarket?
11. **Footer**: baris booking + WA, alamat (perumahan + Temas), link Maps, "Contoh tampilan oleh Lamanara · foto milik Villa Frengky".
- **Bar mobile sticky**: "Rp500rb/malam · Cek tanggal" + ikon WA. Selalu terlihat.

Pesan WA terisi (contoh):
`Halo Kak, saya mau booking Villa Frengky tgl 20–22 Desember 2026 (2 malam), 5 orang. Estimasi Rp1.150.000. Masih kosong?`

---

## 4. Larangan khusus proyek ini
- Tidak memakai tampilan "resort mewah" (krem + serif tipis + hijau tua). Ini rumah Rp500 ribu untuk keluarga.
- Tidak ada foto stok, ikon gambar tangan, atau emoji ikon.
- Harga, jam, dan aturan tidak dibuat sebagai baris hairline judul tebal + deskripsi abu. Harga ditampilkan di dalam kalender dan satu kalimat.
- Tidak ada langkah "01/02/03 cara booking".
- Tidak ada detail karangan (luas m², merek kasur, "air hangat 24 jam"). Hanya yang dikatakan owner atau yang ada di Maps, dan yang belum pasti diberi data-assumed.
- Tidak ada ulasan karangan. Kutipan Google hanya dipakai setelah owner OK.
- Ambil semua pelajaran dari /topics/lessons-design.md (Omah Lereng, Lentur).

## 5. Teknis
Astro + Tailwind, ikon Lucide inline, kalender buatan sendiri (bukan input date native), deploy ke `villa-frengky.vercel.app` dengan `noindex` selama masih demo. Target: hero < 250 KB, foto lain < 150 KB (WebP).
Motion: hero masuk sekali, sheet booking 300ms `--ease-drawer`, tombol scale 0.97 saat ditekan, hormati reduced-motion.
