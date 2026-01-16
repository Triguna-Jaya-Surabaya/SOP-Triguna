DATA DASAR SISTEM
===========================================

- Sumber listrik: PLN 3 Phase
- Daya: 16.500 VA
- Arus maksimum: ±25 A per phase
- Urutan phase: R – S – T – N
- Sistem proteksi: MCB (tanpa RCD / ELCB)

Kabel feeder utama ke sub panel masing-masing area:

- 3 Phase + Netral (RST-N): NYYHY - Eterna 6 mm² (warna hitam)
- Ground / PE: NYAF - 4 mm² (kuning-hijau)

Kabel setelah sub panel:

- 1 Phase + Netral + Ground  NYMHY 2.5 mm² (warna putih)




WARNA KABEL 
===========================================
- 3 PHASE:
	- R (L1) : Biru
	- S (L2) : Merah
	- T (L3) : Kuning polos
	- N      : Hitam
	- PE     : Kuning–Hijau
- URUTAN PHASE:
	- KIRI → KANAN : R – S – T


- 1 PHASE:
	- L      : Biru
	- N      : Coklat
	- PE     : Kuning–Hijau
- Patokan Internal (Biar sama aja):
	- L  → Pin kanan
	- N  → Pin kiri




ATURAN MUTLAK (SEMUA AREA)
=========================
- Pakai sarung tangan, sepatu
- Setiap area menerima: R + S + T + N + PE
- Kabel 2.5 mm² → MCB MAX 16 A
- Exhaust 3 phase → MCB 3P
- Semua MCB WAJIB diberi label
- 1 beban besar = 1 MCB (AC MCB sendiri, Exhaust Fan MCB Sendiri, dst)
- Phase TIDAK BOLEH diganti di lapangan, Selalu berurutan 
	- Phase dirancang untuk dibuat seimbang
- Semua body logam WAJIB terhubung ke ground (PE)
- Dibagi 3 sub-panel
	- [[MCB Gudang]]
	- [[MCB Kantor]]
	- [[MCB Picker Packer]]



DATA BEBAN 2025-01-03
===========================================

```
Feeder:
- Office : 20A ✔
- Gudang : 25A ✔
- Picker : 25A ✔ (borderline tapi aman)

Gudang
R ≈ 4.5 A   (HVLS)
S ≈ 18–22 A (tools + charger + exhaust)
T ≈ 7.8 A (lampu UFO + exhaust)

Kantor
R ≈ 21.3 A (UPS + 2 AC 1 PK)
S ≈ 9.0 A (AC Mess + Lampu)
T ≈ 5.5 A (AC Mess + Stop Kontak)

Picker Packer
R ≈ 7.8 A
S ≈ 1.0 A
T ≈ 7.8 A


PHASE R ≈ 33 A (est berlebih di UPS)
PHASE S ≈ 30 A (est berlebih di Charger Stacker)
PHASE T ≈ 22 A
```

Kalau MCB turun, pindah AC kantor 1 PK ke T satu

PANEL UTAMA (INCOMING PLN)
===========================================
1. Pasang MCB utama:
   - MCB 3 Phase: 25 A

2. Dari panel utama, buat feeder ke tiap area:
   - Phase + Netral: 6 mm²
   - PE: 4 mm²


ATURAN PEMBAGIAN PHASE
------------------------
- Beban besar harus dibagi merata antar phase
- Gunakan pola:
	R → S → T → ulangi

Jika suatu phase sering trip:

- Berarti beban pada phase tersebut terlalu besar
- Pindahkan SATU beban besar (AC), bukan seluruh sirkuit.


KONFIGURASI YANG DILARANG
---------------------------
❌ Kabel 2.5 mm² pada MCB >16 A

❌ Lebih dari 1 Air Conditioner dalam 1 MCB

❌ Air Conditioner digabung dengan stop kontak

❌ Ground tidak terhubung ke body peralatan

❌ Phase tidak diberi label

❌ MCB dipilih berdasarkan “kira-kira”


