# Návrh počítačového vybavení malé školy

**Autor:** Martin Chejn  
**Třída:** 4C

---

## 1. Zadání
Proveďte návrh počítačového vybavení malé školy s 2 počítačovými učebnami po 8 PC.  
V těchto učebnách se bude vyučovat AutoCAD a Inventor. V každé třídě bude navíc učitelské pracoviště s projektorem a síťovou laserovou tiskárnou. Ve škole bude dále fileserver a pracoviště správce. Do školy vede telefonní linka technicky způsobilá pro VDSL.

---

## 2. Vybavení

### 2.1 IT třídy
- **PC sestava:** HelloComp Intel GAMER Pro 4060 Ti  
  - CPU: Intel Core i7-12700F  
  - GPU: NVIDIA 4060 Ti (8 GB GDDR6 VRAM)  
- **Počet:** 9 strojů na třídu (8 pro žáky, 1 pro učitele)  
- **Monitory:** 27" Dell P2725HE Professional  
- **Periferie:** bezdrátová klávesnice a myš  
- **Projektor (učitel):** Epson EB-992F  
- **Tiskárna (učebna):** HP Color Laser 178nw All-in-One  

### 2.2 Zbytek školy
- **PC sestava:** Dell Optiplex 7020 SFF  
  - CPU: Intel Core i3-14100  
  - Úložiště: SSD  
- **Počet:**  
  - 10 strojů v běžných třídách  
  - 5 strojů v kabinetech  
  - 2 pro vedení školy  
- **Interaktivní tabule:** Samsung LH86WADWLGCXEN (10 ks)  
- **Periferie:** jako v IT učebnách  
- **Tiskárny:** HP Color Laser 178nw (v kabinetu i vedení)  

---

## 3. Síťová infrastruktura a server
- **Připojení:** VDSL (50 Mbps základ, až 300 Mbps s bonding/vectoring)  
- **Router:** MikroTik Cloud Core CCR2116-12G-4S+  
- **Switche:** MikroTik Cloud Smart CSS326-24G-2S+RM (2 ks)  
- **Kabeláž:** CAT6 UTP  
- **Podsítě:**  
  - IT učebny: 192.168.1.0/24  
  - Ostatní: 192.168.2.0/24  
- **Server:** Dell PowerEdge R360  
  - RAM: upgrade na 128 GB ECC  
  - Disky: 7× WD Gold 6 TB (RAID)  

---

## 4. Sítové služby
- Fileserver  
- WSUS (Windows Update Services)  
- Kerberos (autentizace)  
- DHCP (statická IP pro většinu, DHCP pro WiFi)  
- DNS  

---

## 5. Software
- **CAD:** AutoCAD, Inventor (Autodesk Education zdarma)  
- **OS (PC):** Windows 11 Education (600 CZK/rok/licence)  
- **Office:** Office 365 A3 (630 CZK/rok/uživatel, ~150 uživatelů)  
- **Server OS:** Windows Server Standard (26 000 CZK jednorázově)  

---

## 6. Cena a seznam vybavení

### Infrastruktura
| Zařízení                                        | Cena (CZK) | Ks. | Celkem (CZK) |
|-------------------------------------------------|------------|-----|--------------|
| Dell PowerEdge R360                             | 55 472     | 1   | 55 472       |
| WD Gold 6 TB                                    | 5 929      | 7   | 41 503       |
| MikroTik CCR2116-12G-4S+                        | 17 932     | 1   | 17 932       |
| MikroTik CSS326-24G-2S+RM                       | 2 918      | 2   | 5 836        |
| Ubiquiti POE-48-24W-G                           | 321        | 4   | 1 284        |
| Ubiquiti UniFi AP U6+                           | 3 050      | 4   | 12 200       |
| Datacom drát CAT6 UTP (305 m)                   | 2 751      | 1   | 2 751        |
| **Celkem infrastruktura**                       |            |     | **136 978**  |

### Učebny a zázemí
| Zařízení                                        | Cena (CZK) | Ks. | Celkem (CZK)   |
|-------------------------------------------------|------------|-----|----------------|
| Samsung LH86WADWLGCXEN                          | 42 316     | 10  | 423 160        |
| Epson EB-992F                                   | 18 174     | 2   | 36 348         |
| Dell Optiplex 7020 SFF                          | 21 749     | 17  | 369 733        |
| HelloComp Intel GAMER Pro 4060 Ti               | 30 157     | 18  | 542 826        |
| Dell KM555 (CZ/SK)                              | 1 321      | 40  | 52 840         |
| 27" Dell P2725HE Professional                   | 4 793      | 35  | 167 755        |
| HP Color Laser 178nw All-in-One printer         | 6 445      | 4   | 25 780         |
| **Celkem učebny a zázemí**                     |            |     | **1 618 442**  |

**Celkem (bez licencí):** 1 755 420 CZK  
**Licence:** 26 000 CZK jednorázově + 115 500 CZK/rok  
**Grand Total:** 1 781 420 CZK  

---

## 7. Odkazy
- Dell PowerEdge R360: https://www.suntech.cz/dell-server-poweredge-r360_d669941.html  
- WD Gold 6 TB: https://www.westerndigital.com/...  
- MikroTik CCR2116-12G-4S+: https://www.suntech.cz/mikrotik-cloud-core-router-ccr2116-12g-4s-_d583795.html  
- MikroTik CSS326-24G-2S+RM: https://www.suntech.cz/...  
- Ubiquiti POE-48-24W-G: https://www.alza.cz/...  
- Ubiquiti UniFi AP U6+: https://www.alza.cz/...  
- Samsung LH86WADWLGCXEN: https://www.senetic.cz/...  
- Epson EB-992F: https://www.alza.cz/...  
- HelloComp Intel GAMER Pro 4060 Ti: https://www.hellocomp.cz/...  
- Dell Optiplex 7020 SFF: https://www.alza.cz/...  
- HP Color Laser 178nw: https://www.alza.cz/...  

---
