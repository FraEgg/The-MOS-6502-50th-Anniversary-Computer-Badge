# The MOS 6502 – 50th Anniversary Computer Badge (1975–2025)

## A Retro Computer in a Badge for 8‑bit 6502 Fans

By Frank Eggen

[<img src="images/Youtube.jpg" title="Watch on YouTube" alt="Watch on YouTube" style="zoom:50%;">](https://www.youtube.com/shorts/PbgMO4NnUvw)

---

Based on an idea by **Lee Hart, Daryl Rictor, and Josh Bensadon** (revived and updated).
👉 Original project: [sunrise-ev.com/6502.htm](http://www.sunrise-ev.com/6502.htm)

---

## Table of Contents

- [50 Years of the MOS 6502](#50-years-of-the-mos-6502)
- [What is the Computer Badge?](#what-is-the-computer-badge)
- [Variants](#variants)
- [What can you use it for?](#what-can-you-use-it-for)
- [Technical Specs at a Glance](#technical-specs-at-a-glance)
- [Bill of Materials (BOM)](#bill-of-materials-bom)
- [Assembly](#assembly)
- [Jumper Options](#jumper-options)
- [Power‑On & Demo](#poweron--demo)
- [Schematic](#schematic)
- [Memory Map](#memory-map)
- [Input / Output](#input--output)
- [LED Display](#led-display)
- [Serial Port](#serial-port)
- [Software Overview](#software-overview)
- [6502 Badge — Monitor & Reference Guide](#6502-badge--monitor--reference-guide)
  - [Monitor Commands](#monitor-commands)
  - [Hex Dump](#hex-dump)
  - [Edit Memory](#edit-memory)
  - [Move Memory](#move-memory)
  - [Insert Memory](#insert-memory)
  - [Execute](#execute)
  - [Disassemble](#disassemble)
  - [Text Dump](#text-dump)
  - [Set LED Text](#set-led-text)
  - [Upload (XMODEM)](#upload-xmodem)
  - [Download (XMODEM)](#download-xmodem)
  - [Show Version](#show-version)
  - [Protected Power Down](#protected-power-down)
  - [Mini‑Assembler](#mini-assembler)
  - [Help](#help)
- [EhBASIC: Cold & Warm Start](#ehbasic-cold--warm-start)
- [EhBASIC Quick Reference & Keywords](#ehbasic-quick-reference--keywords)
- [LED Operations](#led-operations)
- [Serial I/O Operations](#serial-io-operations)
- [System Memory Usage](#system-memory-usage)
- [Source Organization & Build Notes](#source-organization--build-notes)
- [Downloads / Firmware / Manuals](#downloads--firmware--manuals)
- [Ordering](#ordering)
- [Troubleshooting](#troubleshooting)
- [Disclaimer](#disclaimer)
- [Donations](#donations)
- [Acknowledgements](#acknowledgements)

---

## 50 Years of the MOS 6502

<img title="White Ceramic 6502 CPU Illustration" src="images/white-ceramic-6502-illustration.png" alt="white-ceramic-6502-illustration" data-align="center">

The legendary **MOS 6502** debuted in 1975 and changed computing forever. It delivered performance at a low price and powered the rise of **home computers**.

Famous 6502‑based systems:

* Apple II
* Commodore VIC‑20 & C64
* Nintendo NES
* BBC Micro
* Atari VCS

👉 Learn more: [team6502.org](https://www.team6502.org)

---

## What is the Computer Badge?

<img title="The MOS 6502 – 50th Anniversary Computer Badge (1975–2025)" src="images/The_MOS_6502–50th_Anniversary_Computer_Badge_Real.jpg" alt="The MOS 6502 – 50th Anniversary Computer Badge (1975–2025)" data-align="center" style="zoom:25%;">

The **MOS 6502 50th Anniversary Computer Badge** is a **minimalist re‑imagining** of an 8‑bit microcomputer with a 6502 CPU, redesigned with modern, easy‑to‑source parts—compact enough to wear like a retro name badge.

**Highlights:**

* **W65C02S microprocessor @ 2 MHz**
* **32 KB RAM** with battery backup
* **32 KB EPROM** with Floating‑Point BASIC + 6502 monitor
* **7‑digit 7‑segment LED display + 7 discrete LEDs** for effects
* **RS‑232‑compatible interface** for data exchange
* **USB‑C (CH340) serial TTL interface** – plug straight into your PC
* **DC/DC step‑up module** for stable battery operation
* **CR2032 coin cell** for SRAM data retention

> Fully functional, programmable in **assembler** or **BASIC**—and still small enough to wear as a retro badge.

---

## Variants

**Badge Version**

<img title="MOS 6502 50th Anniversary Computer Badge Render" src="images/PCB_Render_V2_Badge.png" alt="PCB MOS 6502 50th Anniversary Computer Badge Render Photo" style="zoom:50%;" data-align="center">

<img title="MOS 6502 50th Anniversary Computer Badge Layout" src="images/PCB_Layout_V2_Badge.png" alt="PCB MOS 6502 50th Anniversary Computer Badge Layout" style="zoom:33%;" data-align="center">

* 7.62 × 10.16 cm (3 × 4 in) – classic badge format  
* PCB layout (Gerber) download > [here](gerber/) <

---

## What can you use it for?

* As a **retro name badge** with a scrolling message of your choice
* To **celebrate 50 years of the 6502** & the home‑computer era
* As a **teaching project** for assembler, BASIC, and hardware nostalgia
* For **tinkering & fun** with a minimal part count
* Simply as a **cool collectible** for the anniversary

---

## Technical Specs at a Glance

* W65C02S @ 2 MHz
* 32 KB RAM with battery backup
* 32 KB EPROM (BASIC + monitor)
* 2× 8‑bit output latches
* 7‑digit 7‑segment LED display + 7 LEDs
* 9600 8‑N‑1 software RS‑232 serial interface
* USB‑C to TTL CH340 UART adapter (BTE17‑06B)
* DC/DC 5 V step‑up boost converter
* Charging support for 3× AA Ni‑Cd cells

👉 You get a **complete retro system** in your hand—minimalist, educational, and a head‑turner at any nerd meetup. 😎

---

## Bill of Materials (BOM)

_Created on 2025‑09‑20 19:50_

| Pos. | Ref               | Qty | Value                        | Notes                                                                                                                                                                                                                     | Description                                                 | Datasheet / Link                                                                                                 |
| ---- | ----------------- | --- | ---------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------- |
| 1    | BT1               | 1   | Battery Holder               | 3× AA Ni‑Cd cells (optional).<br/>**If you use disposable batteries, open JP2 (Charging); otherwise they will see charge voltage when external power is present. Use only Ni‑Cd cells for charging—fire risk otherwise!** | Holder Keystone 3×AA                                        | [Link](https://www.digikey.com/en/products/detail/keystone-electronics/106/27386)                                |
| 2    | BT2               | 1   | CR2032 Cell Holder           | CR2032                                                                                                                                                                                                                    | Battery Holder CR2032 Horizontal, circular holes            | [Link](https://www.digikey.com/en/products/detail/keystone-electronics/2464/303813)                              |
| 3    | C1,C4,C5,C6,C7,C8 | 6   | Capacitor 0.1 µF             |                                                                                                                                                                                                                           | Capacitor Disc D4.7 mm W2.5 mm P5.00 mm (THT)               | [Link](https://www.digikey.com/en/products/detail/kemet/C322C104M5U5TA/818107)                                   |
| 4    | C2,C3             | 2   | Capacitor 470 µF 10–16 V     |                                                                                                                                                                                                                           | Capacitor Radial D8.0 mm P3.50 mm (THT)                     | [Link](https://www.digikey.com/en/products/detail/rubycon/16ZLH470MEFC8X11-5/3563382)                            |
| 5    | D1,D2,D3          | 1   | Schottky Diode 1N5817        | **Install only D1!** D2 and D3 are for test purposes. **Bridge D2 and D3 with a wire.**                                                                                                                                   | Diode DO‑41 SOD81 P10.16 mm Horizontal (THT)                | [Link](https://www.digikey.com/en/products/detail/smc-diode-solutions/1N5817/21705460)                           |
| 6    | J1                | 1   | 5 V DC‑DC Step‑Up Module     |                                                                                                                                                                                                                           | Converter Step‑Up 5 V Module 10.5×11 (THT with pin header)  | [Link](https://de.aliexpress.com/item/1005005624977910.html)                                                     |
| 7    | J2                | 1   | CH340N SOP‑8 USB‑to‑TTL Mod. |                                                                                                                                                                                                                           | CH340N SOP‑8 USB‑to‑TTL Module (THT with pin header)        | [Link](https://de.aliexpress.com/item/1005009386863437.html)                                                     |
| 8    | J3                | 1   | Pin Header                   | (optional)                                                                                                                                                                                                                | Header 1×05 P2.54 mm Vertical (THT)                         | ~                                                                                                                |
| 9    | LED1,LED7         | 2   | LED WHITE                    | or other color                                                                                                                                                                                                            | LED D5.0 mm (THT)                                           | [Link](https://www.digikey.com/en/products/detail/seoul-semiconductor-inc/LW520AS/2770221)                       |
| 10   | LED2              | 1   | LED RED                      | or other color                                                                                                                                                                                                            | LED D5.0 mm (THT)                                           | [Link](https://www.digikey.com/en/products/detail/american-bright-optoelectronics-corporation/BL-B5134/20506048) |
| 11   | LED3              | 1   | LED ORANGE                   | or other color                                                                                                                                                                                                            | LED D5.0 mm (THT)                                           | [Link](https://www.digikey.com/en/products/detail/rohm-semiconductor/SLR-56DUT32/2337242)                        |
| 12   | LED4              | 1   | LED YELLOW                   | or other color                                                                                                                                                                                                            | LED D5.0 mm (THT)                                           | [Link](https://www.digikey.com/en/products/detail/american-bright-optoelectronics-corporation/BL-B3134/20506076) |
| 13   | LED5              | 1   | LED GREEN                    | or other color                                                                                                                                                                                                            | LED D5.0 mm (THT)                                           | [Link](https://www.digikey.com/en/products/detail/american-bright-optoelectronics-corporation/BL-B2134/20505921) |
| 14   | LED6              | 1   | LED BLUE                     | or other color                                                                                                                                                                                                            | LED D5.0 mm (THT)                                           | [Link](https://www.digikey.com/en/products/detail/lumimax-optoelectronic-technology/LED5BLU-D/25881229)          |
| 15   | LED8              | 1   | LED RED Power                | or other color                                                                                                                                                                                                            | LED D5.0 mm (THT)                                           | [Link](https://www.digikey.com/en/products/detail/american-bright-optoelectronics-corporation/BL-B5134/20506048) |
| 16   | R1,R6             | 2   | Resistor 10 kΩ               |                                                                                                                                                                                                                           | Resistor Axial DIN0204 L3.6 mm D1.6 mm P5.08 mm Hor. 1/4 W  | [Link](https://www.digikey.com/en/products/detail/stackpole-electronics-inc/RNMF14FAD10K0/1683413)               |
| 17   | R2,R3,R4          | 3   | Resistor 3.3 kΩ              |                                                                                                                                                                                                                           | Resistor Axial DIN0204 L3.6 mm D1.6 mm P5.08 mm Hor. 1/4 W  | [Link](https://www.digikey.com/en/products/detail/stackpole-electronics-inc/RNMF14FTC3K30/2617342)               |
| 18   | R5                | 1   | Resistor 56 Ω                |                                                                                                                                                                                                                           | Resistor Axial DIN0204 L3.6 mm D1.6 mm P5.08 mm Hor. 1/4 W  | [Link](https://www.digikey.com/en/products/detail/stackpole-electronics-inc/RNMF14FTC56R0/2617362)               |
| 19   | R7                | 1   | Resistor 2 kΩ                |                                                                                                                                                                                                                           | Resistor Axial DIN0204 L3.6 mm D1.6 mm P5.08 mm Hor. 1/4 W  | [Link](https://www.digikey.com/en/products/detail/stackpole-electronics-inc/CFM14JT560R/1742246)                 |
| 20   | SEG1–SEG7         | 7   | 7‑Segment LED SC39‑11EWA     | Best results with Kingbright                                                                                                                                                                                              | LED Display 7‑Segment (Sx39‑1xxxxx) CC (THT)                | [Link](https://www.digikey.com/en/products/detail/kingbright/SC39-11EWA/3084564)                                 |
| 21   | SW1               | 1   | Reset Button                 |                                                                                                                                                                                                                           | Push Button 6 mm H4.3 mm (MJTP1230) (THT)                   | [Link](https://www.digikey.com/en/products/detail/apem-inc/MJTP1230/1798037)                                     |
| 22   | SW2               | 1   | DIP Switch On/Off            |                                                                                                                                                                                                                           | DIP Switch SPSTx01 Slide 6.7×4.1 mm W7.62 mm P2.54 mm (THT) | [Link](https://www2.mouser.com/ProductDetail/Wurth-Elektronik/418127270901?qs=wr8lucFkNMUHAgaqq%2FoMmA%3D%3D)    |
| 23   | U1                | 1   | 27C256 EPROM                 | alt. W27E257                                                                                                                                                                                                              | Package DIP‑28 W15.24 mm Socket (THT)                       | [Link](https://www.digikey.com/en/products/detail/microchip-technology/AT27C256R-70PC/304743)                    |
| 24   | U2                | 1   | W65C02S CPU (DIP‑40)         | Microprocessor                                                                                                                                                                                                            | Package DIP‑40 W15.24 mm Socket (THT)                       | [WDC Datasheet](https://www.westerndesigncenter.com/wdc/documentation/w65c02s.pdf)                               |
| 25   | U3                | 1   | 74HC139 (SOP‑16)             |                                                                                                                                                                                                                           | Package SOP‑16 4.4×10.4 mm P1.27 mm (SMD)                   | [Link](https://www.digikey.com/en/products/detail/nexperia-usa-inc/74AHC139PW-Q100J/4020140)                     |
| 26   | U4                | 1   | CY62256N SRAM 32 KB (SOP‑28) | SRAM 32 KB                                                                                                                                                                                                                | Package SOP‑28 8.4×18.16 mm P1.27 mm (SMD)                  | [Link](https://www.digikey.com/en/products/detail/rochester-electronics-llc/CY62256NLL-70ZC/12099783)            |
| 27   | U5                | 1   | MAX690xPA (DIP‑8)            | MAX692xPA also usable                                                                                                                                                                                                     | Package DIP‑8 W7.62 mm (THT) <br/>MAX690 or MAX692          | [Link](https://www.digikey.com/en/products/detail/analog-devices-inc-maxim-integrated/MAX694CPA/948163)          |
| 28   | U6,U7             | 2   | 74HC273 (SOIC‑20)            |                                                                                                                                                                                                                           | Package SOIC‑20W 7.5×12.8 mm P1.27 mm (SMD)                 | [Link](https://www.digikey.com/en/products/detail/toshiba-semiconductor-and-storage/74HC273D/6198939)            |
| 29   | X1                | 1   | 2 MHz Oscillator (DIP‑14)    |                                                                                                                                                                                                                           | Oscillator DIP‑14 (THT)                                     | [Link](https://www.digikey.com/en/products/detail/cts-frequency-controls/MXO45-3C-2M000000/1801885)              |

**Notes:**  
Use DIP sockets for U1 and U2.

---

## Assembly

Check the parts list to make sure you have everything. For assembly you need a soldering iron, solder, and flux for the SMD ICs—plus tweezers, a solder sucker, and desoldering braid on hand.

I recommend this order:

1. **Solder the SMD ICs** onto the PCB: U3 (74HC139), U6 & U7 (74HC273), then U4 (SRAM). Everyone has their own SMD technique. I add a small drop of flux to pin 1 (top‑left) and the last pin (bottom‑right), align the IC on the pads, and tack those two pins with a touch of solder. Once aligned, add flux and solder the remaining pins one by one. **Make sure every IC is oriented correctly.** Pin 1 is where the board’s arrow points.
2. **Install the sockets** for U1 (EPROM) and U2 (W65C02S microprocessor).
3. **Solder U5** (MAX690 or MAX692).
4. **Install X1**, the 2 MHz oscillator (CPU clock).
5. **Add D1 (1N5817)**. **Install only D1!** D2 and D3 are for testing—**bridge D2 and D3 with a wire.**
6. **Solder the resistors R1–R7.**
7. **Solder the ceramic capacitors** C1, C4–C8.
8. **Install the electrolytic capacitors** C2, C3 (470 µF, 10–16 V).
9. **Mount SW1 (Reset)** and **SW2 (On/Off DIP)**.
10. **Place LEDs** LED1–LED7 (LED bar) and LED8 (Power). **Observe polarity!** The hole with the square pad is the **cathode**.
11. **Install J1**, the 5 V DC‑DC step‑up module. Use **3‑pin male‑male headers** and mount the module on the **back** of the PCB. Observe polarity. The inductor must face **away from** the PCB. If you **don’t** want to use the step‑up module, **bridge pins 1 and 3 at J1** (do **not** connect to pin 2). Only do this if the badge is powered from a **stable 5 V** source (bench supply or USB‑C power bank).
12. **Install J2**, the **CH340N SOP‑8 USB‑to‑TTL** module, on the back using a 5‑pin male‑male header. Again, check orientation.
13. **Clean the PCB** to remove flux residues.
14. At this point, everything except the **7‑segment displays** should be populated.
15. **Install the 7‑segment displays.** Observe orientation: there is a small dot bottom‑right—on the **front** side this dot must point **down**.
16. **Install the battery holders** BT1 and BT2 if needed, but **do not insert batteries yet**.  
    **Warning:** *Only use 3× AA **Ni‑Cd 1.2 V** cells!* The charger is very simple. **Do not** use Li‑ion or NiMH—this could cause fire or explosion. If you use disposable batteries, **disable charging** (open JP2).
17. Finally, **insert U2** (W65C02S CPU) and the **programmed U1** (EPROM).
18. Your **MOS 6502 50th Anniversary Computer Badge** is now assembled. 🎉

---

## Jumper Options

The badge has **three jumpers** for different configuration options.

1. **JP1** selects the CPU type. By default it’s **open**, configured for the **W65C02S** from Western Design Center (still in production and easy to obtain). On this CPU, pin 1 outputs **VPB (Vector Pull)** and **must not** be tied permanently to GND.  
   Older CPU types from MOS, Rockwell, UMC, or Synertek require **GND at pin 1**—close JP1 for those. When using other CPUs, choose a **2 MHz** variant: MOS **6502AD**, Rockwell **R6502AP**, UMC **UM6502A**. The circuit has only been tested with **W65C02S**, and I recommend a **CMOS** part over **NMOS** due to lower power. The badge OS uses the **extended CMOS instruction set**, so original NMOS 6502 would need a dedicated OS.
2. **JP2** controls charging of the AA **Ni‑Cd** cells and is **closed by default**. If you use **3× AA 1.5 V disposable batteries** instead of Ni‑Cd **rechargeables**, you **must open JP2** so they are not accidentally charged by external power (USB‑C J2 or header J3).

---

## Power‑On & Demo

Now for the big moment. Turn **SW2 to OFF**. Connect a **stable 5 V** power source via **J2** or the **J3** pin header, observing polarity. Then set **SW2 to ON**—the **power LED** should light and you should see the default scrolling text *“6502 badge for VCF”* or *“6502 50th Birthday 1975–2025”* on the **7‑segment displays**.

To test **battery operation**, turn **SW2 OFF** and disconnect external power. Insert a **CR2032** for SRAM retention and **3× AA Ni‑Cd** cells. Unlike external power, the power LED does **not** light in battery mode when **SW2 = OFF**. Turn **SW2 ON**—the computer should start and the scrolling text should appear again. Nice!

When you later connect external 5 V via **USB‑C (J2)** or **header J3**, the Ni‑Cd pack will **slowly charge**. A full charge takes **about 6–8 h**. Runtime with full cells is **~6–12 h**, depending on LED brightness (set by series resistors).

The PCB has **four mounting holes**. Use them for feet if you want to display the board on a desk or mount it in an enclosure.

![Lanyard](images/Lanyards.jpg "Lanyard — MOS 6502 - 50th Anniversary Computer Badge (1975–2025) - ATARI - APPLE - COMMODORE - NINTENDO - BBC MICRO")

Short video on YouTube: [[Go to YouTube](https://www.youtube.com/shorts/PbgMO4NnUvw)]

A bonus accessory is the **lanyard** that attaches to the top holes so you can wear the badge.

---

## Schematic

Schematic for **The MOS 6502 – 50th Anniversary Computer Badge (1975–2025)** > [here](downloads/Schematic.pdf) < (PDF, 0.2 MB)

<img title="Schematic PCB" src="images/Schematic_PCB_2.0b.png" alt="Schematic PCB" style="zoom:25%;" data-align="left"><img title="Schematic Display" src="images/Schematic_Display_2.0b.png" alt="Schematic Display" style="zoom:25%;" data-align="left">

The **badge** is a complete minimalist computer: a **6502 CPU** at **2 MHz** with **32 KB RAM (U4)** and **32 KB ROM (U1)**. **U3** provides address decode for RAM/ROM (CS) and drives the LED segments. The two **74HC273** (U6/U7) act as latches/flip‑flops to control the LEDs and 7‑segment display. **Bit 7** also serves as **TX** for the serial port.

For **RX**, the CPU’s **IRQ (pin 4)** is used. This is a **software serial** (soft‑RS‑232) link handled by the ROM OS, which avoids a separate UART chip. The serial port runs **9600 baud, 8‑N‑1**. The serial interface is connected to the **CH340N SOP‑8 USB‑to‑TTL** module at **J2**. When you connect it to a PC, a new **COM** (or tty) port appears for **9600, 8‑N‑1** with a terminal like **PuTTY** or **minicom**. On Windows you usually need a driver: <https://www.arduined.eu/tag/ch340/>.

---

## Memory Map

Badge memory: **32 KB RAM** starts at `$0000` through `$7FFF`.

| Address | Start | End                  |
| ------- | ----- | -------------------- |
| 8000h   | FFFFh | ROM 32 KB (EPROM U1) |
| 0000h   | 7FFFh | RAM 32 KB (SRAM U4)  |

---

## Input / Output

The two **74HC273** 8‑bit latches (U6/U7) handle I/O. They share a clock derived from a **write** (RW low) into the **ROM address space**. All **8 data** bus lines and the **low 8 address** lines are captured by the latches whenever you write to `$8000–$FFFF`. These latches drive the **8 rows** and **7 columns** of the multiplexed LEDs and 7‑segment digits. The schematic shows the logical D‑ and A‑bus mapping. In the PCB, address/data pins are interleaved between the latches to simplify routing—what matters is that **each input matches its output** (D0→D0, D5→D5, A4→A4, etc.).

![Input-Output Schema](images/Input-Output-Schema.png "Input-Output Schema")

This “crazy” setup meets several conflicting goals:

- Update all **15 LED control bits** at once with a single instruction (no flicker).
- Minimize hardware (no discrete UART).
- Simplify and shrink the PCB layout.

**Bit 7 of the data latch** isn’t needed for LEDs, so it’s used for **serial TX**. The CPU’s **IRQ** serves as **serial RX**. Together with software, this provides a simple, minimalist **interrupt‑driven** serial port for user I/O. A **system monitor** and **BASIC interpreter** are presented over this port.

---

## LED Display

The **data‑bus latch** drives the LED **anodes** (segments), the **address‑bus latch** drives the LED **cathodes** (digits).  
Data latch bits **0–6** select segments **A–G**. Because the digits have only 7 segments, **data bit 7** is used for **TxD**.  
Address latch bits **1–7** select the **7 digits** (common cathodes). Since there are exactly 7 digits, **address bit 0** selects the **7 discrete LEDs**. The schematic shows how the LED module maps to the latches.

Anodes are **active‑high**, cathodes are **active‑low**. For example, to light **segment A** of the **leftmost digit**, set **data bit 3 = 1** and **address bit 1 = 0**. Do this by writing the value **`$08`** to address **`$80FD`**.

Let’s break that down:

```
Data bits
76543210
00001000 = 08h

Address bits
76543210
11111101 = FDh

Write to $8000–$FFFF → 0x8000 + 0x00FD = 0x80FD
(95FDh or FEFDh would also work; any address ≥ 8000h latches.)
```

**Note:** Unlike the original design by Lee Hart, Daryl Rictor, and Josh Bensadon, this badge uses **7** discrete LEDs connected to the data bus (not 5). If you use their original firmware, the chaser will use only 5 LEDs because its table defines 5. I provide a firmware ([BadgeOS_50th.zip](downloads/BadgeOS_50th.zip)) that uses **all 7** LEDs. See the **[Basic](basic)** folder for example programs.

---

## Serial Port

The serial port is TTL‑level asynchronous: **TxD**, **RxD**, and **GND**. It resembles RS‑232 but uses **5 V/0 V** logic and **non‑inverted** data (idle = 5 V = logic 1). You can use a **TTL‑to‑RS‑232** adapter on **J3** to talk to a classic terminal, or mount the **CH340N SOP‑8 USB‑to‑TTL** module at **J2** for a USB serial adapter supported by modern OSes. Bonus: USB provides **5 V power** to run the board and **charge Ni‑Cd cells** (if present and **JP2 closed**).

**Serial settings:** **9600, N, 8, 1** (9600 baud, no parity, 8 data bits, 1 stop bit).

**Writing TX:** write `%00000000` (`$00`) to clear bit 7 (TX=0) or `%10000000` (`$80`) to set TX=1 at **any** address ≥ `$8000`. To **blank** all digits, write to any address ≥ `$8000` with **low byte = `$FF`** (e.g., `$80FF`), which drives all 8 cathodes **high** (inactive). To preserve the current LED state, store the LED data and address values in **RAM**.

**Reading RX:** the **6502 IRQ (pin 4)** is used. The software contains an **interrupt handler** to capture incoming transitions. Because IRQ is **active‑low**, it directly detects low levels; precise timing loops detect high (absence of interrupt). RX is **inverted by U3**, so effective RX behavior is **RS‑232‑conformant**.

Install a **terminal program** on your PC (e.g., **PuTTY** on Windows, **miniterm/minicom** on Linux).

For reliable **copy‑and‑paste uploads**, slow the send rate in your terminal if possible:

1. **Inter‑byte delay:** ~**20 ms**
2. **Delay after LF/CR:** ~**200 ms**

There is **no FIFO** (software serial), so sending too fast will cause **timing errors** and **corrupted transfers**.

---

## Software Overview

Power‑on begins with **reset**. The 6502 jumps via the 16‑bit vector at **`$FFFC/$FFFD`**. The reset routine initializes the LED display and the software serial port, then enters the **machine‑language monitor**.

The monitor runs on the serial port at **9600, N, 8, 1** and also drives a **scrolling message** on the 7‑segment digits (default “6502 badge for VCF” or “6502 50th Birthday 1975–2025”). The 7 discrete LEDs run a “Knight Rider” chase. The display refreshes while the monitor waits for serial input; if no data arrives, the animation runs continuously.

---

## 6502 Badge — Monitor & Reference Guide

Entering `?<Return>` shows a concise help screen:

<img src="images/OS_Monitor.png" title="Monitor Help Screen" alt="Monitor Help Screen" style="zoom:50%;">

### Monitor Commands

The monitor uses hexadecimal digits plus **non‑alphanumeric** command characters. Command line format:

```
SSSS.EEEE C <Return>
```

* `SSSS` and `EEEE` are **start** and **end** addresses (separated by a dot).
* `C` is the **command symbol** (a non‑alphanumeric character).
* `<Return>` is the Enter key.  
  **Note:** No spaces between tokens (e.g., `1234.5678L<Return>`).

Addresses can be 1–2 bytes (2–4 hex digits). If you type more than 4 hex digits, only the **last 4** are used (e.g., `1A2B3C.4D5E6C` becomes `2B3C` and `5E6C`). Shorter inputs are **left‑padded with `0`**; thus `0.3FF` covers `$0000–$03FF`.

For several commands the address is optional. The monitor remembers the **last hex value** and **auto‑increments** it if you omit a new one. Example:

`1000L<Return>` disassembles 20 lines starting at `$1000`. A following `L<Return>` continues from that address. `1000LLL<Return>` shows 60 lines from `$1000` with fewer keystrokes.

`?<Return>` prints a quick help:

```
Commands are :
Syntax = {} required, [] optional, HHHH hex address, DD hex data

[HHHH][ HHHH]{Return}         - Hex dump address(es) (up to 16 w/o address)
[HHHH]{.HHHH}{Return}         - Hex dump range (16 per line)
[HHHH]{:DD}[ DD]{Return}      - Change data bytes
[HHHH]{G}{Return}             - Execute program (RTS returns to monitor)
{HHHH.HHHH>HHHHI}{Return}     - Insert (2nd) down into 1st→3rd (backward copy)
[HHHH]{L}{Return}             - Disassemble 20 lines
[HHHH]{.HHHH}{L}{Return}      - Disassemble range
{HHHH.HHHH>HHHHM}{Return}     - Move (1st→2nd) to 3rd (forward copy)
{HHHH}[ HHHH]{Q}{Return}      - Text dump address(es)
[HHHH]{.HHHH}{Q}{Return}      - Text dump range (16/line)
{S}[up to 32 chars]{Return}   - Set LED message
[HHHH]{U}{Return}             - Upload (PC→SBC, XMODEM/CRC)
[HHHH.HHHH]{X}{Return}        - Download (SBC→PC, XMODEM/CRC)
{V}{Return}                   - Monitor version
{P*}{Return}                  - Protected power down
{!}{Return}                   - Mini-assembler
{@}{Return}                   - EhBASIC cold start
{#}{Return}                   - EhBASIC warm start
{?}{Return}                   - Show help
```

### Hex Dump

```
[HHHH][ HHHH]<Return>   - Hex dump address(es) (up to 16 w/o address)
[HHHH]{.HHHH}<Return>   - Hex dump range (16 per line)
```

Shows raw memory contents in hex.

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

Writes data to RAM. Address followed by a colon `:` and one or more bytes `DD` (space‑separated for more).  
Writes to ROM won’t fail, but won’t change ROM—on the badge they act on the **I/O latches** (see above).

### Move Memory

```
{SSSS.EEEE>DDDDM}<Return>
```

Copies memory **forward** from `SSSS…EEEE` to start at `DDDD`.

Trick to **fill** a range: set the first byte with *Edit Memory*, then *Move* it across the range.

```
1000:00<Return>
1000.1FFE>1001M<Return>
```

**Warning:** If `DDDD` lies inside `SSSS–EEEE`, you will overwrite the source. Use **Insert Memory** instead.

### Insert Memory

```
{SSSS.EEEE>DDDDI}<Return>
```

Like *Move*, but copies **backward** (from `EEEE` down). Lets you open gaps inside a region. If `DDDD` lies **outside** `SSSS–EEEE`, both Move/Insert behave the same.

### Execute

```
[HHHH]{G}<Return>
```

Runs a machine‑language program. Use `RTS` (`$60`) to return to the monitor. If omitted, the last stored address is used—but it’s safer to specify it (e.g., `1000G<Return>`).

### Disassemble

```
[HHHH]{L}<Return>          - 20 lines
[HHHH]{.HHHH}{L}<Return>   - range
```

Without an address: 20 lines from the last position. Example:

```
>FF00L

FF00-  x    78         SEI  
FF01-  X    D8         CLD  
FF02-  ".   A2 FF      LDX  #$FF
...
FF25-  )h   A9 E8      LDA  #$E8
>
```

Format: address – ASCII of bytes (non‑printables as `.`) – hex – mnemonic + operands.

### Text Dump

```
{HHHH}[ HHHH]{Q}<Return>
[HHHH]{.HHHH}{Q}<Return>
```

Like *Hex Dump*, but **ASCII**. Useful to find text in memory. Non‑printables → `.`

### Set LED Text

```
{S}[up to 32 characters]<Return>
```

Sets the scrolling LED message (32‑byte buffer; longer input is truncated). Example: `S6502 badge<Return>` shows:

```
6502 badge
```

See **LED Operations** for refresh/scroll details and custom routines.

### Upload (XMODEM)

```
[HHHH]{U}<Return>  – Upload PC→Badge (XMODEM/CRC)
```

File is stored starting at the given (or last) address. **Caution:** due to the 128‑byte buffer, up to **127 extra bytes** may be appended—avoid overwriting. Only **XMODEM/CRC** is supported (no checksum/1k mode).

### Download (XMODEM)

```
[HHHH.HHHH]{X}<Return> – Download Badge→PC (XMODEM/CRC)
```

Sends the specified range. Always provide explicit addresses if possible (same 128‑byte buffer caveats).

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

### Protected Power Down

```
{P*}<Return>
```

Turns off LEDs and enters an infinite loop in ROM so RAM remains intact before power‑off.

### Mini‑Assembler

```
{!}<Return>   – enter assembler
```

A simple RAM assembler (hex operands, no labels/arithmetic). Prompt changes from `>` to `!`. Help (`!?`) shows:

```
HHHH=hex address, OPC=Opcode, DD=hex data, '_'=Space/Tab
'$' optional, all HEX. Input after ';' is ignored.

{HHHH}{Return}                      - set input address
[HHHH][_]{OPC}[_][#($DD_HHHH,X),Y]{Return} - assemble one line
[HHHH]{L}{Return}                   - disassemble 20 lines
{Return}                            - leave assembler
{?}{Return}                         - help
```

Supported mnemonics include: `ADC AND ASL BCC ... WAI STP BBRx BBSx RMBx SMBx .DB .DW .DS`.  
WDC opcodes (`WAI`, `STP`, `BBRx/BBSx`, `RMBx/SMBx`) are **not implemented** by the badge CPU but are accepted by the assembler (see WDC docs). Extra pseudo‑ops:

* `.DB HH`  – define byte
* `.DW HHHH` – define word (low byte first)
* `.DS 'Text'` – define ASCII string

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

The `^` marker shows an error (e.g., branch target out of range).

### Help

```
{?}<Return>
```

Shows the help menu (available in both monitor and mini‑assembler).

---

## EhBASIC: Cold & Warm Start

**Cold start** `{@}<Return>` initializes RAM and sets the **top of memory**. Enter the size in **decimal**:

* 2048 → 2 KB RAM
* 32768 → 32 KB RAM

Example (2 KB RAM):

```
>@
Memory size ? 2048
1023 Bytes free
Enhanced BASIC 2.22

Ready
```

The first **1 KB** of RAM is used by the monitor & LED display, so with 2 KB total you have ~1 KB free. Use `SYS<Return>` (new) to return from the EhBASIC prompt to the monitor.

**Warm start** `{#}<Return>` returns to EhBASIC after `SYS` **without** re‑initialization (RAM program remains).

---

## EhBASIC Quick Reference & Keywords

EhBASIC by **Lee Davison** (adapted here with permission). Manual: `http://www.sunrise-ev.com/photos/6502/EhBASIC-manual.pdf`. Source is extensively commented.

**Keyword list (excerpt):**  
`ABS AND ASC ATN BIN$ BITCLR BITSET BITTST CALL CHR$ CLEAR CONT COS DATA DEC DEEK DEF DIM DO DOKE ELSE END EOR EXP FN FOR FRE GET GOSUB GOTO HEX$ IF INC INPUT INT IRQ LCASE$ LEFT$ LEN LET LIST LOAD LOG LOOP MAX MID$ MIN NEW NEXT NMI NOT NULL OFF ON OR PEEK PI POKE POS PRINT READ REM RESTORE RETIRQ RETNMI RETURN RIGHT$ RND RUN SADD SAVE SGN SIN SPC( SQR STEP STOP STR$ SWAP SYS TAB( TAN THEN TO TWOPI UCASE$ UNTIL USR VAL VARPTR WAIT WHILE WIDTH + - * / ^ << >> > = <`

* Keywords are **UPPERCASE** and **space‑free**.
* Numbers: integer, decimal, or float; prefix `$` (hex) or `%` (binary). Examples: `$0A`, `1`, `-142`, `96.3`, `2.718E-3`.
* Variables: numeric, `Strings$`, or arrays `(n)`; strings in quotes (`"Hello world"`).

---

## LED Operations

The monitor provides routines to **refresh** the scrolling **7‑segment digits** and the **discrete LEDs**. Basics: set address latch to the first digit → fetch bit pattern from RAM → write to buffer → briefly enable → move to next digit → repeat (persistence of vision). For **scrolling**, shift the start pointer periodically; speed depends on the number of refresh cycles between shifts. While idle (monitor/EhBASIC input wait), refresh runs smoothly; during input it may briefly pause.

Sources: `LEDdrive.asm` and `font.asm`.

**Important RAM addresses (variables):**

```
Lbuff  = $02A0 ; LED text buffer (max 32 bytes)
LDbuff = $02C0 ; discrete LED buffer (max 32 bits)
Lptr   = $E2   ; LED pointer (0..31)
Ldig   = $E3   ; digit counter (0..7; 0 = discrete LEDs)
Lscn   = $E4   ; scan delay (brightness/flicker) – 0..255, 0=display refresh off
Lscl   = $E5   ; scroll delay – 0..255, 0=static
Lscnc  = $E6   ; scan counter (counts down from Lscn)
Lsclc  = $E7   ; scroll counter (counts down from Lscl)
LEDchk1 = $E8  ; config checksum #1
LEDchk2 = $E9  ; config checksum #2
```

`Lbuff`/`LDbuff` are **synchronized** (position 0..31). Set `Lscn=$00` to **disable monitor refresh** (for your own LED routines).  
`LEDchk1=$A5` **and** `LEDchk2=$5A` prevent buffers from being overwritten on reset (otherwise they default to “6502 badge for VCF” + “Knight Rider”). Use *Edit Memory* to set/clear these flags.

---

## Serial I/O Operations

There are three monitor subroutines for serial I/O (call with `JSR`). **Note:** there are two ROM versions; addresses depend on the **version date** (`V` command).

* **Serial_Output** (`$EAE8` *or* `$EAEC`) – sends 1 byte (in A); `X`/`Y` preserved.
  
  ```asm
  ; 5-17-17 ROM          ; 2-24-18 ROM
  LDA #$41               LDA #$41   ; ASCII "A"
  JSR $EAE8              JSR $EAEC  ; send
  ```
* **Serial_Input** (`$EB35` *or* `$EB39`) – blocking read; byte in A; `X`/`Y` preserved; flags `Z/N` set.
  
  ```asm
  JSR $EB35              JSR $EB39  ; get char
  STA $400               STA $400   ; store
  JSR $EAE8              JSR $EAEC  ; echo
  ```
* **Scan_Input** (`$EB4C` *or* `$EB50`) – non‑blocking; no input → **carry clear**; input: byte in A, `Z/N` set, **carry set**.
  
  ```asm
  Loop  JSR $EB4C        JSR $EB50  ; check
        BCC Loop         BCC Loop   ; nothing → again
        BMI Loop         BMI Loop   ; >$7F? (N=1) → again
        STA $400         STA $400   ; store
  ```

---

## System Memory Usage

The following regions are used by the system. Whether you may overwrite them depends on your use—study the sources.

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

| Range         | Use                                |
| -------------:| ---------------------------------- |
| `$0100–$01FF` | system stack                       |
| `$0200–$027F` | serial receive ring buffer         |
| `$02A0–$02DF` | LED buffer                         |
| `$0300–$037F` | monitor input buffer               |
| `$0390–$03FF` | EhBASIC input buffer               |
| `$0400–$7FFF` | user RAM / EhBASIC program (32 KB) |

### ROM (depends on monitor date)

| **5‑17‑17 ROM** | **2‑24‑18 ROM** | Description               |
| --------------- | --------------- | ------------------------- |
| `$C000–$C1FF`   | `$C000–$C1FF`   | CRC lookup table (XMODEM) |
| `$C200–$EA9B`   | `$C200–$EA9F`   | EhBASIC                   |
| `$EA9C–$EB64`   | `$EAA0–$EB68`   | serial I/O routines       |
| `$EB65–$FC39`   | `$EB69–$FC3D`   | monitor                   |
| `$FC3A–$FD93`   | `$FC3E–$FD97`   | LED support               |
| `$FD94–$FFBE`   | `$FD98–$FFC2`   | XMODEM                    |
| `$FFBF–$FFFF`   | `$FFC3–$FFFF`   | reset code & vectors      |

---

## Source Organization & Build Notes

Except for EhBASIC, software by **Daryl Rictor**. Use/adapt for **non‑commercial** purposes.

**Files:**

* `sbc.asm` – “makefile” style: includes all sources in order/addresses
* `basic.asm` – EhBASIC source
* `basldsv.asm` – patch for load/save via XMODEM
* `sbcOS.asm` – monitor incl. disassembler & mini‑assembler
* `serial.asm` – software serial driver
* `LEDdrive.asm` – LED driver (refresh, scroll, text)
* `font.asm` – LED font (ASCII → latch pins)
* `xmodem.asm` – XMODEM protocol
* `CRCtable.asm` – CRC lookup table
* `reset.asm` – reset/init; ROM vectors `$FFFA–$FFFF`; BRK handler (`$00`) → reset & monitor

**Assembling (6502 Macroassembler & Simulator, `6502.exe`):**

1. Start the program
2. Open `sbc.asm` (`File → Open → sbc.asm`)
3. Options:
   * `Assembler` → **Extra byte after BRK**: **disable**
   * `General` → select **65C02, 6501**
4. Assemble (`F7`)
5. Save object (`File → Save Code`) as Intel‑Hex, S‑Record, or Binary
   * **Start address**: `0xC000` (16 KB ROM) **or** `0x8000` (32 KB ROM)
   * **End address**: `0xFFFF`
   * **OK** → **SAVE**

---

## Downloads / Firmware / Manuals

1. Custom **BadgeOS firmware** 32 KB 27C256 EPROM U1 (7× LEDs, 50th version) > [here](downloads/BadgeOS_32k_50th.rom) < (BIN, 32 KB)
2. Original **BadgeOS (firmware/ROM)** > [here](downloads/BadgeOS.zip) < (ZIP, 0.8 MB)
3. Original **Badge Manual** by **Lee Hart, Daryl Rictor, and Josh Bensadon** > [here](downloads/badge-manual.pdf) < (PDF, 1.6 MB)
4. Original **EhBASIC** manual > [here](downloads/EhBASIC-manual.pdf) < (PDF, 0.5 MB)
5. **Schematic** (badge) > [here](downloads/Schematic.pdf) < (PDF, 0.2 MB)
6. **PCB layout (Gerber)** > [here](gerber/) <
7. **BOM files** > [here](bom/) <
8. Driver for **CH340 USB‑C to Serial TTL**: <https://www.arduined.eu/tag/ch340/>
9. More downloads for the **MOS 6502 – 50th Anniversary Computer Badge (1975–2025)** > [here](downloads) <

---

## Ordering

This project is available as a **Shared Project** on PCBWay.com > [here](https://www.pcbway.com/project/shareproject/The_MOS_6502_50th_Anniversary_Computer_Badge_1975_2025_439a8755.html) <

---

## Troubleshooting

1. **Power LED is on, but LEDs/scrolling flicker.**  
   Check for a stable **4.5–5 V** at **U2 pin 8**. If not, verify the power source. If the **5 V step‑up booster** receives **< 1.2 V**, it will collapse and pulse.
2. **Some LEDs or 7‑segment digits are stuck off or on.**  
   Inspect **U6/U7 (74HC273)** for bent pins, poor joints, or solder bridges.
3. **Power LED on, but no other function.**  
   1) Check **U3 (74HC139)** pins for shorts or cold joints.  
   2) Verify **U1 EPROM** and **U2 CPU** are correctly seated and U1 has the correct firmware.  
   3) Check **U4 SRAM** seating/orientation.  
   4) Check oscillator **X1**.
4. **No USB‑C connection on Windows.**  
   Install the **CH340** USB‑to‑TTL driver (see Downloads).
5. **CH340 USB module LED stays on when powered from a battery pack, even when the computer is off.**  
   That’s expected: the CH340 module is powered from the pack so the **6502 IRQ** stays high even with no USB cable attached. Otherwise the CPU would be stuck in an IRQ loop and not start. I plan to improve this in a future revision.

---

## Disclaimer

This is a non‑commercial hobby project. Building and using **The MOS 6502 – 50th Anniversary Computer Badge (1975–2025)** is **at your own risk**. No guarantees are made for functionality, safety, completeness, or freedom from errors. The creator (Frank Eggen) is not liable for damage or loss arising from construction or use.

---

## Donations

I’ve spent many hours on this project. If you’d like to support the work, you can buy me a coffee—thank you! [Click here to donate via PayPal.](https://www.paypal.com/donate/?cmd=_s-xclick&hosted_button_id=Q8HXKYARXKT4L&ssrt=1714757590172)

---

## Acknowledgements

1. This project is based on the idea by **Lee Hart, Daryl Rictor, and Josh Bensadon** 👉 Original project: [sunrise-ev.com/6502.htm](http://www.sunrise-ev.com/6502.htm). Huge thanks to the original authors—and especially to **Lee Hart** for many helpful tips during the revamp. 🙏
2. To the visionary **Chuck Peddle** and the MOS team including **Terry Holdt, Wil Mathys, Rod Orgill, Harry Bawcom, Sydney Anne Holt, Walt Eisenhower, and John Paivinen**, whose vision enabled the 6502 processor. [https://www.team6502.org](https://www.team6502.org)
3. **Bill Mensch**, founder of Western Design Center, for keeping the 6502 alive, documented, and evolving. [https://www.westerndesigncenter.com](https://www.westerndesigncenter.com)
4. **Ben Eater** for the “Build a 6502 computer” project. [https://eater.net/6502](https://eater.net/6502)
