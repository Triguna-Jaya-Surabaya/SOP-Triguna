UPS Maintenance (MULTIMETER)
=================================================

Jenis UPS      : Online UPS (contoh: Prolink PRO901-ES)
Jenis Baterai  : VRLA / SLA 12V
Frekuensi      : 1x per tahun (12 bulan sekali)

-------------------------------------------------
1. TUJUAN
-------------------------------------------------
- Mendeteksi baterai UPS yang mulai lemah atau rusak
- Mencegah UPS mati mendadak saat listrik padam
- Menentukan apakah baterai masih layak atau harus diganti

-------------------------------------------------
2. PERALATAN
-------------------------------------------------
- Multimeter digital
- Obeng (berinsulasi)
- Kacamata safety (disarankan)
- Sarung tangan (opsional)
- Buku catatan / HP untuk dokumentasi

-------------------------------------------------
3. KESELAMATAN (WAJIB)
-------------------------------------------------
- JANGAN menghubungkan (+) dan (–) baterai (short)
- JANGAN mencampur baterai lama dan baru
- JANGAN melakukan pengukuran saat UPS sedang charge
- Anggap baterai sebagai sumber listrik DC aktif

-------------------------------------------------
4. PERSIAPAN
-------------------------------------------------
1. Pastikan UPS di-charge penuh
   - Sambungkan ke listrik PLN
   - Biarkan minimal 8 jam
2. Matikan beban (server / PC / alat)
3. Matikan UPS
4. Cabut input listrik PLN
5. Tunggu 5–10 menit (agar tegangan stabil)

-------------------------------------------------
5. AKSES BATERAI
-------------------------------------------------
1. Buka cover baterai UPS
2. Identifikasi baterai:
   - Biasanya 2 x 12V VRLA (tersusun seri)
3. Jangan lepas kabel kecuali diperlukan

-------------------------------------------------
6. PROSEDUR PENGUKURAN
-------------------------------------------------

6.1 Setting Multimeter
- Mode      : DC Voltage (V⎓)
- Range     : 20V atau Auto

6.2 Pengukuran Baterai
Lakukan untuk SETIAP baterai 12V:

1. Probe merah  → terminal (+)
2. Probe hitam  → terminal (–)
3. Catat tegangan

-------------------------------------------------
7. INTERPRETASI HASIL
-------------------------------------------------

Tegangan Baterai (kondisi diam):

≥ 12.6 V
- Kondisi : Sehat
- Tindakan: Tidak perlu ganti

12.3 – 12.5 V
- Kondisi : Mulai menua
- Tindakan: Monitor, rencanakan penggantian

12.0 – 12.2 V
- Kondisi : Lemah
- Tindakan: GANTI SET BATERAI

< 12.0 V
- Kondisi : Rusak
- Tindakan: GANTI SEGERA

Catatan Penting:
- Jika selisih antar baterai > 0.3 V → WAJIB GANTI SEMUA
- Jika satu baterai rusak → ganti SATU SET, bukan satuan

-------------------------------------------------
8. TES BEBAN RINGAN (OPSIONAL, DISARANKAN)
-------------------------------------------------
1. Pasang kembali cover baterai
2. Nyalakan UPS
3. Hubungkan beban ringan (10–20%)
4. Cabut listrik PLN
5. Amati:
   - Tidak langsung mati
   - Tidak alarm baterai lemah
   - Runtime masuk akal

Jika runtime < 50% normal → baterai dianggap FAIL

-------------------------------------------------
9. DOKUMENTASI
-------------------------------------------------
Catat:
- Tanggal pengecekan
- Model UPS
- Lokasi UPS
- Tegangan tiap baterai
- Status (OK / Monitor / Ganti)
- Nama teknisi

-------------------------------------------------
10. KEBIJAKAN PENGGANTIAN
-------------------------------------------------
Baterai WAJIB diganti jika:
- Tegangan < 12.2 V
- Selisih antar baterai > 0.3 V
- Runtime < 50%
- Umur baterai ≥ 3 tahun

-------------------------------------------------
11. PEMBUANGAN BATERAI
-------------------------------------------------
- Serahkan ke penjual baterai / recycler resmi
- DILARANG buang ke sampah umum
