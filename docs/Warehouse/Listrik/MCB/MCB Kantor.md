Diagram
===========================================

- Feeder R,S,T → langsung ke busbar 3 phase

```
┌─────────────────────────────────────────┐
│ HAGER DB – OFFICE + DORM (24 WAY)       │
├─────────────────────────────────────────┤
│ [1] R | FEEDER 3P 20A                   │
│ [2] S | FEEDER 3P 20A                   │
│ [3] T | FEEDER 3P 20A                   │
│-----------------------------------------│
│ [4] R | UPS ONLY            C16         │
│ [5] S | AC Mess #1          C10         │
│ [6] T | AC Mess #2          C10         │
│                                         │
│ [7] R | AC Kantor #1        C10         │
│ [8] S | Lampu               C10         │
│ [9] T | Stop Kontak         C16         │
│                                         │
│ [10]R | AC Kantor #2        C10         │
│ [11+] | --- sisa slot ---               │
└─────────────────────────────────────────┘

```

R ≈ 21.3 A (UPS + 2 AC)

S ≈ 9.0 A

T ≈ 5.5 A


Penjelasan
===========================================

SISTEM:

- 3 Phase: R – S – T – N
- Semua body logam WAJIB ke ground (PE)

ISI MCB PANEL OFFICE + DORM:


0. Feeder 
---------------------
MCB : 3P 25 A

Phase : R - S - T

Beban : 

 - Sumber arus untuk subpael
 - Gunakan bus bar 3 Phase


1. LAMPU OFFICE + DORM
---------------------
MCB   : 1P 10 A

Phase : S

Beban :

- Semua lampu ruangan


2. STOP KONTAK UMUM
------------------
MCB   : 1P 16 A

Phase : T

Beban :

- Laptop
- Printer
- Charger
- Peralatan ringan


3. STOP KONTAK UPS (KHUSUS)
--------------------------
MCB   : 1P 10–16 A

Phase : R

Beban :

- UPS
- Router
- Switch
- DVR CCTV


WAJIB LABEL:

"UPS ONLY – DILARANG PAKAI ALAT LAIN"


4. AC DORM #1
-------------

MCB   : 1P 10–16 A (Curve C)

Phase : S


5. AC DORM #2
-------------

MCB   : 1P 10–16 A (Curve C)

Phase : S


6. AC MAIN OFFICE #1
-------------------

MCB   : 1P 10–16 A (Curve C)

Phase : S


7. AC MAIN OFFICE #2 (JIKA ADA)
------------------------------

MCB   : 1P 10–16 A (Curve C)

Phase : S

ATURAN:

- 1 AC = 1 MCB
- AC TIDAK boleh digabung stop kontak
- Phase TIDAK boleh diganti
- Semua MCB WAJIB ada label

===========================================
