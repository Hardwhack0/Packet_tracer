# 3ITE POS - PCK - Switch

## Popis

Vytvořil jsem LAN síť v Cisco Packet Traceru.
Síť obsahuje 2 switche (S1, S2) a 4 počítače (PC1–PC4).
PC1 a PC2 jsou připojeny k S1. PC3 a PC4 k S2.
Switche S1 a S2 jsou propojeny.

---

## Výpočet X a Y

### Jméno: Viktor

ASCII hodnoty:
V(86) + i(105) + k(107) + t(116) + o(111) + r(114) = 639

Y = 639 % 10 = **9**

### Příjmení: Vlcek

ASCII hodnoty:
V(86) + l(108) + c(99) + e(101) + k(107) = 501

X = 501 % 256 = **245**

---

## IP adresace

Síť:
10.245.0.0 /25

Maska:
255.255.255.128

### Přidělené adresy:

* PC1: 10.245.0.1
* PC2: 10.245.0.2
* PC3: 10.245.0.3
* PC4: 10.245.0.4

---

## Konfigurace switchů

Na obou switchích:

enable
configure terminal
hostname S1 / S2
no ip domain-lookup

---

## Test konektivity

Na PC1 byl proveden ping na PC4:

ping 10.245.0.4

Ping byl úspěšný.

---

## Screenshoty

<img width="457" height="121" alt="image" src="https://github.com/user-attachments/assets/3c3c4b3b-6cca-4622-a4a0-839e8b266d36" />

<img width="634" height="152" alt="image" src="https://github.com/user-attachments/assets/5085bc3f-c8cd-48d7-9c0e-3c4f668e4772" />

<img width="448" height="198" alt="image" src="https://github.com/user-attachments/assets/b6c3186e-b401-4a35-b41c-65c0e6a57db1" />


---
