Diagram
===========================================

- Feeder R,S,T → langsung ke busbar 3 phase
- Exhaust fan ambil dari busbar (bukan looping MCB)

```
┌─────────────────────────────────────────┐
│ HAGER DB – GUDANG (18 WAY)              │
├─────────────────────────────────────────┤
│ [1] R | FEEDER 3P 25A                   │
│ [2] S | FEEDER 3P 25A                   │
│ [3] T | FEEDER 3P 25A                   │
│-----------------------------------------│
│ [4] R | HVLS                  C10       │
│ [5] S | Stop Kontak / Tools   C20       │
│ [6] T | Lampu UFO             C10       │
│                                         │
│ [7] R |                                 │
│ [8] S |                                 │
│ [9] T |                                 │
│                                         │
│ [10+] | --- sisa slot ---               │
└─────────────────────────────────────────┘
```

R ≈ 4.5 A   (exhaust share)

S ≈ 18–22 A (tools + charger + exhaust)

T ≈ 7.8 A (lampu UFO + exhaust)



Penjelasan
===========================================

SISTEM:

- 3 Phase: R – S – T – N
- Semua body logam WAJIB ke ground (PE)

ISI MCB PANEL GUDANG:

0. Feeder 
---------------------
MCB : 3P 20 A

Phase : R - S - T

Beban : 

 - Sumber arus untuk subpael
 - Gunakan bus bar 3 Phase

1. LAMPU GUDANG (UFO)
--------------------
MCB   : 1P 10 A

Phase : R

Beban :

- Lampu UFO 150 W (±12 unit)

2. STOP KONTAK GUDANG
--------------------
MCB   : 1P 16 A

Phase : S

Beban :

- Colokan umum gudang
- Alat maintenance ringan

3. EXHAUST FAN GUDANG (3 PHASE)
-------------------------------
MCB   : 3P 10 A

Phase : R + S + T

Beban :

- 2 unit exhaust fan
- 550 W / unit
- Motor 3 phase

ATURAN:

- Exhaust TIDAK boleh digabung beban lain
- Phase TIDAK boleh diganti
- Semua MCB WAJIB ada label
