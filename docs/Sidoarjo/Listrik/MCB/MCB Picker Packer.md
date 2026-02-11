Diagram
===========================================

- Feeder R,S,T → langsung ke busbar 3 phase

```
┌─────────────────────────────────────────┐
│ HAGER DB – PICKER PACKER (18 WAY)       │
├─────────────────────────────────────────┤
│ [1] R | FEEDER 3P 25A                   │
│ [2] S | FEEDER 3P 25A                   │
│ [3] T | FEEDER 3P 25A                   │
│-----------------------------------------│
│ [4] R | AC 2 PK #2          C20         │
│ [5] S | Lampu               C10         │
│ [6] T | AC 2 PK #1          C20         │
│                                         │
│ [7] R | --- cadangan ---    C6          │
│ [8] S | Colokan             C10         │
│ [9+]  | --- sisa slot ---               │
└─────────────────────────────────────────┘


```

R ≈ 7.8 A

S ≈ 1.0 A

T ≈ 7.8 A



Penjelasan
===========================================

SISTEM:

- 3 Phase: R – S – T – N
- Semua body logam WAJIB ke ground (PE)

ISI MCB PANEL PICKER–PACKER:


0. Feeder 
---------------------
MCB : 3P 20 A

Phase : R - S - T

Beban : 

 - Sumber arus untuk subpael
 - Gunakan bus bar 3 Phase


1. LAMPU AREA KERJA
------------------

MCB   : 1P 10 A

Phase : R

Beban :

- Lampu area picker–packer


2. STOP KONTAK RINGAN
--------------------
MCB   : 1P 16 A

Phase : T

Beban :

- Charger HP
- Laptop
- Printer
- Alat kecil


3. AC PICKER–PACKER #1
----------------------

MCB   : 1P 20 A (Curve C)

Phase : R

Beban :

- AC 2 PK


4. AC PICKER–PACKER #2
----------------------
MCB   : 1P 20 A (Curve C)

Phase : R

Beban :

- AC 2 PK


ATURAN:

- 1 AC = 1 MCB
- AC TIDAK boleh digabung stop kontak
- Phase TIDAK boleh diganti

===========================================
