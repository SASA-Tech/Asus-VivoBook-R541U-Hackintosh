# Asus-VivoBook-R541U-Hackintosh
[![](https://img.shields.io/badge/Gitter%20HL%20Community-Chat-informational?style=flat&logo=gitter&logoColor=white&color=ed1965)](https://gitter.im/Hackintosh-Life-IT/community)
[![](https://img.shields.io/badge/Repository-SASATech-informational?style=flat&logo=apple&logoColor=white&color=9debeb)](https://github.com/SASA-Tech?tab=repositories)
[![](https://img.shields.io/badge/Telegram-HackintoshLifeIT-informational?style=flat&logo=telegram&logoColor=white&color=5fb659)](https://t.me/HackintoshLife_it)
[![](https://img.shields.io/badge/Facebook-HackintoshLifeIT-informational?style=flat&logo=facebook&logoColor=white&color=3a4dc9)](https://www.facebook.com/hackintoshlife/)
[![](https://img.shields.io/badge/Instagram-HackintoshLifeIT-informational?style=flat&logo=instagram&logoColor=white&color=8a178a)](https://www.instagram.com/hackintoshlife.it_official/)

## macOS Big Sur/Monterey correttamente installato su ASUS Vivobook R541U

# Specifiche:

| Componenti       | Modello                               |
| ---------------- | --------------------------------------|
| Notebook         | ASUS Vivobook R541U                   |
| CPU              | Intel Core i3 6600U                   | 
| iGPU             | Intel® HD Graphics 520                |
| Audio            | Realtek ALC256                        |
| LAN              | Realtek RTL810xE                      |
| RAM              | 8 GB DDR4 2133 Mhz (indicati da macOS |
| SSD              | Samsung 860 Evo 500gb                 |
| SMBIOS           | MacBookPro13,1                        |
| Bootloader       | OpenCore 0.7.3                        |

![infodp1](./Screenshot/Mobo.png)

## NOTE:
Vi lascio la EFI con SSDT, non avrebbe senso lasciarvi quella con DSDT patchato perché non funzionerebbe sul vostro PC.
Pertanto l'unica cosa che non funzionerà sarà la combo dei tasti FN (FN+F1, FN+F2 ecc.)
In post installazione scrivete nel gruppo HackintoshLife che vi lascio in fondo la pagina per estrarre e patchare il vostro DSDT.
Kexts aggiornati alle ultime versioni.

## Se volete installare la Beta 7 di macOS Monterey:
Vi lascio il config.plist rinominato in configbeta7.plist pronto da utilizzare SOLO per scaricare ed installare l'aggiornamento.
Al termine dell'aggiornamento dovete cancellarlo e rimettere l'originale config.plist.
È consigliabile scollegare l'Hackintosh dall'ID Apple prima di sostituire momentaneamente il config.plist

# Impostazioni Bios

## Disabilita:

- Fast Boot
- VT-d
- CSM
- Intel SGX
- Intel Platform Trust
- CFG Lock (MSR 0xE2 write protection)

## Abilita:

- Intel Virtualizzation Technology
- Above 4G decoding
- Hyper-Threading
- Execute Disable Bit
- EHCI/XHCI Hand-off
- OS type: (Windows 10 Feautres: Windows 8/10 WHQL oppure Other)
- DVMT Pre-Allocated(iGPU Memory): 64 MB
- DVMT Total Gfx Mem → MAX

## Impostazioni generiche, potresti non trovarne alcune.
  
# Dispositivo Screenshot
![infodp1](./Screenshot/Peripherials.png)
![infodp2](./Screenshot/PCIe.png)

# Cosa funziona e cosa no:
- [x] Intel® HD Graphics 520 iGPU
- [x] Realtek ALC256 uscite interne
- [x] Realtek ALC256 HDMI Audio Output
- [x] Porte USB (Funzionano ma richiedono mappatura)
- [x] Realtek RTL810xE
- [x] NVRAM
- [x] Avvio Windows da OpenCore
- [ ] NVIDIA® GeForce® 920MX
- [ ] Lettore Scheda SD (potrebbe funzionare)
- [ ] WiFi + Bluetooth (si può sostituire la scheda con una compatibile)

# Sezione Info SSDT ASUS Vivobook R541U

![SSDT](./Screenshot/SSDT.png)

## Crediti

- [Acidanthera](https://github.com/acidanthera) per OpenCore Bootloader
- [Apple](https://apple.com) per macOS;
- [HackintoshLifeIT](https://github.com/Hackintoshlifeit) Gruppo di supporto pre e post installazione
- [Dortania](https://github.com/dortania) per le guide OpenCore

# Se avete bisogno di aiuto contattateci su [Telegram](https://t.me/HackintoshLife_it)
