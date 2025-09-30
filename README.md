# The MOS 6502 – 50th Anniversary Computer Badge (1975–2025)

## A Retro Computer in Badge Format for 8‑bit 6502 Fans

By Frank Eggen

👉 **[German Version](README_DE.md)**

[![Watch the video on YouTube](images/Youtube.jpg "YouTube: MOS 6502 – 50th Anniversary Computer Badge")](https://youtu.be/MOvFbZeAMVU)

---

Based on an idea by **Lee Hart, Daryl Rictor, and Josh Bensadon** (revived and updated).  
👉 Original project: <http://www.sunrise-ev.com/6502.htm>

---

## 50 Years of the 8‑bit MOS 6502 Microprocessor

<img src="images/white-ceramic-6502-illustration.png" title="White Ceramic 6502 CPU Illustration" alt="Illustration of a white 6502 CPU" width="600" />

The legendary **MOS 6502** was introduced in 1975 and changed the world of computing.  
It delivered performance at a low price and enabled the rise of **home computers**.

Famous 6502‑based systems:

- Apple II
- Commodore VIC‑20 & C64
- Nintendo NES
- BBC Micro
- Atari VCS

👉 Learn more about the history: <https://www.team6502.org>

---

### What is the “Computer Badge”?

<img title="The MOS 6502 – 50th Anniversary Computer Badge (1975–2025)" src="images/The_MOS_6502–50th_Anniversary_Computer_Badge_Real.jpg" alt="The MOS 6502 – 50th Anniversary Computer Badge (1975–2025)" data-align="center" style="zoom:25%;">

The **MOS 6502 50th Anniversary Computer Badge** is a **minimalist re‑release** of the original—compatible, yet rebuilt with modern parts to make it easy to assemble today.

**Highlights:**

- **W65C02S microprocessor @ 2 MHz**
- **32 KB RAM** with battery backup
- **32 KB EPROM** with floating‑point BASIC + 6502 monitor
- **7‑digit 7‑segment LED display + 7 LEDs** for effects
- **USB‑C Serial TTL (CH340)** – plug directly into your PC
- **DC/DC step‑up module** for stable battery operation
- **CR2032 coin cell** to retain SRAM data

> Fully functional, programmable in **assembler** or **BASIC**—and still small enough to wear as a retro name badge.

---

### Version

**Badge version**

<img title="MOS 6502 50th Anniversary Computer Badge Render" src="images/PCB_Render_V2_Badge.png" alt="PCB MOS 6502 50th Anniversary Computer Badge Render Photo" style="zoom:50%;" data-align="center">

<img title="MOS 6502 50th Anniversary Computer Badge Layout" src="images/PCB_Layout_V2_Badge.png" alt="PCB MOS 6502 50th Anniversary Computer Badge Layout" style="zoom:33%;" data-align="center">

- 7.62 × 10.16 cm (3 × 4 inches) – classic badge format

---

### What can you use it for?

- As a **retro name badge** with a scrolling text of your choice
- To **celebrate 50 years of the 6502** and the home‑computer era
- As a **teaching project** for assembler, BASIC, and hardware nostalgia
- For **tinkering & fun** with a minimal part count
- Simply as a **cool collectible** for the anniversary

---

### Technical Specs at a Glance

- W65C02S @ 2 MHz  
- 32 KB RAM with battery backup  
- 32 KB EPROM (BASIC + Monitor)  
- 2× 8‑bit output latches  
- 7‑digit 7‑segment LED display + 7 LEDs  
- USB‑C to TTL CH340 UART adapter (BTE17‑06B)  
- DC/DC 5 V step‑up boost converter  
- Charging function for **3× AA NiCd** cells

👉 This gives you a **fully featured retro system** in your hand—minimalist, educational, and a real eye‑catcher at any nerd meetup. 😎

---

### Bill of Materials (BOM)

_Created on 2025‑09‑20 19:50_

| Pos. | Reference         | Qty | Value                           | Notes                                                                                                                                                                                                                                                | Description                                                            | Datasheet/Link                                                                                                                  |
|:----:|:----------------- |:---:| ------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------- |
| 1    | BT1               | 1   | Battery Holder                  | **3× AA NiCd cells** (optional). **If using non‑rechargeable batteries, open JP2 (Charging), otherwise the batteries receive charge when an external supply is connected. If using rechargeables, use NiCd only. Fire risk with other chemistries!** | Holder Keystone 3×AA                                                   | [Link](https://www.digikey.com/en/products/detail/keystone-electronics/106/27386)                                               |
| 2    | BT2               | 1   | Battery Cell Holder CR2032      | CR2032                                                                                                                                                                                                                                               | Battery Holder CR2032 Horizontal Circular Holes                        | [Link](https://www.digikey.com/en/products/detail/keystone-electronics/2464/303813)                                             |
| 3    | C1,C4,C5,C6,C7,C8 | 6   | Capacitor 0.1 µF                |                                                                                                                                                                                                                                                      | Capacitor Disc D4.7 mm W2.5 mm P5.00 mm (THT)                          | [Link](https://www.digikey.com/en/products/detail/kemet/C322C104M5U5TA/818107)                                                  |
| 4    | C2,C3             | 2   | Capacitor 470 µF 10–16 V        |                                                                                                                                                                                                                                                      | Capacitor Radial D8.0 mm P3.50 mm (THT)                                | [Link](https://www.digikey.com/en/products/detail/rubycon/16ZLH470MEFC8X11-5/3563382)                                           |
| 5    | D1,D2,D3          | 3   | **Schottky Diode 1N5817**       |                                                                                                                                                                                                                                                      | Diode DO‑41 SOD81 P10.16 mm Horizontal (THT)                           | [Link](https://www.digikey.com/en/products/detail/smc-diode-solutions/1N5817/21705460)                                          |
| 6    | J1                | 1   | 5 V DC‑DC Step‑Up Module        |                                                                                                                                                                                                                                                      | Converter DCDC Step‑Up 5 V Module 10.5×11 (THT with pin header)        | [Link](https://de.aliexpress.com/item/1005005624977910.html)                                                                    |
| 7    | J2                | 1   | CH340N SOP‑8 USB‑to‑TTL Module  |                                                                                                                                                                                                                                                      | CH340N SOP‑8 USB‑to‑TTL Module (THT with pin header)                   | [Link](https://de.aliexpress.com/item/1005009386863437.html)                                                                    |
| 8    | J3                | 1   | Connector Pin Header            | (optional)                                                                                                                                                                                                                                           | Connector Pin Header 1×05 P2.54 mm Vertical (THT)                      | ~                                                                                                                               |
| 9    | LED1,LED7         | 2   | LED WHITE                       | or other color                                                                                                                                                                                                                                       | LED D5.0 mm (THT)                                                      | [Link](https://www.digikey.com/en/products/detail/seoul-semiconductor-inc/LW520AS/2770221)                                      |
| 10   | LED2              | 1   | LED RED                         | or other color                                                                                                                                                                                                                                       | LED D5.0 mm (THT)                                                      | [Link](https://www.digikey.com/en/products/detail/american-bright-optoelectronics-corporation/BL-B5134/20506048)                |
| 11   | LED3              | 1   | LED ORANGE                      | or other color                                                                                                                                                                                                                                       | LED D5.0 mm (THT)                                                      | [Link](https://www.digikey.com/en/products/detail/rohm-semiconductor/SLR-56DUT32/2337242)                                       |
| 12   | LED4              | 1   | LED YELLOW                      | or other color                                                                                                                                                                                                                                       | LED D5.0 mm (THT)                                                      | [Link](https://www.digikey.com/en/products/detail/american-bright-optoelectronics-corporation/BL-B3134/20506076)                |
| 13   | LED5              | 1   | LED GREEN                       | or other color                                                                                                                                                                                                                                       | LED D5.0 mm (THT)                                                      | [Link](https://www.digikey.com/en/products/detail/american-bright-optoelectronics-corporation/BL-B2134/20505921)                |
| 14   | LED6              | 1   | LED BLUE                        | or other color                                                                                                                                                                                                                                       | LED D5.0 mm (THT)                                                      | [Link](https://www.digikey.com/en/products/detail/lumimax-optoelectronic-technology/LED5BLU-D/25881229)                         |
| 15   | LED8              | 1   | LED RED Power                   | or other color                                                                                                                                                                                                                                       | LED D5.0 mm (THT)                                                      | [Link](https://www.digikey.com/en/products/detail/american-bright-optoelectronics-corporation/BL-B5134/20506048)                |
| 16   | R1,R6             | 2   | Resistor 10 kΩ                  |                                                                                                                                                                                                                                                      | Resistor Axial DIN0204 L3.6 mm D1.6 mm P5.08 mm Horizontal 1/4 W (THT) | [Link](https://www.digikey.com/en/products/detail/stackpole-electronics-inc/RNMF14FAD10K0/1683413,~)                            |
| 17   | R2,R3,R4          | 3   | Resistor 3.3 kΩ                 |                                                                                                                                                                                                                                                      | Resistor Axial DIN0204 L3.6 mm D1.6 mm P5.08 mm Horizontal 1/4 W (THT) | [Link](https://www.digikey.com/en/products/detail/stackpole-electronics-inc/RNMF14FTC3K30/2617342)                              |
| 18   | R5                | 1   | Resistor 56 Ω                   |                                                                                                                                                                                                                                                      | Resistor Axial DIN0204 L3.6 mm D1.6 mm P5.08 mm Horizontal 1/4 W (THT) | [Link](https://www.digikey.com/en/products/detail/stackpole-electronics-inc/RNMF14FTC56R0/2617362)                              |
| 19   | R7                | 1   | Resistor 2 kΩ                   |                                                                                                                                                                                                                                                      | Resistor Axial DIN0204 L3.6 mm D1.6 mm P5.08 mm Horizontal 1/4 W (THT) | [Link](https://www.digikey.com/en/products/detail/stackpole-electronics-inc/RNMF14FTC2K00/1683937)                              |
| 20   | SEG1–SEG7         | 7   | 7‑Segment LED SC39‑11EWA        | Best results with Kingbright                                                                                                                                                                                                                         | LED Display 7‑segment (Sx39‑1xxxxx) CC (THT)                           | [Link](https://www.digikey.com/en/products/detail/kingbright/SC39-11EWA/3084564)                                                |
| 21   | SW1               | 1   | Reset Button                    |                                                                                                                                                                                                                                                      | Button Switch PUSH 6 mm H4.3 mm (MJTP1230) (THT)                       | [Link](https://www.digikey.com/en/products/detail/apem-inc/MJTP1230/1798037)                                                    |
| 22   | SW2               | 1   | DIP Switch On/Off               |                                                                                                                                                                                                                                                      | DIP Switch SPSTx01 Slide 6.7×4.1 mm W7.62 mm P2.54 mm (THT)            | [Link](https://www2.mouser.com/ProductDetail/Wurth-Elektronik/418127270901?qs=wr8lucFkNMUHAgaqq%2FoMmA%3D%3D)                   |
| 23   | U1                | 1   | 27C256 EPROM                    | alternative W27E257                                                                                                                                                                                                                                  | Package DIP‑28 W15.24 mm socket (THT)                                  | [Link](https://www.digikey.com/en/products/detail/microchip-technology/AT27C256R-70PC/304743)                                   |
| 24   | U2                | 1   | IC CPU W65C02S (DIP‑40)         | microprocessor                                                                                                                                                                                                                                       | Package DIP‑40 W15.24 mm socket (THT)                                  | [Link](https://www.westerndesigncenter.com/wdc/documentation/w65c02s.pdf)                                                       |
| 25   | U3                | 1   | IC 74HC139 (SOP‑16)             |                                                                                                                                                                                                                                                      | Package SOP‑16 4.4×10.4 mm P1.27 mm (SMD)                              | [Link](https://www.digikey.com/en/products/detail/nexperia-usa-inc/74AHC139PW-Q100J/4020140)                                    |
| 26   | U4                | 1   | IC CY62256N SRAM 32 KB (SOP‑28) | SRAM 32 KB                                                                                                                                                                                                                                           | Package SOP‑28 8.4×18.16 mm P1.27 mm (SMD)                             | [Link](https://www.digikey.com/en/products/detail/rochester-electronics-llc/CY62256NLL-70ZC/12099783)                           |
| 27   | U5                | 1   | IC MAX690xPA (DIP‑8)            | MAX690 or MAX692                                                                                                                                                                                                                                     | Package DIP‑8 W7.62 mm (THT)                                           | [Link](https://www.digikey.com/en/products/detail/analog-devices-inc-maxim-integrated/MAX694CPA/948163)                         |
| 28   | U6,U7             | 2   | IC 74HC273 (SOIC‑20)            |                                                                                                                                                                                                                                                      | Package SOIC‑20W 7.5×12.8 mm P1.27 mm (SMD)                            | [Link](https://www.digikey.com/en/products/detail/toshiba-semiconductor-and-storage/74HC273D/6198939)                           |
| 29   | X1                | 1   | Oscillator 2 MHz (DIP‑14)       |                                                                                                                                                                                                                                                      | Oscillator DIP‑14 (THT)                                                | [Link](https://www.digikey.com/en/products/detail/cts-frequency-controls/MXO45-3C-2M000000/1801885) |

#### Notes

For **U1** and **U2** it’s recommended to use sockets.

---

## Assembly

Check the parts list to make sure you have everything. For assembly you’ll need a **soldering iron**, **solder**, and **flux** (for the SMD ICs). Ideally also have **flush cutters**, a **desoldering pump**, and **desoldering braid** at hand.

**Recommended order:**

1. **Solder SMD ICs:** U3 (74HC139), U6/U7 (74HC273), then U4 (SRAM).  
   Tip: Put a tiny drop of flux on pin 1 (top left) and the last pin (bottom right), align the IC, and tack those two pins with a small amount of solder. Once aligned, solder the remaining pins one by one using flux and little solder. **Mind the orientation**: Pin 1 is where the arrow/marker on the PCB points.
2. **Insert and solder sockets:** for U1 (EPROM) and U2 (W65C02S).
3. **Solder U5 (MAX690).**
4. **Insert oscillator X1 (2 MHz)** as the clock source.
5. **Populate diodes D1–D3 (1N5817).**
6. **Populate resistors R1–R7.**
7. **Populate ceramic capacitors C1, C4–C8.**
8. **Populate electrolytic capacitors C2, C3 (470 µF, 10–16 V).**
9. **Insert push‑button SW1 (Reset)** and **DIP switch SW2 (ON/OFF).**
10. **Install LED row LED1–LED7** and **LED8 (power LED).** **Observe polarity!** The hole with the square pad is the **cathode**.
11. **Mount J1 – DC/DC Step‑Up 5 V (10.5×11)** on the **back** of the PCB. Use 3‑pin **male‑male pin headers**. **Observe orientation:** The inductor of the step‑up module must face the back of the PCB.  
    **Without the step‑up module:** Bridge pin 1 and pin 3 at **J1** (do not connect to pin 2). **Only recommended** if the badge is powered from **stable 5 V** (bench PSU or USB‑C power bank).
12. **Connect J2 – CH340N SOP‑8 USB‑to‑TTL module** on the **back** via a **5‑pin male‑male header**. **Observe orientation.**
13. **Clean the PCB** (remove flux residues after soldering).
14. Verify that all parts **except** the 7‑segment displays are mounted.
15. **Insert the 7‑segment displays (SEG1–SEG7).** **Observe orientation:** There’s a small dot at bottom right—on the front, this dot must point **downwards**.
16. **Mount battery holders BT1 and BT2** (if desired). **Do not insert batteries/cells yet.**  
    **Caution:** Use **only 3× AA NiCd 1.2 V** as rechargeable cells! The charge circuit is very simple. **Do not** use Li‑ion or NiMH—fire/explosion hazard! When using **disposable batteries**, disable charging (**open JP2**).
17. **Insert U2 (W65C02S CPU)** and the **programmed U1 (EPROM).**
18. Congrats—the **MOS 6502 50th Anniversary Computer Badge** is assembled!

---

## Jumper Options

The **MOS 6502 50th Anniversary Computer Badge** has **two** jumpers for configuration.

1. **JP1 – CPU type**  
   Default: **open** → for **W65C02S** (Western Design Center). This CPU is still manufactured and easy to source. On the W65C02S, pin 1 outputs **VPB (Vector Pull)** and **must not** be tied permanently to GND.  
   Older CPU types by **MOS**, **Rockwell**, **UMC**, or **Synertek** need a GND connection here to work → **close JP1**.  
   **Note:** Use **2 MHz variants** (e.g., MOS 6502**AD**, Rockwell R6502**AP**, UMC UM6502**A**). The circuit has been tested with **W65C02S**. **CMOS** variants (65**C**02) are preferred for lower power.
2. **JP2 – Charging the AA NiCd cells**  
   Default: **closed**.  
   If you use **regular 3× AA 1.5 V batteries**, **JP2 must be opened**, so they won’t be (accidentally) charged by external power (USB‑C on **J2** or the pin header **J3**).

---

## Bring it to Life!

1. Set **SW2 to OFF**.  
2. Connect **5 V** to **J2 (USB‑C/CH340N)** or **J3 (pin header)** (**observe polarity!**).  
3. Set **SW2 to ON** → the **power LED** turns on and the 7‑segment displays show the default scrolling message **“6502 badge for VCF”** or **“6502 50th Birthday 1975–2025.”**

**Test on battery power:**  

- **SW2 OFF**, disconnect external 5 V.  
- Insert the **CR2032** for SRAM backup and **3× AA NiCd cells**.  
- On battery power, the power LED stays off while **SW2 is OFF**.  
- **SW2 ON** → the computer starts; the scrolling text appears.

When you then reconnect an external **5 V** source via **USB‑C (J2)** or **J3**, the **NiCd cells are slowly charged**. A full charge takes around **6–8 h**. **Runtime** with full cells is about **6–12 h**, depending on the series resistors (LED brightness).

The PCB has **four mounting holes**. You can attach standoffs or mount the board in an **enclosure**.

<img src="images/Lanyards.jpg" alt="Lanyard for the MOS 6502 Badge" title="Lanyard – MOS 6502 50th Anniversary Computer Badge (1975–2025)" width="700" />

Short Video on Youtube: [YouTube Short Video](https://www.youtube.com/shorts/PbgMO4NnUvw)

A nice extra is the **lanyard**, which you can attach to the two top holes—so you can wear the **MOS 6502 50th Anniversary Computer Badge** around your neck.

---

## Schematic

Download **Schematic** (PCB & display) ⇒ **[Schematic.pdf](downloads/Schematic.pdf)** (PDF, 0.2 MB)

<img src="images/Schematic_PCB_2.0b.png" alt="Schematic PCB" title="Schematic PCB" width="420" />  
<img src="images/Schematic_Display_2.0b.png" alt="Schematic Display" title="Schematic Display" width="420" />

The **MOS 6502 50th Anniversary Computer Badge** is a complete minimalist computer: 6502 CPU at **2 MHz**, **32 KB RAM (U4)**, and **32 KB ROM (U1)**. **U3** forms the **addressing logic** for RAM/ROM (**CS**) as well as the drive logic for the LED segments. The two **74HC273 (U6/U7)** act as latches/flip‑flops for the LEDs and the 7‑segment display. **Bit 7** is additionally used as the **TX signal** for the serial interface.

**RX** uses **pin 4 (IRQ)** of the 6502 (U2). This is a **software RS‑232**; the **OS in ROM** handles it. Thus, no separate UART is required. The RS‑232 link runs at **9600 baud, 8N1**. The serial connection is via the **CH340N SOP‑8 USB‑to‑TTL module (J2)**. Once connected to a PC, a **new COM port** appears; communicate with **9600,8N1** using e.g. **PuTTY** or **minicom**. On Windows you may need a driver: <https://www.arduined.eu/tag/ch340/>.

---

## Memory Map (RAM/ROM)

Badge RAM (32 KB) starts at **$0000** and extends to **$7FFF**.

| Area | Start | End                |
| ----:|:-----:|:------------------ |
| ROM  | 8000h | FFFFh – 32 KB (U1) |
| RAM  | 0000h | 7FFFh – 32 KB      |

---

## Input / Output

The two **74HC273 8‑bit latches (U6/U7)** control I/O. They share a common clock derived from a **memory write pulse (R/W)** into the ROM address space. All 8 **data bus lines** and the low 8 **address bus lines** are latched whenever a **write** to **$8000–$FFFF** occurs. These latches drive the **8 rows** and **7 columns** of the multiplexed LEDs and 7‑segment displays. The schematic shows the logical data and address bus connections. In practice, the address and data pins are intermixed between the two latches to simplify the PCB layout. The important point is that each input connects to the matching output: **D0→D0, D5→D5, A4→A4**, etc.

![Input‑Output Schematics](images/Input-Output-Schema.png "Input‑Output Schematics")

This design meets several conflicting requirements:

- With a single instruction, all **15 LED output bits** can be updated simultaneously (flicker‑free display).
- Minimal hardware (no separate UART).
- Simpler, smaller PCB layout.

**Bit 7** of the **data latch** isn’t needed for the LEDs and is therefore used for **serial output (TX)**. The CPU’s **IRQ pin** serves as **serial input (RX)**. Together with software, this yields a simple, minimalist, interrupt‑driven serial port for I/O. The **system monitor** and **BASIC interpreter** are exposed over this port.

---

## LED Display

The **data‑bus latches** drive the **LED anodes (segments)**, the **address‑bus latches** drive the **LED cathodes (digits)**.  
Data‑latch bits **0–6** select the LED segments (A–G). Since the digits have only 7 segments, **bit 7** is used for the serial port’s **TxD**.

Address‑latch bits **1–7** select the common cathodes of each of the 7 digits. Because there are only 7 digits, **address bit 0** selects the cathodes of the **7 discrete LEDs**. See the schematic for mapping.

Anode signals are **active high**, cathode signals are **active low**.  
Example: To turn on segment **A** of the **leftmost digit** → **data bit 3 = high** and **address bit 1 = low**. You achieve this by writing the value **$08** to address **$80FD**.

Breakdown:

```
; Data bits
76543210
00001000 = 08h

; Address bits
76543210
11111101 = FDh
```

To write the latches, write anywhere into the ROM region **$8000–$FFFF**. Add **$8000** to address **$00FD** → **$80FD**. (Writing to **$95FD** or **$FEFD** has the same effect—any address ≥ **$8000** works.)

---

## Serial Port

The serial port is **TTL‑level asynchronous**: **TX**, **RX**, and **GND**. It resembles **RS‑232**, but uses **5 V/0 V logic levels** with **non‑inverted** data (idle = 5 V = 1). Therefore, you can either use a **TTL‑to‑RS‑232 adapter** on **J3**, or plug in the **CH340N USB‑to‑TTL module (J2)** and use it as a USB serial adapter (supported by most systems). Bonus: **5 V** from USB powers the board and **charges** NiCd cells (if present and **JP2 is closed**).

**Configuration:** `9600, N, 8, 1` (9600 baud, no parity, 8 data bits, 1 stop bit).

**TX write:** Set/clear bit 7 → write `00h` (TX=0) or `80h` (TX=1) to **any** address **≥ $8000**.  
**Turn all LEDs off:** write to any address ≥ **$8000** with a **low byte of `FFh`** (e.g., **$80FF**), which makes all 8 cathodes high (inactive).  
**Hold LED state:** buffer LED data and address values in RAM.

**RX read:** **IRQ pin 4** senses **low levels** directly; high levels are detected via precise **timing loops**. The RX signal is **inverted** by **U3** so that processing is **RS‑232‑conformant**.

**Terminal program:** On Windows use **PuTTY** (COM port), on Linux **minicom**/`miniterm`. For **copy & paste** of source code set **send delays** (not all terminals support this):

1. Delay when sending a **byte**: **50 ms**  
2. Delay after **LF/CR**: **500 ms**

Since this is a **software‑based** serial interface without a FIFO, transmissions that are too fast will cause **timing issues** and **errors**.

---

## Software Overview

On power‑up/reset the 6502 jumps via the reset vector (16‑bit value at **$FFFC/$FFFD**) into the reset routine. This initializes the **LED display** and **software serial**, then branches into the **machine language monitor**.

The monitor runs via the **serial port** at **9600, N, 8, 1** and simultaneously creates a **scrolling message** on the seven LED digits (default: “6502 badge for VCF” or “6502 50th Birthday 1975–2025”). The seven **discrete LEDs** run a **Knight‑Rider** pattern. While waiting for serial input, the display is continuously updated.

---

## 6502 Badge – Monitor & Reference Guide

Entering `?` + `<Return>` shows the help screen:

<img src="images/OS_Monitor.png" title="Monitor Help Screen" alt="Screenshot: Monitor Help" width="700" />

### Monitor Commands

Basic command‑line format:

```
SSSS.EEEE C <Return>
```

- `SSSS` / `EEEE` = start/end address (separated by a dot)  
- `C` = **command symbol** (non‑alphanumeric)  
- `<Return>` = Enter key  
  **Note:** No spaces between these elements (e.g., `1234.5678L<Return>`).

Addresses can be 1–2 bytes (2–4 hex digits). If more than 4 hex digits are entered, the monitor takes only the **last 4** (e.g., from `1A2B3C.4D5E6C` it uses `2B3C` and `5E6C`). Shorter inputs are left‑padded with `0`; thus `0.3FF` covers `$0000–$03FF`.

For some commands the address is optional. The monitor remembers the **last entered** hex value and **increments** it automatically if no new address follows. Example:

- `1000L<Return>` disassembles **20 lines** starting at `$1000`.  
- A following `L<Return>` continues where it left off.  
- `1000LLL<Return>` thus shows **60 lines** from `$1000`.

`?<Return>` shows a short help:

```
Commands are :
Syntax = {} required, [] optional, HHHH hex address, DD hex data

[HHHH][ HHHH]{Return}         - Hex dump address(es) (up to 16 with no address)
[HHHH]{.HHHH}{Return}         - Hex dump range (16 per line)
[HHHH]{:DD}[ DD]{Return}      - Change data bytes
[HHHH]{G}{Return}             - Execute program (RTS returns to monitor)
{HHHH.HHHH>HHHHI}{Return}     - Insert (2nd) down into 1st→3rd
[HHHH]{L}{Return}             - Disassemble 20 lines
[HHHH]{.HHHH}{L}{Return}      - Disassemble range
{HHHH.HHHH>HHHHM}{Return}     - Move range (1st→2nd) to 3rd
{HHHH}[ HHHH]{Q}{Return}      - Text dump address(es)
[HHHH]{.HHHH}{Q}{Return}      - Text dump range (16/line)
{S}[up to 32 text chars]{Return} - Set LED message
[HHHH]{U}{Return}             - Upload (PC→SBC, XMODEM/CRC)
[HHHH.HHHH]{X}{Return}        - Download (SBC→PC, XMODEM/CRC)
{V}{Return}                   - Monitor version
{P*}{Return}                  - Protected shutdown
{!}{Return}                   - Mini‑assembler
{@}{Return}                   - EhBASIC cold start
{#}{Return}                   - EhBASIC warm start
{?}{Return}                   - Show help
```

### Hex Dump

```
[HHHH][ HHHH]<Return>   - Hex dump address(es) (up to 16 with no address)
[HHHH]{.HHHH}<Return>   - Hex dump range (16 per line)
```

Shows raw memory contents in hex.

**Variants:**

1. **Start address only** → only that byte (multiple addresses separated by spaces).  
2. **Start–End** → range, shown in 16‑byte lines (starts aligned on `$xxx0`).  
3. **No address** → up to 16 bytes starting at the last remembered address.

Example `5.2D<Return>`:

```
0005 - 2D FF 06 - 42 55 7A 68 AE F5 5B FF
0010 - 7C FF 37 FF FF FC DF EF - 8F CB D7 FF FF 5F 19 76
0020 - 36 DA D4 5D EF F3 EA FF - EA E1 E3 65 4B FF
```

### Edit Memory

```
[HHHH]{:DD}[ DD]<Return>   - Change data bytes
```

Writes data into RAM. After the address comes a colon `:` and at least one data byte `DD` (more bytes separated by spaces; written consecutively).

Example: Set memory `$1000` to `$55` → `1000:55<Return>`.

Writes to ROM **don’t cause an error** but have no effect (on the badge they affect the **I/O latches**—see above).

### Move Memory

```
{SSSS.EEEE>DDDDM}<Return>
```

Copies memory **from** `SSSS` **to** `EEEE` **into** `DDDD` (forward).

Handy trick to **fill** a region: First set the first byte with *Edit Memory*, then use *Move* to fill the rest.

Example: Fill `$1000–$1FFF` with `$00`:

```
1000:00<Return>
1000.1FFE>1001M<Return>
```

**Caution:** If `DDDD` lies within `SSSS–EEEE`, source data will be overwritten. Use **Insert Memory** if needed.

### Insert Memory

```
{SSSS.EEEE>DDDDI}<Return>
```

Like *Move*, but **backwards** (copies starting at `EEEE` downwards). This can create gaps of any size within a region. If `DDDD` lies outside, both variants work.

### Execute

```
[HHHH]{G}<Return>
```

Starts a machine program. An `RTS` (`$60`) returns to the monitor. Without an address, the last stored one is used—but giving an **explicit start address** is recommended (e.g., `1000G<Return>`).

### Disassemble (List)

```
[HHHH]{L}<Return>          - 20 lines
[HHHH]{.HHHH}{L}<Return>   - range
```

Without an address: 20 lines from the last address. Example:

```
>FF00L

FF00-  x    78         SEI  
FF01-  X    D8         CLD  
FF02-  ".   A2 FF      LDX  #$FF
...
FF25-  )h   A9 E8      LDA  #$E8
>
```

Format: address – ASCII of bytes (non‑printables → `.`) – hex values – mnemonic + operands.

### Text Dump

```
{HHHH}[ HHHH]{Q}<Return>
[HHHH]{.HHHH}{Q}<Return>
```

Like *Hex Dump*, but as **ASCII**. Useful to find text blocks in memory. Non‑printable characters → `.`

### Set LED Text

```
{S}[up to 32 chars]<Return>
```

Sets the scrolling LED message (32‑byte buffer; longer input is truncated). Example: `S6502 badge<Return>` shows:

```
6502 badge
```

### Upload (XMODEM)

```
[HHHH]{U}<Return>  – Upload from PC to badge (XMODEM/CRC)
```

The file is stored starting at the specified (or last remembered) address. **Note:** Due to the 128‑byte buffer, up to **127** extra bytes may be appended—avoid overwriting. Only **XMODEM/CRC** is supported (no checksum/1k mode).

### Download (XMODEM)

```
[HHHH.HHHH]{X}<Return> – Download from badge to PC (XMODEM/CRC)
```

Sends the specified range. Always provide addresses if possible (same 128‑byte buffer considerations). Only **XMODEM/CRC**.

### Show Version

```
{V}<Return>
```

Example:

```
>V
65C02 Monitor v5.2 (5-27-17) Ready
with Enhanced Basic Interpreter (c) Lee Davison
(Press ? for help)
>
```

### Protected Shutdown

```
{P*}<Return>
```

Turns off the LEDs and jumps into an endless loop in ROM. This keeps **RAM contents** intact before powering off.

### Mini‑Assembler

```
{!}<Return>   – Enter assembler
```

Simple RAM assembler (hex operands, no labels/arithmetic). Prompt changes from `>` to `!`. Help (`!?`) shows:

```
HHHH=hex address, OPC=Opcode, DD=hex data, '_'=Space/Tab
'$' optional, all HEX. Anything after ';' is ignored.

{HHHH}{Return}                      - Set input address
[HHHH][_]{OPC}[_][#($DD_HHHH,X),Y]{Return} - Assemble one line
[HHHH]{L}{Return}                   - Disassemble 20 lines
{Return}                            - Leave assembler
{?}{Return}                         - Help menu
```

Supported mnemonics include: `ADC AND ASL BCC ... WAI STP BBRx BBSx RMBx SMBx .DB .DW .DS`.  
**Note:** WDC opcodes (`WAI`, `STP`, `BBRx/BBSx`, `RMBx/SMBx`) are **not available** on the badge CPU, but the assembler accepts them; see the WDC manual. Pseudo‑opcodes:

- `.DB HH`   – store 1 byte  
- `.DW HHHH` – store 2 bytes (low byte first)  
- `.DS 'text'` – store ASCII string

**Example session (excerpt):**

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

The `^` marker indicates an error (e.g., branch target out of range).

---

## EhBASIC: Cold Start & Warm Start

**Cold start** `{@}<Return>` initializes RAM and sets the upper limit (“top of memory”). Input is **decimal**:

- `2048` → 2 KB RAM
- `32768` → 32 KB RAM

Example (2 KB RAM):

```
>@
Memory size ? 2048
1023 Bytes free
Enhanced BASIC 2.22

Ready
```

The first 1 KB of RAM is used by the monitor & LED display; thus with 2 KB total you get ≈ 1 KB free. Use `SYS<Return>` (new) to return from the EhBASIC prompt to the monitor.

**Warm start** `{#}<Return>` returns to EhBASIC after `SYS` (no re‑initialization; the RAM program remains).

---

## EhBASIC Quick Reference & Keywords

EhBASIC by **Lee Davison** (adapted here with permission). Manual: `http://www.sunrise-ev.com/photos/6502/EhBASIC-manual.pdf`. The source is thoroughly commented.

**Keyword list (excerpt):**  
`ABS AND ASC ATN BIN$ BITCLR BITSET BITTST CALL CHR$ CLEAR CONT COS DATA DEC DEEK DEF DIM DO DOKE ELSE END EOR EXP FN FOR FRE GET GOSUB GOTO HEX$ IF INC INPUT INT IRQ LCASE$ LEFT$ LEN LET LIST LOAD LOG LOOP MAX MID$ MIN NEW NEXT NMI NOT NULL OFF ON OR PEEK PI POKE POS PRINT READ REM RESTORE RETIRQ RETNMI RETURN RIGHT$ RND RUN SADD SAVE SGN SIN SPC( SQR STEP STOP STR$ SWAP SYS TAB( TAN THEN TO TWOPI UCASE$ UNTIL USR VAL VARPTR WAIT WHILE WIDTH + - * / ^ << >> > = <`

- Keywords **UPPERCASE** and **no spaces**.  
- Numbers: integer, decimal, or float; prefix `$` (hex) or `%` (binary). Examples: `$0A`, `1`, `-142`, `96.3`, `2.718E-3`.  
- Variables: numeric, `strings$`, or arrays `(n)`; strings in quotes (`"Hello world"`).

---

## LED Operation

The monitor contains routines to **refresh** the scrolling **7‑segment digits** and the **discrete LEDs**.  
Principle: Set the address latch to the first digit → fetch bit pattern from RAM → write to buffer → briefly enable → next digit. Repeat cyclically (**persistence of vision**).  
For **scrolling**, the start pointer is periodically shifted; speed follows from the number of refresh cycles between shifts. While waiting for input (monitor/EhBASIC), the display runs smoothly; when receiving characters there are brief interruptions.

**Sources:** `LEDdrive.asm`, `font.asm`.

**Important RAM addresses:**

```
Lbuff   = $02A0 ; LED text buffer (max. 32 bytes)
LDbuff  = $02C0 ; discrete LED buffer (max. 32 bits)
Lptr    = $E2   ; LED pointer (0..31)
Ldig    = $E3   ; digit counter (0..7; 0 = discrete LEDs)
Lscn    = $E4   ; scan delay (brightness/flicker) – 0..255, 0 = display refresh off
Lscl    = $E5   ; scroll delay – 0..255, 0 = static
Lscnc   = $E6   ; scan counter (counts down from Lscn)
Lsclc   = $E7   ; scroll counter (counts down from Lscl)
LEDchk1 = $E8   ; config checksum 1
LEDchk2 = $E9   ; config checksum 2
```

`Lbuff`/`LDbuff` are **synchronized** (position 0..31). Set `Lscn=$00` to disable the monitor refresh (for custom LED code).  
`LEDchk1=$A5` **and** `LEDchk2=$5A` prevent the buffers from being overwritten on reset (otherwise default text “6502 badge for VCF” + “Knight Rider”). You can set these flags with *Edit Memory*.

---

## Serial I/O (ROM Routines)

There are three monitor subroutines for serial I/O (call via `JSR`). **Note:** There are two monitor ROM versions; use addresses depending on the version date (`V` command):

- **Serial_Output** (`$EAE8` *or* `$EAEC`) – sends 1 byte (in the accumulator); `X/Y` unchanged.
  
  ```asm
  ; 5-17-17 ROM          ; 2-24-18 ROM
  LDA #$41               LDA #$41   ; ASCII "A"
  JSR $EAE8              JSR $EAEC  ; send
  ```

- **Serial_Input** (`$EB35` *or* `$EB39`) – blocking read; byte in A; `X/Y` unchanged; `Z/N` flags set.
  
  ```asm
  JSR $EB35              JSR $EB39  ; get char
  STA $400               STA $400   ; store
  JSR $EAE8              JSR $EAEC  ; echo
  ```

- **Scan_Input** (`$EB4C` *or* `$EB50`) – non‑blocking; no input → carry **clear**; input: byte in A, `Z/N` set, carry **set**.
  
  ```asm
  Loop  JSR $EB4C        JSR $EB50  ; check
        BCC Loop         BCC Loop   ; none → again
        BMI Loop         BMI Loop   ; >$7F? (N=1) → again
        STA $400         STA $400   ; store
  ```

---

## System Memory Usage

The following areas are used by the system. Whether overwriting is acceptable is up to you; study the sources.

### Zero Page

| Range     | Use               |
| ---------:| ----------------- |
| `$00–$13` | EhBASIC           |
| `$14–$31` | free              |
| `$32–$3F` | monitor variables |
| `$40–$5A` | free              |
| `$5B–$DF` | EhBASIC           |
| `$E2–$E9` | LED driver        |
| `$EA–$ED` | serial driver     |
| `$EF–$FF` | EhBASIC           |

### RAM

| Range         | Use                                    |
| -------------:| -------------------------------------- |
| `$0100–$01FF` | system stack                           |
| `$0200–$027F` | serial receive ring buffer             |
| `$02A0–$02DF` | LED buffer                             |
| `$0300–$037F` | monitor input buffer                   |
| `$0390–$03FF` | EhBASIC input buffer                   |
| `$0400–$7FFF` | user RAM / EhBASIC program (32 KB RAM) |

### ROM (depending on monitor date)

| **5‑17‑17 ROM** | **2‑24‑18 ROM** | Description               |
| ---------------:| ---------------:| ------------------------- |
| `$C000–$C1FF`   | `$C000–$C1FF`   | CRC lookup table (XMODEM) |
| `$C200–$EA9B`   | `$C200–$EA9F`   | EhBASIC                   |
| `$EA9C–$EB64`   | `$EAA0–$EB68`   | serial I/O routines       |
| `$EB65–$FC39`   | `$EB69–$FC3D`   | monitor                   |
| `$FC3A–$FD93`   | `$FC3E–$FD97`   | LED support               |
| `$FD94–$FFBE`   | `$FD98–$FFC2`   | XMODEM                    |
| `$FFBF–$FFFF`   | `$FFC3–$FFFF`   | reset code & vectors      |

---

## Source Code Organization & Build Notes

With the exception of EhBASIC, the software is by **Daryl Rictor**. Use and adaptation for **non‑commercial** purposes is permitted.

**Files:**

- `sbc.asm` – “makefile”: includes all sources at the proper order/addresses  
- `basic.asm` – EhBASIC source  
- `basldsv.asm` – patch for load/save via XMODEM  
- `sbcOS.asm` – monitor incl. disassembler & mini‑assembler  
- `serial.asm` – software serial driver  
- `LEDdrive.asm` – LED driver (refresh, scroll, text)  
- `font.asm` – LED font (ASCII→latch pins)  
- `xmodem.asm` – XMODEM protocol  
- `CRCtable.asm` – CRC lookup table  
- `reset.asm` – reset/initialization; ROM vectors `$FFFA–$FFFF`; BRK handler (`$00`) → reset & monitor

**Assembling (6502 Macroassembler & Simulator, `6502.exe`):**

1. Launch the program  
2. Open `sbc.asm` (`File → Open → sbc.asm`)  
3. Options:  
   - `Assembler` → **Extra byte after BRK**: **disabled**  
   - `General` → select **65C02, 6501**  
4. Assemble (`F7`)  
5. Save object (`File → Save Code`): Intel‑Hex, S‑Record, or binary  
   - **Start address**: `0xC000` (16 KB ROM) **or** `0x8000` (32 KB ROM)  
   - **End address**: `0xFFFF`  
   - **OK** → **SAVE**

---

## Downloads / Firmware / Manuals

1. Adjusted BadgeOS firmware **32 KB** (27C256, U1; 7× LEDs of the 50th version) ⇒ **[BadgeOS_32k_50th.rom](downloads/BadgeOS_32k_50th.rom)** (BIN, 32 KB)  
2. Original **BadgeOS** (firmware/ROM) ⇒ **[BadgeOS.zip](downloads/BadgeOS.zip)** (ZIP, 0.8 MB)  
3. Original **Badge Manual** by **Lee Hart, Daryl Rictor, and Josh Bensadon** ⇒ **[badge-manual.pdf](downloads/badge-manual.pdf)** (PDF, 1.6 MB)  
4. Original **EhBASIC Manual** ⇒ **[EhBASIC-manual.pdf](downloads/EhBASIC-manual.pdf)** (PDF, 0.5 MB)  
5. **Schematic** (PCB & display) ⇒ **[Schematic.pdf](downloads/Schematic.pdf)** (PDF, 0.2 MB)  
6. **PCB layout (Gerber)** ⇒ **[gerber/](gerber/)**  
7. **BOM files** ⇒ **[bom/](bom/)**  
8. Driver for **CH340 USB‑C to Serial TTL**: <https://www.arduined.eu/tag/ch340/>  
9. More downloads ⇒ **[downloads/](downloads/)**

---

## Ordering

Soon I will make this project available to everyone on **pcbway.com** as a **Shared Project**.

---

## Troubleshooting

1. **Power LED is on, LEDs/scrolling text flicker.**  
   Check whether **U2 pin 8** has a stable **4.5–5 V**. If the 5 V step‑up booster input is **< 1.2 V**, the voltage collapses and pulses.
2. **Some LEDs/7‑segment digits are dark or always on.**  
   Check **U6/U7 (74HC273)** for proper pin contact and possible **solder bridges**.
3. **Power LED is on, but nothing else works.**  
   (1) Inspect **U3 (74HC139)** for shorts/pins. (2) Check **U1 (EPROM)** and **U2 (microprocessor)** seating (and firmware!). (3) Check **U4 (SRAM)**. (4) Check **oscillator X1**.
4. **No USB connection (Windows).**  
   Install the **CH340 driver** (see downloads).

---

## Disclaimer

This is a non‑commercial hobby project. Building and using the **MOS 6502 – 50th Anniversary Computer Badge (1975–2025)** is entirely at your **own risk**. There is **no warranty** of any kind regarding function, safety, completeness, or freedom from errors. The author (Frank Eggen) assumes **no liability** for damages, losses, or consequential damages arising from building or using the project.

---

## Donations

I’ve invested many hours in this project. If you’d like to support the work, feel free to contribute to the **coffee fund**. Thanks a lot!  
👉 **[PayPal – Donate](https://www.paypal.com/donate/?cmd=_s-xclick&hosted_button_id=Q8HXKYARXKT4L&ssrt=1714757590172)**

---

## Acknowledgments

1. This project is based on the idea by **Lee Hart, Daryl Rictor, and Josh Bensadon**. 👉 Original project: <http://www.sunrise-ev.com/6502.htm>  
   Huge thanks to the original designers for their pioneering work—and especially to **Lee Hart** for many helpful tips during this rework. 🙏
2. **Chuck Peddle** and the team at **MOS** (incl. Terry Holdt, Wil Mathys, Rod Orgill, Harry Bawcom, Sydney Anne Holt, Walt Eisenhower, John Paivinen), whose vision made the 6502 possible: <https://www.team6502.org>
3. **Bill Mensch**, founder of the **Western Design Center**, who keeps the 6502 alive, documented, and evolving: <https://www.westerndesigncenter.com>
4. **Ben Eater** for his “Build a 6502 computer” project: <https://eater.net/6502>
