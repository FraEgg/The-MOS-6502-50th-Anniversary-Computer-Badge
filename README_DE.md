# The MOS 6502 – 50th Anniversary Computer Badge (1975–2025)

## Ein Retro‑Computer im Badge‑Format für 8‑Bit‑6502‑Fans

Von Frank Eggen

👉 **[English Version](README.md)**

[![Schau dir das Video auf YouTube an](images/Youtube.jpg "YouTube: MOS 6502 – 50th Anniversary Computer Badge")](https://youtu.be/MOvFbZeAMVU)

---

Basierend auf einer Idee von **Lee Hart, Daryl Rictor und Josh Bensadon** (neu aufgelegt und aktualisiert).  
👉 Originalprojekt: <http://www.sunrise-ev.com/6502.htm>

---

## 50 Jahre 8‑Bit‑Mikroprozessor MOS 6502

<img src="images/white-ceramic-6502-illustration.png" title="White Ceramic 6502 CPU Illustration" alt="Illustration einer weißen 6502‑CPU" width="600" />

Der legendäre **MOS 6502** wurde 1975 vorgestellt und veränderte die Welt der Computer.  
Er brachte Leistung zum kleinen Preis und machte den Siegeszug der **Homecomputer** möglich.

Bekannte Systeme mit 6502:

- Apple II
- Commodore VIC‑20 & C64
- Nintendo NES
- BBC Micro
- Atari VCS

👉 Mehr zur Geschichte: <https://www.team6502.org>

---

### Was ist das „Computer Badge“?

<img title="The MOS 6502 – 50th Anniversary Computer Badge (1975–2025)" src="images/The_MOS_6502–50th_Anniversary_Computer_Badge_Real.jpg" alt="The MOS 6502 – 50th Anniversary Computer Badge (1975–2025)" data-align="center" style="zoom:25%;">

Der **MOS 6502 50th Anniversary Computer Badge** ist eine **minimalistische Neuauflage** des Originals – kompatibel, aber mit modernen Bauteilen leicht nachzubauen.

**Highlights:**

- **W65C02S Mikroprozessor @ 2 MHz**
- **32 KB RAM** mit Batterie‑Backup
- **32 KB EPROM** mit Floating‑Point BASIC + 6502‑Monitor
- **7‑stellige 7‑Segment‑LED‑Anzeige + 7 LEDs** für Effekte
- **USB‑C Seriell TTL (CH340)** – direkt am PC nutzbar
- **DC/DC‑Step‑Up‑Modul** für stabilen Akkubetrieb
- **CR2032‑Batterie** für SRAM‑Datenerhalt

> Voll funktionsfähig, programmierbar in **Assembler** oder **BASIC** – und trotzdem klein genug, um als Retro‑Namensschild getragen zu werden.

---

### Varianten

**Badge-Version**

<img title="MOS 6502 50th Anniversary Computer Badge Render" src="images/PCB_Render_V2_Badge.png" alt="PCB MOS 6502 50th Anniversary Computer Badge Render Photo" style="zoom:50%;" data-align="center">

<img title="MOS 6502 50th Anniversary Computer Badge Layout" src="images/PCB_Layout_V2_Badge.png" alt="PCB MOS 6502 50th Anniversary Computer Badge Layout" style="zoom:33%;" data-align="center">

- 7,62 × 10,16 cm (3 × 4 Zoll) – klassisches Badge‑Format

---

### Wofür kannst Du es nutzen?

- Als **Retro‑Namensschild** mit Laufschrift deiner Wahl
- Zum **Feiern von 50 Jahren 6502** & der Homecomputer‑Ära
- Als **Lehrprojekt** für Assembler, BASIC und Hardware‑Nostalgie
- Zum **Tüfteln & Spaßhaben** mit minimaler Teilezahl
- Einfach als **cooles Sammlerstück** zum Jubiläum

---

### Technische Ausstattung im Überblick

- W65C02S @ 2 MHz  
- 32 KB RAM mit Batterie‑Backup  
- 32 KB EPROM (BASIC + Monitor)  
- 2× 8‑Bit‑Ausgangslatches  
- 7‑stellige 7‑Segment‑LED‑Anzeige + 7 LEDs  
- USB‑C‑zu‑TTL CH340 UART‑Adapter (BTE17‑06B)  
- DC/DC 5 V Step‑Up Boost‑Converter  
- Ladefunktion für 3× AA **NiCd**‑Akkus

👉 Damit hast Du ein **vollwertiges Retro‑System** in der Hand – minimalistisch, lehrreich und ein echter Hingucker auf jedem Nerd‑Treffen. 😎

---

### Stückliste (BOM)

_Erstellt am 2025‑09‑20 19:50_

| Pos. | Referenz          | Menge | Wert                            | Notizen                                                                                                                                                                                                                                           | Beschreibung                                                           | Datenblatt                                                                                                                      |
|:----:|:----------------- |:-----:| ------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------- |
| 1    | BT1               | 1     | Battery Holder                  | 3× AA **NiCd‑Akkus** (optional). **Bei Batterien (nicht wiederaufladbar) bitte JP2 (Charging) öffnen, da sonst die Batterien bei externer Stromversorgung Ladespannung erhalten. Bei Akkus nur NiCd verwenden. Brandgefahr bei anderen Chemien!** | Holder Keystone 3×AA                                                   | [Link](https://www.digikey.com/en/products/detail/keystone-electronics/106/27386)                                               |
| 2    | BT2               | 1     | Battery Cell Holder CR2032      | CR2032                                                                                                                                                                                                                                            | Battery Holder CR2032 Horizontal Circular Holes                        | [Link](https://www.digikey.com/en/products/detail/keystone-electronics/2464/303813)                                             |
| 3    | C1,C4,C5,C6,C7,C8 | 6     | Kondensator 0,1 µF              |                                                                                                                                                                                                                                                   | Capacitor Disc D4.7 mm W2.5 mm P5,00 mm (THT)                          | [Link](https://www.digikey.com/en/products/detail/kemet/C322C104M5U5TA/818107)                                                  |
| 4    | C2,C3             | 2     | Kondensator 470 µF 10–16 V      |                                                                                                                                                                                                                                                   | Capacitor Radial D8,0 mm P3,50 mm (THT)                                | [Link](https://www.digikey.com/en/products/detail/rubycon/16ZLH470MEFC8X11-5/3563382)                                           |
| 5    | D1,D2,D3          | 3     | **Schottky‑Diode 1N5817**       |                                                                                                                                                                                                                                                   | Diode DO‑41 SOD81 P10,16 mm Horizontal (THT)                           | [Link](https://www.digikey.com/en/products/detail/smc-diode-solutions/1N5817/21705460)                                          |
| 6    | J1                | 1     | 5 V DC‑DC Step‑Up‑Modul         |                                                                                                                                                                                                                                                   | Converter DCDC Step‑Up 5 V Module 10,5×11 (THT mit Pin‑Header)         | [Link](https://de.aliexpress.com/item/1005005624977910.html)                                                                    |
| 7    | J2                | 1     | CH340N SOP‑8 USB‑zu‑TTL‑Modul   |                                                                                                                                                                                                                                                   | CH340N SOP‑8 USB‑zu‑TTL‑Modul (THT mit Pin‑Header)                     | [Link](https://de.aliexpress.com/item/1005009386863437.html)                                                                    |
| 8    | J3                | 1     | Connector Pin‑Header            | (optional)                                                                                                                                                                                                                                        | Connector Pin‑Header 1×05 P2,54 mm Vertical (THT)                      | ~                                                                                                                               |
| 9    | LED1,LED7         | 2     | LED WHITE                       | oder andere Farbe                                                                                                                                                                                                                                 | LED D5,0 mm (THT)                                                      | [Link](https://www.digikey.com/en/products/detail/seoul-semiconductor-inc/LW520AS/2770221)                                      |
| 10   | LED2              | 1     | LED RED                         | oder andere Farbe                                                                                                                                                                                                                                 | LED D5,0 mm (THT)                                                      | [Link](https://www.digikey.com/en/products/detail/american-bright-optoelectronics-corporation/BL-B5134/20506048)                |
| 11   | LED3              | 1     | LED ORANGE                      | oder andere Farbe                                                                                                                                                                                                                                 | LED D5,0 mm (THT)                                                      | [Link](https://www.digikey.com/en/products/detail/rohm-semiconductor/SLR-56DUT32/2337242)                                       |
| 12   | LED4              | 1     | LED YELLOW                      | oder andere Farbe                                                                                                                                                                                                                                 | LED D5,0 mm (THT)                                                      | [Link](https://www.digikey.com/en/products/detail/american-bright-optoelectronics-corporation/BL-B3134/20506076)                |
| 13   | LED5              | 1     | LED GREEN                       | oder andere Farbe                                                                                                                                                                                                                                 | LED D5,0 mm (THT)                                                      | [Link](https://www.digikey.com/en/products/detail/american-bright-optoelectronics-corporation/BL-B2134/20505921)                |
| 14   | LED6              | 1     | LED BLUE                        | oder andere Farbe                                                                                                                                                                                                                                 | LED D5,0 mm (THT)                                                      | [Link](https://www.digikey.com/en/products/detail/lumimax-optoelectronic-technology/LED5BLU-D/25881229)                         |
| 15   | LED8              | 1     | LED RED Power                   | oder andere Farbe                                                                                                                                                                                                                                 | LED D5,0 mm (THT)                                                      | [Link](https://www.digikey.com/en/products/detail/american-bright-optoelectronics-corporation/BL-B5134/20506048)                |
| 16   | R1,R6             | 2     | Widerstand 10 kΩ                |                                                                                                                                                                                                                                                   | Resistor Axial DIN0204 L3,6 mm D1,6 mm P5,08 mm Horizontal 1/4 W (THT) | [Link](https://www.digikey.com/en/products/detail/stackpole-electronics-inc/RNMF14FAD10K0/1683413)                              |
| 17   | R2,R3,R4          | 3     | Widerstand 3,3 kΩ               |                                                                                                                                                                                                                                                   | Resistor Axial DIN0204 L3,6 mm D1,6 mm P5,08 mm Horizontal 1/4 W (THT) | [Link](https://www.digikey.com/en/products/detail/stackpole-electronics-inc/RNMF14FTC3K30/2617342)                              |
| 18   | R5                | 1     | Widerstand 56 Ω                 |                                                                                                                                                                                                                                                   | Resistor Axial DIN0204 L3,6 mm D1,6 mm P5,08 mm Horizontal 1/4 W (THT) | [Link](https://www.digikey.com/en/products/detail/stackpole-electronics-inc/RNMF14FTC10R0/2617280)                              |
| 19   | R7                | 1     | Widerstand 2 kΩ                 |                                                                                                                                                                                                                                                   | Resistor Axial DIN0204 L3,6 mm D1,6 mm P5,08 mm Horizontal 1/4 W (THT) | [Link](https://www.digikey.com/en/products/detail/stackpole-electronics-inc/RNMF14FTC2K00/1683937)                              |
| 20   | SEG1–SEG7         | 7     | 7‑Segment LED SC39‑11EWA        | Beste Erfahrungen mit Kingbright                                                                                                                                                                                                                  | LED Display 7‑Segment (Sx39‑1xxxxx) CC (THT)                           | [Link](https://www.digikey.com/en/products/detail/kingbright/SC39-11EWA/3084564)                                                |
| 21   | SW1               | 1     | Reset‑Button                    |                                                                                                                                                                                                                                                   | Button Switch PUSH 6 mm H4,3 mm (MJTP1230) (THT)                       | [Link](https://www.digikey.com/en/products/detail/apem-inc/MJTP1230/1798037)                                                    |
| 22   | SW2               | 1     | DIP‑Schalter On/Off             |                                                                                                                                                                                                                                                   | DIP‑Schalter SPSTx01 Slide 6,7×4,1 mm W7,62 mm P2,54 mm (THT)          | [Link](https://www2.mouser.com/ProductDetail/Wurth-Elektronik/418127270901?qs=wr8lucFkNMUHAgaqq%2FoMmA%3D%3D)                   |
| 23   | U1                | 1     | 27C256 EPROM                    | alternativ W27E257                                                                                                                                                                                                                                | Gehäuse DIP‑28 W15,24 mm Sockel (THT)                                  | [Link](https://www.digikey.com/en/products/detail/microchip-technology/AT27C256R-70PC/304743)                                   |
| 24   | U2                | 1     | IC CPU W65C02S (DIP‑40)         | Mikroprozessor                                                                                                                                                                                                                                    | Gehäuse DIP‑40 W15,24 mm Sockel (THT)                                  | [Link](https://www.westerndesigncenter.com/wdc/documentation/w65c02s.pdf)                                                       |
| 25   | U3                | 1     | IC 74HC139 (SOP‑16)             |                                                                                                                                                                                                                                                   | Gehäuse SOP‑16 4,4×10,4 mm P1,27 mm (SMD)                              | [Link](https://www.digikey.com/en/products/detail/nexperia-usa-inc/74AHC139PW-Q100J/4020140)                                    |
| 26   | U4                | 1     | IC CY62256N SRAM 32 KB (SOP‑28) | SRAM 32 KB                                                                                                                                                                                                                                        | Gehäuse SOP‑28 8,4×18,16 mm P1,27 mm (SMD)                             | [Link](https://www.digikey.com/en/products/detail/rochester-electronics-llc/CY62256NLL-70ZC/12099783)                           |
| 27   | U5                | 1     | IC MAX690xPA (DIP‑8)            | MAX690 oder MAX692                                                                                                                                                                                                                                | Gehäuse DIP‑8 W7,62 mm (THT)                                           | [Link](https://www.digikey.com/en/products/detail/analog-devices-inc-maxim-integrated/MAX694CPA/948163)                         |
| 28   | U6,U7             | 2     | IC 74HC273 (SOIC‑20)            |                                                                                                                                                                                                                                                   | Gehäuse SOIC‑20W 7,5×12,8 mm P1,27 mm (SMD)                            | [Link](https://www.digikey.com/en/products/detail/toshiba-semiconductor-and-storage/74HC273D/6198939)                           |
| 29   | X1                | 1     | Oszillator 2 MHz (DIP‑14)       |                                                                                                                                                                                                                                                   | Oscillator DIP‑14 (THT)                                                | [Link](https://www.digikey.com/en/products/detail/cts-frequency-controls/MXO45-3C-2M000000/1801885) |

#### Hinweise

Für die ICs **U1** und **U2** wird empfohlen, einen Sockel zu verwenden.

---

## Montage

Überprüfe die Teileliste, um sicherzugehen, dass Du alles hast. Zur Montage benötigst Du einen **Lötkolben**, **Lötzinn** und **Flussmittel** (für die SMD‑ICs). Halte idealerweise auch **Seitenschneider**, **Entlötpumpe** und **Entlötlitze** bereit.

**Empfohlene Reihenfolge:**

1. **SMD‑ICs löten:** U3 (74HC139), U6/U7 (74HC273), danach U4 (SRAM).  
   Tipp: Einen Tropfen Flussmittel an Pin 1 (oben links) und den letzten Pin (unten rechts) geben, IC ausrichten, diese zwei Pins mit wenig Lötzinn fixieren. Sitzt das IC korrekt, restliche Pins mit Flussmittel und wenig Lötzinn einzeln verlöten. **Achte unbedingt auf die Polung**: Pin 1 liegt dort, wo der Pfeil/Marker auf der Platine hinzeigt.
2. **Sockel einsetzen und löten:** für U1 (EPROM) und U2 (W65C02S).
3. **U5 (MAX690) einlöten.**
4. **Oszillator X1 (2 MHz)** als Taktgeber einsetzen.
5. **Dioden D1–D3 (1N5817)** bestücken.
6. **Widerstände R1–R7** bestücken.
7. **Keramikkondensatoren C1, C4–C8** bestücken.
8. **Elektrolytkondensatoren C2, C3 (470 µF, 10–16 V)** bestücken.
9. **Taster SW1 (Reset)** und **DIP‑Schalter SW2 (ON/OFF)** einsetzen.
10. **LED‑Leiste LED1–LED7** sowie **LED8 (Power‑LED)** einsetzen. **Polung beachten!** Das Loch mit dem eckigen Lötpad ist die **Kathode**.
11. **J1 – DC/DC Step‑Up 5 V (10,5×11)** auf der **Rückseite** der Platine montieren. Dazu 3‑polige **Pin‑Pin‑Header** (Male‑Male) verwenden. **Polung beachten:** Die Spule des Step‑Up‑Moduls muss zur Platinenrückseite zeigen.  
    **Ohne Step‑Up‑Modul:** Pin 1 und Pin 3 an **J1** brücken (nicht mit Pin 2 verbinden). **Nur empfehlenswert**, wenn das Badge mit **stabilen 5 V** (Labornetzteil oder USB‑C‑Powerbank) betrieben wird.
12. **J2 – CH340N SOP‑8 USB‑zu‑TTL‑Modul** auf der **Rückseite** per **5‑poligem Pin‑Pin‑Header** verbinden. **Polung beachten.**
13. **Platine reinigen** (Flussmittelrückstände nach dem Löten entfernen).
14. Prüfe, ob alle Bauteile **bis auf** die 7‑Segment‑Displays montiert sind.
15. **7‑Segment‑Displays (SEG1–SEG7)** einsetzen. **Polung beachten:** Unten rechts befindet sich ein kleiner Punkt – dieser muss auf der Platinenvorderseite **nach unten** zeigen.
16. **Batteriehalter BT1 und BT2** montieren (falls gewünscht). **Setze jetzt noch keine Batterien/Akkus ein.**  
    **Achtung:** **Nur 3× AA NiCd 1,2 V** als Akkus verwenden! Die Ladeelektronik ist sehr einfach. **Keine** Li‑Ion‑ oder NiMH‑Akkus verwenden – Brand‑/Explosionsgefahr! Bei Betrieb mit **Batterien** die Ladefunktion deaktivieren (**JP2 öffnen**).
17. **U2 (W65C02S CPU)** und das **programmierte U1 (EPROM)** einsetzen.
18. Glückwunsch – der **MOS 6502 50th Anniversary Computer Badge** ist fertig!

---

## Jumper‑Optionen

Der **MOS 6502 50th Anniversary Computer Badge** hat **zwei** Jumper für unterschiedliche Konfigurationsoptionen.

1. **JP1 – Prozessortyp**  
   Standard: **offen** → für **W65C02S** (Western Design Center). Dieser wird noch produziert und ist leicht erhältlich. Beim W65C02S liegt an Pin 1 das Ausgangssignal **VPB (Vector Pull)** und darf **nicht dauerhaft** auf GND gelegt werden.  
   Ältere Prozessortypen von **MOS**, **Rockwell**, **UMC** oder **Synertek** benötigen hier eine GND‑Verbindung, damit sie funktionieren → **JP1 schließen**.  
   **Hinweis:** Verwende **2 MHz‑Varianten** (z. B. MOS 6502**AD**, Rockwell R6502**AP**, UMC UM6502**A**). Die Schaltung ist mit dem **W65C02S** getestet. **CMOS**‑Varianten (65**C**02) sind wegen des geringeren Stromverbrauchs bevorzugt.
2. **JP2 – Laden der AA‑NiCd‑Akkus**  
   Standard: **geschlossen**.  
   Wenn Du **normale 3× AA 1,5 V Batterien** verwendest, **muss JP2 geöffnet werden**, damit diese nicht versehentlich durch externe Quellen (USB‑C an **J2** oder Pin‑Header **J3**) geladen werden.

---

## Lass es uns arbeiten sehen!

1. **SW2 auf OFF** schalten.  
2. **5 V** an **J2 (USB‑C/CH340N)** oder **J3 (Pin‑Header)** anschließen (**Polung beachten!**).  
3. **SW2 auf ON** schalten → die **Power‑LED** leuchtet und auf den 7‑Segment‑Displays erscheint die Standard‑Laufschrift **„6502 badge for VCF“** oder **„6502 50th Birthday 1975–2025“**.

**Batteriebetrieb testen:**  

- **SW2 OFF**, externe 5 V trennen.  
- **CR2032** für das SRAM und **3× AA NiCd‑Akkus** in die Halter einsetzen.  
- Im Batteriebetrieb leuchtet die Power‑LED nicht, solange **SW2 OFF** ist.  
- **SW2 ON** → der Computer startet; die Laufschrift erscheint.

Wenn Du danach wieder eine externe 5‑V‑Quelle über **USB‑C (J2)** oder **J3** anschließt, werden die **NiCd‑Akkus langsam geladen**. Ein kompletter Ladevorgang dauert etwa **6–8 h**. Die **Laufzeit** mit vollen Akkus beträgt etwa **6–12 h**, abhängig von den Vorwiderständen (LED‑Helligkeit).

Die Leiterplatte hat **vier Befestigungslöcher**. Damit kannst Du Standfüße montieren oder das Board in ein **Gehäuse** einbauen.

<img src="images/Lanyards.jpg" alt="Lanyard für das MOS 6502 Badge" title="Lanyard – MOS 6502 50th Anniversary Computer Badge (1975–2025)" width="700" />

Kurzes Video auf Youtube: [[Zu YouTube weitergehen](https://www.youtube.com/shorts/PbgMO4NnUvw)]

Ein zusätzliches Highlight ist das **Lanyard**, das Du an den oberen Löchern befestigen kannst – so kannst Du den **MOS 6502 50th Anniversary Computer Badge** um den Hals tragen.

---

## Schaltplan

**Schaltplan** (PCB & Display) ⇒ **[Schematic.pdf](downloads/Schematic.pdf)** (PDF, 0,2 MB)

<img src="images/Schematic_PCB_2.0b.png" alt="Schaltplan PCB" title="Schaltplan PCB" width="420" />  
<img src="images/Schematic_Display_2.0b.png" alt="Schaltplan Display" title="Schaltplan Display" width="420" />

Der **MOS 6502 50th Anniversary Computer Badge** ist ein vollständiger minimalistischer Computer: 6502‑CPU mit **2 MHz** Takt, **32 KB RAM (U4)** sowie **32 KB ROM (U1)**. **U3** bildet die **Adressenlogik** für RAM/ROM (**CS**) sowie die Ansteuerung der LED‑Segmente. Die zwei **74HC273 (U6/U7)** fungieren als Latches/Flip‑Flops für die LEDs und die 7‑Segment‑Anzeige. **Bit 7** dient zusätzlich als **TX‑Signal** für die serielle Schnittstelle.

Als **RX** wird **Pin 4 (IRQ)** des 6502 (U2) verwendet. Es handelt sich um eine **Software‑RS‑232**; das Handling übernimmt das **Betriebssystem im ROM**. So konnte ein separater UART entfallen. Die RS‑232‑Schnittstelle arbeitet mit **9600 Baud, 8N1**. Die serielle Verbindung erfolgt über das **CH340N SOP‑8 USB‑zu‑TTL‑Modul (J2)**. Nach dem Anschluss an den PC erscheint ein **neuer COM‑Port**, über den Du mit **9600,8N1** z. B. mit **PuTTY** oder **minicom** kommunizieren kannst. Unter Windows ist ggf. ein Treiber erforderlich: <https://www.arduined.eu/tag/ch340/>.

---

## Speicher

Das Badge‑RAM (32 KB) beginnt bei Adresse **$0000** und geht bis **$7FFF**.

| Bereich | Start | Ende               |
| -------:|:-----:|:------------------ |
| ROM     | 8000h | FFFFh – 32 KB (U1) |
| RAM     | 0000h | 7FFFh – 32 KB (U4) |

---

## Eingabe / Ausgabe

Die beiden **74HC273 8‑Bit‑Latches (U6/U7)** steuern die Ein-/Ausgabe. Sie teilen sich einen gemeinsamen Takt, der von einem **Speicherschreibimpuls (R/W)** in den ROM‑Adressraum abgeleitet wird. Alle 8 **Datenbusleitungen** und die niedrigen 8 **Adressbusleitungen** werden in den Latches gespeichert, wann immer ein **Schreiben** auf die Adressen **$8000–$FFFF** erfolgt. Diese Latches treiben die **8 Reihen** und **7 Spalten** der multiplexed LEDs und 7‑Segment‑Anzeigen an. Der Schaltplan zeigt die logischen Daten‑ und Adressbus‑Verbindungen. In der Realität sind die Adress‑ und Datenpins zwischen den beiden Latches gemischt, um das Platinenlayout zu vereinfachen. Wichtig ist, dass jeder Eingang mit dem richtigen Ausgang verbunden ist: **D0→D0, D5→D5, A4→A4** usw.

![Input‑Output‑Schemata](images/Input-Output-Schema.png "Input‑Output‑Schemata")

Dieser Aufbau erfüllt mehrere widersprüchliche Anforderungen:

- Mit einer einzigen Anweisung können alle **15 LED‑Ausgangsbits** gleichzeitig aktualisiert werden (flackerfreie Anzeige).
- Minimale Hardware (kein separater UART).
- Einfacheres, kleineres Leiterplattenlayout.

**Bit 7** des **Daten‑Latch** wird für die LEDs nicht benötigt und wird daher für die **serielle Ausgabe (TX)** verwendet. Der **IRQ‑Pin** des Prozessors dient als **serieller Eingang (RX)**. Zusammen mit Software ergibt das einen einfachen, minimalistischen, interrupt‑gesteuerten seriellen Port für Ein‑/Ausgabe. **Systemmonitor** und **BASIC‑Interpreter** werden über diesen Port zugänglich gemacht.

---

## LED‑Anzeige

Die **Datenbus‑Latches** treiben die **LED‑Anoden (Segmente)** an, die **Adressbus‑Latches** die **LED‑Kathoden (Ziffern)**.  
Daten‑Latch‑Bits **0–6** wählen die LED‑Segmente (A–G). Da die Ziffern nur 7 Segmente haben, wird **Bit 7** für **TxD** des seriellen Ports verwendet.

Adress‑Latch‑Bits **1–7** wählen die gemeinsamen Kathoden jeder der 7 Ziffern. Da es nur 7 Ziffern gibt, wählt **Adress‑Bit 0** die Kathoden der **7 diskreten LEDs**. Der Schaltplan zeigt die Zuordnung.

Die Anodensignale sind **aktiv high**, die Kathodensignale **aktiv low**.  
Beispiel: Segment **A** der **linken Ziffer** einschalten → **Datenbit 3 = high** und **Adressbit 1 = low**. Das erreichst Du, indem Du den Wert **$08** an die Adresse **$80FD** schreibst.

Aufgeschlüsselt:

```
; Datenbits
76543210
00001000 = 08h

; Adressbits
76543210
11111101 = FDh
```

Um die Latches zu beschreiben, schreibe in den ROM‑Bereich **$8000–$FFFF**. Addiere also **$8000** zur Adresse **$00FD** → **$80FD**. (Ein Schreiben nach **$95FD** oder **$FEFD** hat den gleichen Effekt – jede Adresse ≥ **$8000** funktioniert.)

---

## Serieller Port

Der serielle Port ist ein **TTL‑asynchroner** Datentransfer: **TX**, **RX** und **GND**. Er ähnelt **RS‑232**, verwendet aber **5 V/0 V‑Logikpegel** und **nicht invertierte** Daten (Leerlauf = 5 V = 1). Du kannst daher entweder einen **TTL‑zu‑RS‑232‑Adapter** an **J3** verwenden oder das **CH340N USB‑zu‑TTL‑Modul (J2)** aufstecken und als USB‑Seriell‑Adapter nutzen (von den meisten Systemen unterstützt). Bonus: Die **5 V** vom USB‑Port versorgen die Platine und **laden** die NiCd‑Akkus (wenn vorhanden und **JP2 geschlossen** ist).

**Konfiguration:** `9600, N, 8, 1` (9600 Baud, keine Parität, 8 Datenbits, 1 Stopbit).

**TX schreiben:** Bit 7 setzen/löschen → `00h` (TX=0) oder `80h` (TX=1) an **irgendeine** Adresse **≥ $8000** schreiben.  
**Alle LEDs aus:** an Adresse ≥ **$8000** mit **Low‑Byte `FFh`** schreiben (z. B. **$80FF**), dadurch sind alle 8 Kathoden high (inaktiv).  
**LED‑Status halten:** LED‑Daten‑ und Adresswerte im RAM puffern.

**RX lesen:** Der **IRQ‑Pin 4** erfasst **Low‑Pegel** direkt; High‑Pegel werden über präzise **Timing‑Schleifen** erkannt. Das RX‑Signal wird vorher über **U3 invertiert**, sodass die Verarbeitung **RS‑232‑konform** ist.

**Terminal‑Programm:** Unter Windows z. B. **PuTTY** (COM‑Port), unter Linux **minicom**/`miniterm`. Für **Copy & Paste** von Quelltexten **Sende‑Pausen** setzen (nicht jedes Terminal kann das):

1. Verzögerung beim Senden eines **Bytes**: **50 ms**  
2. Verzögerung nach **LF/CR**: **500 ms**

Da es sich um eine **softwarebasierte** serielle Schnittstelle ohne FIFO handelt, führen zu schnelle Übertragungen zu **Timing‑Problemen** und **Fehlern**.

---

## Softwarebeschreibung

Beim Einschalten/Reset springt der 6502 über den Reset‑Vektor (16‑Bit‑Wert an **$FFFC/$FFFD**) in die Reset‑Routine. Diese initialisiert **LED‑Anzeige** und **Software‑Serial** und verzweigt dann in den **Maschinensprachen‑Monitor**.

Der Monitor arbeitet über den **seriellen Port** mit **9600, N, 8, 1** und erzeugt gleichzeitig eine **Laufschrift** auf den 7 LED‑Ziffern (Standard: „6502 badge for VCF“ oder „6502 50th Birthday 1975–2025“). Die 7 **diskreten LEDs** laufen im **„Knight Rider“‑Muster**. Die Anzeige wird während der Wartezeit auf serielle Eingaben fortlaufend aktualisiert.

---

## 6502 Badge – Monitor‑ & Referenzhandbuch

Eingabe von `?` + `<Return>` zeigt den Hilfebildschirm:

<img src="images/OS_Monitor.png" title="Monitor‑Hilfebildschirm" alt="Screenshot: Monitor‑Help" width="700" />

### Monitorbefehle

Grundformat einer Befehlszeile:

```
SSSS.EEEE C <Return>
```

- `SSSS` / `EEEE` = Start‑/Endadresse (durch Punkt getrennt)  
- `C` = **Befehlssymbol** (nicht‑alphanumerisches Zeichen)  
- `<Return>` = Eingabetaste  
  **Hinweis:** Keine Leerzeichen zwischen diesen Elementen (z. B. `1234.5678L<Return>`).

Adressen können 1–2 Bytes (2–4 Hexziffern) lang sein. Werden mehr als 4 Hexziffern eingegeben, interpretiert der Monitor nur die **letzten 4** (z. B. aus `1A2B3C.4D5E6C` werden `2B3C` und `5E6C`). Kürzere Eingaben werden links mit `0` aufgefüllt; `0.3FF` deckt somit `$0000–$03FF` ab.

Bei einigen Befehlen ist die Adresse optional. Der Monitor merkt sich den **zuletzt eingegebenen** Hex‑Wert und **inkrementiert** ihn automatisch, wenn keine neue Adresse folgt. Beispiel:

- `1000L<Return>` disassembliert **20 Zeilen** ab `$1000`.  
- Ein folgendes `L<Return>` macht an der letzten Adresse weiter.  
- `1000LLL<Return>` zeigt so **60 Zeilen** ab `$1000`.

`?<Return>` zeigt eine Kurz‑Hilfe:

```
Commands are :
Syntax = {} required, [] optional, HHHH hex address, DD hex data

[HHHH][ HHHH]{Return}         - Hex dump address(s) (bis zu 16 ohne Adresse)
[HHHH]{.HHHH}{Return}         - Hex dump Bereich (16 pro Zeile)
[HHHH]{:DD}[ DD]{Return}      - Datenbytes ändern
[HHHH]{G}{Return}             - Programm ausführen (RTS kehrt zum Monitor zurück)
{HHHH.HHHH>HHHHI}{Return}     - Bereich (2.) nach unten in 1.→3. einfügen
[HHHH]{L}{Return}             - 20 Zeilen disassemblieren
[HHHH]{.HHHH}{L}{Return}      - Bereich disassemblieren
{HHHH.HHHH>HHHHM}{Return}     - Bereich (1.→2.) nach 3. verschieben
{HHHH}[ HHHH]{Q}{Return}      - Textdump Adresse(n)
[HHHH]{.HHHH}{Q}{Return}      - Textdump Bereich (16/Zeile)
{S}[bis zu 32 Textzeichen]{Return} - LED-Nachricht setzen
[HHHH]{U}{Return}             - Upload (PC→SBC, XMODEM/CRC)
[HHHH.HHHH]{X}{Return}        - Download (SBC→PC, XMODEM/CRC)
{V}{Return}                   - Monitorversion
{P*}{Return}                  - Geschütztes Herunterfahren
{!}{Return}                   - Mini-Assembler
{@}{Return}                   - EhBASIC Kaltstart
{#}{Return}                   - EhBASIC Warmstart
{?}{Return}                   - Hilfe anzeigen
```

### HEX‑Dump

```
[HHHH][ HHHH]<Return>   - Hexdump Adresse(n) (bis zu 16 ohne Adresse)
[HHHH]{.HHHH}<Return>   - Hexdump Bereich (16 pro Zeile)
```

Zeigt den Rohinhalt des gewählten Speichers in Hex.

**Varianten:**

1. **Nur Startadresse** → nur dieses Byte (mehrere Adressen durch Leerzeichen).  
2. **Start–Ende** → Bereich, in 16‑Byte‑Zeilen gerahmt (Beginn jeweils bei `$xxx0`).  
3. **Ohne Adresse** → bis zu 16 Bytes ab letzter gemerkter Adresse.

Beispiel `5.2D<Return>`:

```
0005 - 2D FF 06 - 42 55 7A 68 AE F5 5B FF
0010 - 7C FF 37 FF FF FC DF EF - 8F CB D7 FF FF 5F 19 76
0020 - 36 DA D4 5D EF F3 EA FF - EA E1 E3 65 4B FF
```

### Speicher bearbeiten (Edit Memory)

```
[HHHH]{:DD}[ DD]<Return>   - Datenbytes ändern
```

Schreibt Daten in RAM. Nach der Adresse folgt ein Doppelpunkt `:` und mindestens ein Datenbyte `DD` (weitere Bytes durch Leerzeichen; fortlaufend).

Beispiel: Speicher `$1000` auf `$55` setzen → `1000:55<Return>`.

Schreibzugriffe auf ROM erzeugen **keinen Fehler**, haben aber keine Wirkung (auf dem Badge wirken sie auf die **I/O‑Latches** – siehe oben).

### Speicher verschieben (Move Memory)

```
{SSSS.EEEE>DDDDM}<Return>
```

Kopiert Speicher **von** `SSSS` **bis** `EEEE` **nach** `DDDD` (vorwärts).

Praktischer Trick zum **Füllen**: Erst mit *Edit Memory* das erste Byte setzen, dann mit *Move* den Rest füllen.

Beispiel: `$1000–$1FFF` auf `$00`:

```
1000:00<Return>
1000.1FFE>1001M<Return>
```

**Achtung:** Liegt `DDDD` innerhalb `SSSS–EEEE`, werden Ursprungsdaten überschrieben. Nutze ggf. **Insert Memory**.

### Speicher einfügen (Insert Memory)

```
{SSSS.EEEE>DDDDI}<Return>
```

Wie *Move*, jedoch **rückwärts** (kopiert ab `EEEE` nach unten). So lassen sich Lücken beliebiger Größe innerhalb eines Bereichs schaffen. Liegt `DDDD` außerhalb, funktionieren beide Varianten.

### Ausführen (Execute)

```
[HHHH]{G}<Return>
```

Startet ein Maschinenprogramm. Ein `RTS` (`$60`) kehrt in den Monitor zurück. Ohne Adresse wird die zuletzt gespeicherte verwendet – empfehlenswert ist eine **explizite Startadresse** (z. B. `1000G<Return>`).

### Disassemblieren (List)

```
[HHHH]{L}<Return>          - 20 Zeilen
[HHHH]{.HHHH}{L}<Return>   - Bereich
```

Ohne Adresse: 20 Zeilen ab der zuletzt genutzten Adresse. Beispiel:

```
>FF00L

FF00-  x    78         SEI  
FF01-  X    D8         CLD  
FF02-  ".   A2 FF      LDX  #$FF
...
FF25-  )h   A9 E8      LDA  #$E8
>
```

Format: Adresse – ASCII der Bytes (nicht druckbar → `.`) – Hexwerte – Mnemonic + Operanden.

### Textausgabe (Text Dump)

```
{HHHH}[ HHHH]{Q}<Return>
[HHHH]{.HHHH}{Q}<Return>
```

Wie *Hex Dump*, aber als **ASCII**. Nützlich, um Textblöcke im Speicher zu finden. Nicht druckbare Zeichen → `.`

### LED‑Text setzen

```
{S}[bis zu 32 Zeichen]<Return>
```

Setzt die scrollende LED‑Nachricht (32‑Byte‑Puffer; überlange Eingaben werden abgeschnitten). Beispiel: `S6502 badge<Return>` zeigt:

```
6502 badge
```

### Upload (XMODEM)

```
[HHHH]{U}<Return>  – Upload vom PC zum Badge (XMODEM/CRC)
```

Die Datei wird ab der angegebenen (oder zuletzt gemerkten) Adresse gespeichert. **Achtung**: Durch den 128‑Byte‑Puffer können bis zu **127** zusätzliche Bytes am Ende landen – vermeide Überschreiben. Nur **XMODEM/CRC** wird unterstützt (kein Checksum‑/1k‑Modus).

### Download (XMODEM)

```
[HHHH.HHHH]{X}<Return> – Download vom Badge zum PC (XMODEM/CRC)
```

Sendet den angegebenen Bereich. Gib nach Möglichkeit immer Adressen an (gleiche 128‑Byte‑Pufferhinweise wie oben). Nur **XMODEM/CRC**.

### Version anzeigen

```
{V}<Return>
```

Beispiel:

```
>V
65C02 Monitor v5.2 (5-27-17) Ready
with Enhanced Basic Interpreter (c) Lee Davison
(Press ? for help)
>
```

### Geschütztes Herunterfahren

```
{P*}<Return>
```

Schaltet die LEDs aus und springt in eine Endlosschleife im ROM. So bleibt der **RAM‑Inhalt** vor dem Ausschalten intakt.

### Mini‑Assembler

```
{!}<Return>   – Assembler betreten
```

Einfacher RAM‑Assembler (Hex‑Operanden, keine Labels/Arithmetik). Prompt wechselt von `>` zu `!`. Hilfe (`!?`) zeigt:

```
HHHH=hex address, OPC=Opcode, DD=hex data, '_'=Space/Tab
'$' optional, alles HEX. Nach ';' wird Eingabe ignoriert.

{HHHH}{Return}                      - Eingabeadresse setzen
[HHHH][_]{OPC}[_][#($DD_HHHH,X),Y]{Return} - Zeile assemblieren
[HHHH]{L}{Return}                   - 20 Zeilen disassemblieren
{Return}                            - Assembler verlassen
{?}{Return}                         - Hilfemenü
```

Unterstützte Mnemonics u. a.: `ADC AND ASL BCC ... WAI STP BBRx BBSx RMBx SMBx .DB .DW .DS`.  
**Hinweis:** WDC‑Opcodes (`WAI`, `STP`, `BBRx/BBSx`, `RMBx/SMBx`) sind im Badge‑Prozessor **nicht verfügbar**, werden aber vom Assembler akzeptiert; siehe WDC‑Handbuch. Pseudo‑Opcodes:

- `.DB HH`  – 1 Byte ablegen  
- `.DW HHHH` – 2 Bytes (low‑Byte zuerst)  
- `.DS 'Text'` – ASCII‑String ablegen

**Beispiel‑Session (Auszug):**

```
!1000 LDA #FF
1000-  ).   A9 FF      LDA  #$FF
! STA 00
1002-  ..   85 00      STA  $00
! LDA (00),Y
1004-  1.   B1 00      LDA  ($00),Y
! STA (02,X)
1006-  ..   81 02      STA  ($02,X)
! INX
1008-  h    E8         INX  
! INY
1009-  H    C8         INY  
! BNE 1000
100A-  Pt   D0 F4      BNE  $1000
! BNE 2000
          ^
! RTS
100C-  `    60         RTS  
...
!1000L
1000-  ).   A9 FF      LDA  #$FF
...
1020-  .    00         BRK  
1021-  .    00         BRK  
1022-  .    00         BRK  
!
```

Der `^`‑Marker kennzeichnet einen Fehler (z. B. Branch‑Ziel außerhalb der Reichweite).

---

## EhBASIC: Kaltstart & Warmstart

**Kaltstart** `{@}<Return>` initialisiert RAM und setzt die Obergrenze („top of memory“). Eingabe in **Dezimal**:

- `2048` → 2 KB RAM
- `32768` → 32 KB RAM

Beispiel (2 KB RAM):

```
>@
Memory size ? 2048
1023 Bytes free
Enhanced BASIC 2.22

Ready
```

Die ersten 1 KB RAM nutzt Monitor & LED‑Anzeige; daher bleiben bei 2 KB gesamt ≈ 1 KB frei. Mit `SYS<Return>` (neu) kehrst Du vom EhBASIC‑Prompt in den Monitor zurück.

**Warmstart** `{#}<Return>` kehrt nach `SYS` zu EhBASIC zurück (ohne Neuinitialisierung; RAM‑Programm bleibt erhalten).

---

## EhBASIC‑Kurzübersicht & Schlüsselwörter

EhBASIC von **Lee Davison** (hier angepasst mit freundlicher Genehmigung). Handbuch: `http://www.sunrise-ev.com/photos/6502/EhBASIC-manual.pdf`. Der Quelltext ist umfangreich kommentiert.

**Stichwortliste (Auszug):**  
`ABS AND ASC ATN BIN$ BITCLR BITSET BITTST CALL CHR$ CLEAR CONT COS DATA DEC DEEK DEF DIM DO DOKE ELSE END EOR EXP FN FOR FRE GET GOSUB GOTO HEX$ IF INC INPUT INT IRQ LCASE$ LEFT$ LEN LET LIST LOAD LOG LOOP MAX MID$ MIN NEW NEXT NMI NOT NULL OFF ON OR PEEK PI POKE POS PRINT READ REM RESTORE RETIRQ RETNMI RETURN RIGHT$ RND RUN SADD SAVE SGN SIN SPC( SQR STEP STOP STR$ SWAP SYS TAB( TAN THEN TO TWOPI UCASE$ UNTIL USR VAL VARPTR WAIT WHILE WIDTH + - * / ^ << >> > = <`

- Schlüsselwörter **GROSS** und **ohne Leerzeichen**.  
- Zahlen: Integer, Dezimal oder Float; Präfix `$` (Hex) oder `%` (Binär). Beispiele: `$0A`, `1`, `-142`, `96.3`, `2.718E-3`.  
- Variablen: numerisch, `Strings$` oder Arrays `(n)`; Strings in Anführungszeichen (`"Hello world"`).

---

## LED‑Betrieb

Der Monitor enthält Routinen zum **Refresh** der scrollenden **7‑Segment‑Ziffern** sowie der **diskreten LEDs**.  
Prinzip: Adress‑Latch auf die erste Stelle setzen → Bitmuster aus RAM holen → in Puffer schreiben → kurz einschalten → nächste Stelle. Zyklisch wiederholen (**Persistence of Vision**).  
Für **Scrollen** wird der Startzeiger periodisch verschoben; die Geschwindigkeit ergibt sich aus der Anzahl der Refresh‑Zyklen zwischen Verschiebungen. Während der Eingabewartezeit (Monitor/EhBASIC) läuft die Anzeige flüssig; bei Zeichenempfang gibt es kurze Unterbrechungen.

**Quellen:** `LEDdrive.asm`, `font.asm`.

**Wichtige RAM‑Adressen:**

```
Lbuff   = $02A0 ; LED-Textpuffer (max. 32 Bytes)
LDbuff  = $02C0 ; Puffer diskrete LEDs (max. 32 Bits)
Lptr    = $E2   ; LED-Zeiger (0..31)
Ldig    = $E3   ; Digit-Zähler (0..7; 0 = diskrete LEDs)
Lscn    = $E4   ; Scan-Delay (Helligkeit/Flicker) – 0..255, 0=Display-Refresh aus
Lscl    = $E5   ; Scroll-Delay – 0..255, 0=statisch
Lscnc   = $E6   ; Scan-Zähler (läuft von Lscn runter)
Lsclc   = $E7   ; Scroll-Zähler (läuft von Lscl runter)
LEDchk1 = $E8   ; Konfig-Checksumme 1
LEDchk2 = $E9   ; Konfig-Checksumme 2
```

`Lbuff`/`LDbuff` sind **synchron** (Stelle 0..31). Setze `Lscn=$00`, um den Monitor‑Refresh zu deaktivieren (für eigene LED‑Routinen).  
`LEDchk1=$A5` **und** `LEDchk2=$5A` verhindern das Überschreiben der Puffer bei Reset (sonst Standardtext „6502 badge for VCF“ + „Knight Rider“). Mit *Edit Memory* lassen sich die Flags setzen.

---

## Serielle Ein-/Ausgabe (ROM‑Routinen)

Es gibt drei Monitor‑Subroutinen für serielle I/O (per `JSR` aufrufen). **Achtung:** Es existieren zwei Monitor‑ROM‑Versionen; Adressen je nach Versionsdatum (`V`‑Befehl) verwenden:

- **Serial_Output** (`$EAE8` *oder* `$EAEC`) – sendet 1 Byte (im Akkumulator); `X/Y` bleiben unverändert.
  
  ```asm
  ; 5-17-17 ROM          ; 2-24-18 ROM
  LDA #$41               LDA #$41   ; ASCII "A"
  JSR $EAE8              JSR $EAEC  ; senden
  ```

- **Serial_Input** (`$EB35` *oder* `$EB39`) – blockierendes Lesen; Byte im A; `X/Y` unverändert; Flags `Z/N` gesetzt.
  
  ```asm
  JSR $EB35              JSR $EB39  ; Zeichen holen
  STA $400               STA $400   ; speichern
  JSR $EAE8              JSR $EAEC  ; Echo
  ```

- **Scan_Input** (`$EB4C` *oder* `$EB50`) – nicht blockierend; keine Eingabe → Carry **gelöscht**; bei Eingabe: Byte in A, `Z/N` gesetzt, Carry **gesetzt**.
  
  ```asm
  Loop  JSR $EB4C        JSR $EB50  ; prüfen
        BCC Loop         BCC Loop   ; nichts da → erneut
        BMI Loop         BMI Loop   ; >$7F? (N=1) → erneut
        STA $400         STA $400   ; speichern
  ```

---

## Systemspeicherbelegung

Die folgenden Bereiche nutzt das System. Ob Überschreiben zulässig ist, liegt bei Dir; studiere die Quellen.

### Zero Page

| Bereich   | Nutzung           |
| ---------:| ----------------- |
| `$00–$13` | EhBASIC           |
| `$14–$31` | frei              |
| `$32–$3F` | Monitor‑Variablen |
| `$40–$5A` | frei              |
| `$5B–$DF` | EhBASIC           |
| `$E2–$E9` | LED‑Treiber       |
| `$EA–$ED` | Serieller Treiber |
| `$EF–$FF` | EhBASIC           |

### RAM

| Bereich       | Nutzung                                   |
| -------------:| ----------------------------------------- |
| `$0100–$01FF` | System‑Stack                              |
| `$0200–$027F` | Serieller Receive‑Ringpuffer              |
| `$02A0–$02DF` | LED‑Puffer                                |
| `$0300–$037F` | Monitor‑Eingabepuffer                     |
| `$0390–$03FF` | EhBASIC‑Eingabepuffer                     |
| `$0400–$7FFF` | Nutzer‑RAM / EhBASIC‑Programm (32 KB RAM) |

### ROM (je nach Monitor‑Datum)

| **5‑17‑17 ROM** | **2‑24‑18 ROM** | Beschreibung                |
| ---------------:| ---------------:| --------------------------- |
| `$C000–$C1FF`   | `$C000–$C1FF`   | CRC‑Lookup‑Tabelle (XMODEM) |
| `$C200–$EA9B`   | `$C200–$EA9F`   | EhBASIC                     |
| `$EA9C–$EB64`   | `$EAA0–$EB68`   | Serielle I/O‑Routinen       |
| `$EB65–$FC39`   | `$EB69–$FC3D`   | Monitor                     |
| `$FC3A–$FD93`   | `$FC3E–$FD97`   | LED‑Unterstützung           |
| `$FD94–$FFBE`   | `$FD98–$FFC2`   | XMODEM                      |
| `$FFBF–$FFFF`   | `$FFC3–$FFFF`   | Resetcode & Vektoren        |

---

## Quellcode‑Organisation & Build‑Hinweise

Mit Ausnahme von EhBASIC stammt die Software von **Daryl Rictor**. Nutzung und Anpassung für **nicht‑kommerzielle** Zwecke erlaubt.

**Dateien:**

- `sbc.asm` – „Makefile“: lädt alle Quellen in richtiger Reihenfolge/Adresse  
- `basic.asm` – EhBASIC‑Quelle  
- `basldsv.asm` – Patch für Load/Save via XMODEM  
- `sbcOS.asm` – Monitor inkl. Disassembler & Mini‑Assembler  
- `serial.asm` – Software‑Serielltreiber  
- `LEDdrive.asm` – LED‑Treiber (Refresh, Scroll, Text)  
- `font.asm` – LED‑Font (ASCII→Latch‑Pins)  
- `xmodem.asm` – XMODEM‑Protokoll  
- `CRCtable.asm` – CRC‑Lookuptabelle  
- `reset.asm` – Reset/Initialisierung; ROM‑Vektoren `$FFFA–$FFFF`; BRK‑Handler (`$00`) → Reset & Monitor

**Assemblieren (6502 Macroassembler & Simulator, `6502.exe`):**

1. Programm starten  
2. `sbc.asm` öffnen (`File → Open → sbc.asm`)  
3. Optionen:  
   - `Assembler` → **Extra byte after BRK**: **deaktivieren**  
   - `General` → **65C02, 6501** auswählen  
4. Assemblieren (`F7`)  
5. Objekt speichern (`File → Save Code`): Intel‑Hex, S‑Record oder Binär  
   - **Startadresse**: `0xC000` (16 KB ROM) **oder** `0x8000` (32 KB ROM)  
   - **Endadresse**: `0xFFFF`  
   - **OK** → **SAVE**

---

## Downloads / Firmware / Manuals

1. Angepasste BadgeOS‑Firmware **32 KB** (27C256, U1; 7× LEDs der 50th‑Version) ⇒ **[BadgeOS_32k_50th.rom](downloads/BadgeOS_32k_50th.rom)** (BIN, 32 KB)  
2. Original **BadgeOS** (Firmware/ROM) ⇒ **[BadgeOS.zip](downloads/BadgeOS.zip)** (ZIP, 0,8 MB)  
3. Original **Badge Manual** von **Lee Hart, Daryl Rictor und Josh Bensadon** ⇒ **[badge-manual.pdf](downloads/badge-manual.pdf)** (PDF, 1,6 MB)  
4. Original **EhBASIC Manual** ⇒ **[EhBASIC-manual.pdf](downloads/EhBASIC-manual.pdf)** (PDF, 0,5 MB)  
5. **Schaltplan** (PCB & Display) ⇒ **[Schematic.pdf](downloads/Schematic.pdf)** (PDF, 0,2 MB)  
6. **Platinenlayout (Gerber)** ⇒ **[gerber/](gerber/)**  
7. **BOM‑Dateien** ⇒ **[bom/](bom/)**  
8. Treiber für **CH340 USB‑C zu Serial TTL**: <https://www.arduined.eu/tag/ch340/>  
9. Weitere Downloads ⇒ **[downloads/](downloads/)**

---

## Bestellung

In Kürze werde ich das Projekt bei **pcbway.com** als **Shared Project** allen zur Verfügung stellen.

---

## Fehlerbehebung

1. **Power‑LED leuchtet, LEDs/Laufschrift flackern.**  
   Prüfe, ob an **U2 Pin 8** stabile **4,5–5 V** anliegen. Liegen am 5‑V‑Step‑Up‑Booster **< 1,2 V** an, bricht die Spannung zusammen und pulsiert.
2. **Einige LEDs/7‑Segment‑Anzeigen leuchten nicht oder dauerhaft.**  
   Prüfe **U6/U7 (74HC273)** auf sicheren Pin‑Kontakt und mögliche **Lötbrücken**.
3. **Power‑LED leuchtet, sonst keine Funktion.**  
   (1) **U3 (74HC139)** auf Kurzschlüsse/Pins prüfen. (2) **U1 (EPROM)** und **U2 (Mikroprozessor)** korrekt einsetzen/prüfen (Firmware!). (3) **U4 (SRAM)** prüfen. (4) **Oszillator X1** prüfen.
4. **Keine USB‑Verbindung (Windows).**  
   **CH340‑Treiber** installieren (siehe Downloads).

---

## Haftungsausschluss

Dieses Projekt ist ein nicht‑kommerzielles Hobbyprojekt. Der Nachbau und die Nutzung des **MOS 6502 – 50th Anniversary Computer Badge (1975–2025)** erfolgen ausschließlich auf **eigenes Risiko**. Es wird **keinerlei Garantie** für Funktion, Sicherheit, Vollständigkeit oder Fehlerfreiheit übernommen. Der Ersteller (Frank Eggen) haftet **nicht** für Schäden, Verluste oder Folgeschäden, die aus dem Nachbau oder der Verwendung entstehen können.

---

## Spenden

Ich habe viele Stunden an diesem Projekt gearbeitet. Wenn Du diese Arbeit unterstützen möchtest, kannst Du gerne etwas für die **Kaffeekasse** spenden. Vielen Dank!  
👉 **[PayPal – Spende](https://www.paypal.com/donate/?cmd=_s-xclick&hosted_button_id=Q8HXKYARXKT4L&ssrt=1714757590172)**

---

## Danksagung

1. Dieses Projekt basiert auf der Idee von **Lee Hart, Daryl Rictor und Josh Bensadon**. 👉 Originalprojekt: <http://www.sunrise-ev.com/6502.htm>  
   Ein großes Dankeschön geht an die ursprünglichen Entwickler für ihre Pionierarbeit – und besonders an **Lee Hart** für viele hilfreiche Tipps während der Überarbeitung. 🙏
2. **Chuck Peddle** und seinem Team bei **MOS** (u. a. Terry Holdt, Wil Mathys, Rod Orgill, Harry Bawcom, Sydney Anne Holt, Walt Eisenhower, John Paivinen), die mit ihrer Vision den 6502 ermöglichten: <https://www.team6502.org>
3. **Bill Mensch**, Gründer des **Western Design Center**, der den 6502 bis heute ermöglicht, dokumentiert und weiterentwickelt: <https://www.westerndesigncenter.com>
4. **Ben Eater** für sein Projekt „Build a 6502 computer“: <https://eater.net/6502>
