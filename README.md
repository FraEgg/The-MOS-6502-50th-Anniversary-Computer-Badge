# The MOS 6502 – 50th Anniversary Computer Badge (1975–2025)

## A Retro Computer in Badge Format for 8-Bit 6502 Fans

By Frank Eggen (Final Version 2.6)

👉 [German Version](README_DE.md)

[<img src="images/Youtube.jpg" title="Watch Video on YouTube" alt="Watch Video on YouTube" style="zoom:50%;">](https://www.youtube.com/shorts/PbgMO4NnUvw)

---

Based on an idea by **Lee Hart, Daryl Rictor, and Josh Bensadon** (revived and updated).
👉 Original Project: [sunrise-ev.com/6502.htm](http://www.sunrise-ev.com/6502.htm)

---

## Table of Contents

1. [About the Project](#50-years-of-the-8-bit-mos-6502-microprocessor)
2. [Features & Hardware](#technical-overview)
3. [Bill of Materials (BOM)](#bill-of-materials-bom)
4. [Assembly Guide](#assembly)
5. [Jumper Configuration](#jumper-options)
6. [Setup & First Test](#lets-see-it-in-action)
7. [Technical Details (Architecture & I/O)](#technical-details-schematics--architecture)
8. [Software & Monitor Manual](#software-description)
9. [EhBASIC](#ehbasic-cold-start--warm-start)
10. [System Internals (For Developers)](#system-internals-for-developers)
11. [Downloads & Links](#downloads-firmware-manuals)
12. [FAQ / Troubleshooting](#troubleshooting)
13. [Disclaimer & Credits](#disclaimer)

---

## 50 Years of the 8-Bit MOS 6502 Microprocessor

<img title="White Ceramic 6502 CPU Illustration" src="images/white-ceramic-6502-illustration.png" alt="loading-ag-1374" data-align="center">

The legendary **MOS 6502** was introduced in 1975 and changed the world of computing forever. It brought high performance at an affordable price and made the rise of **home computers** possible.

Famous systems powered by the 6502:

* Apple II
* Commodore VIC-20 & C64
* Nintendo NES
* BBC Micro
* Atari VCS

👉 More history: [team6502.org](https://www.team6502.org)

---

### What is the Computer Badge?

<img title="The MOS 6502 – 50th Anniversary Computer Badge (1975–2025)" src="images/The_MOS_6502–50th_Anniversary_Computer_Badge_Real.jpg" alt="The MOS 6502 – 50th Anniversary Computer Badge (1975–2025)" data-align="center" style="zoom:25%;">

The **MOS 6502 50th Anniversary Computer Badge** is a **minimalist remake** of an 8-bit microcomputer with a 6502 CPU in badge format. Thanks to modern components, it is easy to build today.

**Highlights:**

* **W65C02S Microprocessor @ 2 MHz**
* **32K RAM** with battery backup
* **32K EPROM** with Floating-Point BASIC + 6502 Monitor
* **7-digit 7-segment LED display + 7 LEDs** for effects
* **RS232 compatible interface** for data exchange
* **USB-C (CH340) serial TTL interface** – usable directly on a PC
* **DC/DC Step-Up Module** for stable battery operation
* **CR2032 Battery** for SRAM data retention

> Fully functional, programmable in **Assembler** or **BASIC** – yet small enough to be worn as a retro name badge.

---

### Variants

**Badge Version**

<img title="MOS 6502 50th Anniversary Computer Badge Render" src="./images/PCB_Render_V2.6_Badge.png" alt="PCB MOS 6502 50th Anniversary Computer Badge Render Photo" style="zoom:50%;" data-align="center">

<img title="MOS 6502 50th Anniversary Computer Badge Layout" src="./images/PCB_Layout_V2.6_Badge.png" alt="PCB MOS 6502 50th Anniversary Computer Badge Layout" style="zoom:33%;" data-align="center">

* 7.62 × 10.16 cm (3 × 4 inches) – classic badge format
* Download the PCB layout V2.6 (Gerber file) > [here](gerber/) <

---

### What can you use it for?

* As a **Retro Name Badge** with a scrolling text of your choice
* To **Celebrate 50 Years of the 6502 & the Home Computer Era**
* As an **Educational Project** for Assembler, BASIC, and hardware nostalgia
* For **Tinkering & Fun** with a minimal component count
* Simply as a **cool Collector's Item** for the anniversary

---

### Technical Overview

* W65C02S @ 2 MHz
* 32K RAM with battery backup
* 32K EPROM (BASIC + Monitor)
* 2× 8-Bit Output Latches
* 7-digit 7-segment LED display + 7 LEDs
* 9600, 8n1, serial Soft-RS232 interface
* USB-C to TTL CH340 UART Adapter (BTE17-06B)
* DC/DC 5V Step-Up Boost Converter
* Charging function for 3× AA NiCd rechargeable batteries

👉 This gives you a **full-featured retro system** in your hand – minimalist, educational, and a real eye-catcher at any nerd gathering. 😎

---

### Bill of Materials (BOM)

The list uses recommended components that I have tested. Of course, components from other manufacturers can also be used. I have included alternative components in the current BOM list, which can be obtained cheaply from Chinese suppliers like AliExpress > [here XLS](bom/BOM_65C02_Computer.kicad_pcb_v2.6.xls) <.

_Created on 2025-12-27_

| Pos. | Ref      | Value                         | Qty | Description                            | Package                     | Datasheet                                                                                                                                                     |
|:----:|:-------- |:----------------------------- |:---:|:-------------------------------------- |:--------------------------- |:------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1    | U1       | 27C256 or W27E257-12 (Socket) | 1   | EPROM 256 KiBit (Socket)               | DIP-28_W15.24mm             | [Link](https://www.mouser.com/ProductDetail/Microchip-Technology/AT28C256-25DM-883-815?qs=sGAEpiMZZMv%252BqVJHFCdzIcTLvA16d8bXgqxfSNsRp6tpab4fPFb%2Ffw%3D%3D) |
| 2    | U2       | W65C02S (Socket)              | 1   | W65C02S 8–bit Microprocessor           | DIP-40_W15.24mm_Socket      | [Link](https://www.mouser.com/ProductDetail/Western-Design-Center-WDC/W65C02S6TPG-14?qs=opBjA1TV903lvWo9AEKH5w%3D%3D)                                         |
| 3    | U3       | 74HC139                       | 1   | Dual 2-to-4 line decoder/demultiplexer | SOP-16_4.4x10.4mm_P1.27mm   | [Link](https://www.mouser.com/ProductDetail/Texas-Instruments/SN74HC139PWR?qs=%252BWCn1GN4mVzsIRktqzW%252B6w%3D%3D)                                           |
| 4    | U4       | CY62256N                      | 1   | 256-Kbit (32 K × 8) Static RAM         | SOP-28_8.4x18.16mm_P1.27mm  | [Link](https://www.mouser.com/ProductDetail/Alliance-Memory/CY62256NLL-55SNXIT?qs=byeeYqUIh0MBMJQPS9fE%2Fw%3D%3D)                                             |
| 5    | U5       | MAX690xPA                     | 1   | IC SUPERVISOR 1 CHANNEL 8DIP           | DIP-8_W7.62mm               | [Link](https://www.mouser.com/ProductDetail/Analog-Devices-Maxim-Integrated/MAX690EPA%2b?qs=1THa7WoU59F77SMcFxXEbA%3D%3D)                                     |
| 6    | U6,U7    | 74HC273                       | 2   | IC FF D-TYPE SINGLE 8BIT 20SOIC        | SOIC-20W_7.5x12.8mm_P1.27mm | [Link](https://www.mouser.com/ProductDetail/Nexperia/74HC273D653?qs=sGAEpiMZZMutXGli8Ay4kE3wRMDwmh%2F%252B3McaL2f5IDQ%3D)                                     |
| 7    | R1,R6    | 10K                           | 2   | Metal Film Resistors 10K 1/4W 1%       | Axial                       | [Link](https://www.mouser.com/ProductDetail/SEI-Stackpole/RNMF14FAD10K0?qs=rQFj71Wb1eWBrWvO2mNWLg%3D%3D)                                                      |
| 8    | R2-R4    | 3K3                           | 3   | Metal Film Resistors 3K3 1/4W 1%       | Axial                       | [Link](https://www.mouser.com/ProductDetail/SEI-Stackpole/RNMF14FTC3K30?qs=FESYatJ8odL%252B4KIkrQ9kpA%3D%3D)                                                  |
| 9    | R5       | 10R                           | 1   | Metal Film Resistors 10R 1/4W 1%       | Axial                       | [Link](https://www.mouser.com/ProductDetail/SEI-Stackpole/RNMF14FTC56R0?qs=FESYatJ8odI5g4wJmGs6ow%3D%3D)                                                      |
| 10   | R7       | 2K                            | 1   | Metal Film Resistors 2K 1/4W 1%        | Axial                       | [Link](https://www.mouser.com/ProductDetail/SEI-Stackpole/RNMF14FTC2K00?qs=FESYatJ8odKlooj85fXxuA%3D%3D)                                                      |
| 11   | C1,C4-C8 | 0.1uF                         | 6   | CAP CER 0.1UF 50V Z5U RADIAL           | C_Disc_D4.7mm_W2.5mm        | [Link](https://www.mouser.com/ProductDetail/KEMET/C322C104M5U5TA?qs=CDCeLP2tGBsLrnt3J6Fqow%3D%3D)                                                             |
| 12   | C2,C3    | 470uF                         | 2   | Electrolytic Caps LOW IMPEDANCE        | CP_Radial_D8.0mm_P3.50mm    | [Link](https://www.mouser.com/ProductDetail/Rubycon/16ZLH470MEFC8X11.5?qs=T3oQrply3y9vdBt%2FBJoVxg%3D%3D)                                                     |
| 13   | D1-D3    | 1N5817                        | 3   | 20V 1A Schottky Barrier Rectifier      | D_DO-41_SOD81               | [Link](https://www.mouser.com/ProductDetail/Taiwan-Semiconductor/1N5817?qs=G5AQjGfRJcITga2hz4Rc2w%3D%3D)                                                      |
| 14   | X1       | 2MHz                          | 1   | XTAL OSC XO 2.0000MHZ HCMOS TTL        | Oscillator_DIP-14           | [Link](https://www.mouser.com/ProductDetail/CTS-Electronic-Components/MXO45-3C-2M0000?qs=hbgUSdfWRJVCM8WDm293Vw%3D%3D)                                        |
| 15   | LED1,7   | WHITE                         | 2   | White LED Indication 2.3V              | LED_D5.0mm                  | [Link](https://www.mouser.com/ProductDetail/Lumex/SSL-LX5093UWW?qs=p6VZ%252BklCkRQEgTbVQl4ZVw%3D%3D)                                                          |
| 16   | LED2     | RED                           | 1   | Red LED Indication 2.3V                | LED_D5.0mm                  | [Link](https://www.mouser.com/ProductDetail/LITEON/LTL2F3VEKNT?qs=Sv%252BigzQKaoVYLcEZH8BKGw%3D%3D)                                                           |
| 17   | LED3     | ORANGE                        | 1   | Orange LED Indication 2.3V             | LED_D5.0mm                  | [Link](https://www.mouser.com/ProductDetail/LITEON/LTL-5223?qs=WxFF5lh7QM39C0u211ch5w%3D%3D)                                                                  |
| 18   | LED4     | YELLOW                        | 1   | Yellow LED Indication 2.3V             | LED_D5.0mm                  | [Link](https://www.mouser.com/ProductDetail/Kingbright/WP57YYD?qs=58z0TXQGVSQbwKcOfYiIwA%3D%3D)                                                               |
| 19   | LED5     | GREEN                         | 1   | Green LED Indication 2.3V              | LED_D5.0mm                  | [Link](https://www.mouser.com/ProductDetail/Kingbright/WP56BGD?qs=tMH1uPls0D11B8xP4K7t3g%3D%3D)                                                               |
| 20   | LED6     | BLUE                          | 1   | Blue LED Indication 2.3V               | LED_D5.0mm                  | [Link](https://www.mouser.com/ProductDetail/Kingbright/WP7083QBD-G?qs=vEWui5pQpatbKK552qzGvw%3D%3D)                                                           |
| 21   | LED8     | Power                         | 1   | Red LED Indication (Power) 2.3V        | LED_D3.0mm                  | [Link](https://www.mouser.com/ProductDetail/LITEON/LTL2F3VEKNT?qs=Sv%252BigzQKaoVYLcEZH8BKGw%3D%3D)                                                           |
| 22   | SEG1-7   | SC39-11EWA                    | 7   | 7-segment display, com. cathode        | Sx39-1xxxxx                 | [Link](https://www.mouser.com/ProductDetail/Kingbright/SC39-11EWA?qs=VdjlWU%2FzoOE%2FBaS5v1GsqA%3D%3D)                                                        |
| 23   | SW1      | Reset                         | 1   | SWITCH TACTILE SPST-NO                 | SW_PUSH_6mm                 | [Link](https://www.mouser.com/ProductDetail/Apem/MJTP1230?qs=ooeArD5nza9YuOFpo4pJ2Q%3D%3D)                                                                    |
| 24   | SW2      | ON/OFF                        | 1   | SWITCH SLIDE DPDT 300MA 6V             | JS202011CQN                 | [Link](https://www.mouser.com/ProductDetail/CK/JS202011CQN?qs=LgMIjt8LuD%2Fe%252BE3iTcEFYw%3D%3D)                                                             |
| 25   | J1       | 5V DC-DC                      | 1   | 0.9-5V To 5V Step-Up Module            | THT                         | [Link](https://de.aliexpress.com/item/1005005624977910.html)                                                                                                  |
| 26   | J2       | CH340N                        | 1   | CH340N SOP8 USB to TTL module          | USB-to-TTL-Modul            | [Link](https://de.aliexpress.com/item/1005009386863437.html)                                                                                                  |
| 27   | J3       | Header                        | 1   | Generic connector, 01x05               | PinHeader 1x05              | -                                                                                                                                                             |
| 28   | JP1      | *WD/MOS                       | 1   | Solder Jumper, 2-pole, open            | -                           | -                                                                                                                                                             |
| 29   | JP2      | Charging                      | 1   | Solder Jumper, 2-pole, closed          | -                           | -                                                                                                                                                             |
| 30   | BT1      | 3x AA                         | 1   | Holder 3x AA (Warning: NiCd only!)     | Keystone_3xAA               | [Link](https://www.mouser.com/ProductDetail/Keystone-Electronics/2464?qs=3CbvriavsLDuYK6W9WnmCg%3D%3D)                                                        |
| 31   | BT2      | CR2032                        | 1   | Holder CR2032 (Backup)                 | Panasonic_CR2032            | [Link](https://www.mouser.com/ProductDetail/Keystone-Electronics/106?qs=Q3RoVmURDolnMuconA2vXg%3D%3D)                                                         |

#### Notes:

It is recommended to use a DIP socket for ICs U1 and U2.

---

### Assembly

Please check the parts list to make sure you have everything. To assemble, you will need a soldering iron, solder, and flux for the SMD ICs. It is also best to have pliers, a desoldering pump, and desoldering wick ready.

I recommend the following order for assembly:

1. **SMD ICs:** First, solder the SMD ICs to the board: U3 (74HC139), U6, U7 (74HC273), and then U4 (SRAM).
   *My Tip:* Everyone has their own method for SMDs. I always put a drop of flux on the first pin (top left) and the last pin (bottom right). Then I place the IC on the pads and fix these two pins with a little solder. If the IC sits well, I apply flux to the remaining pins and solder them individually. Be sure to pay attention to the **polarity**: Pin 1 is where the arrow/dot on the board marks it.

2. **Sockets:** Now solder the sockets for U1 (EPROM) and U2 (W65C02S Microprocessor).

3. **U5:** Solder in U5 (MAX690, alternatively MAX692).

4. **Oscillator:** Next is the X1 2MHz oscillator as the clock generator.

5. **Diodes:** Insert the diodes D1, D2, D3 (1N5817) (mind the polarity/ring!).

6. **Resistors:** Now it's time for the resistors R1 - R7.

7. **Ceramic Capacitors:** Solder in C1, C4, C5, C6, C7, and C8.

8. **Electrolytic Caps:** Follow with the two electrolytic capacitors C2 and C3 with 470uF (10-16V). Watch the polarity!

9. **Switches:** Now the reset button SW1 and the DIP switch SW2 (ON/OFF) are still missing.

10. **LEDs:** Place LED1-LED7 (LED bar) and LED8 (Power LED).
    *Attention:* Watch the **polarity**! The hole with the square solder pad is the cathode (minus/flat side).

11. **DC/DC Converter (J1):** Install the Step-Up module on the back of the board (using 3-pin headers).
    *Important:* The coil on the module must face away from the PCB.
    *Option:* If you do **not** want to use a Step-Up module, bridge Pin 1 and 3 on J1 (Caution: Do not connect to Pin 2!). This is only recommended if you operate the badge exclusively with stable 5V (lab power supply or USB-C).

12. **USB Module (J2):** Connect the CH340N USB-to-TTL module with a 5-pin header on the back. Make sure the alignment is correct here as well.

13. **Cleaning:** Clean the board of flux residues.

14. **Displays:** Install the 7-segment displays. The decimal point (DP) is at the bottom right; this must also face down on the board.

15. **Battery Holders:** Install BT1 and BT2 if needed. Do not insert batteries yet!
    **WARNING:** For BT1, use **only 3x AA NiCd 1.2V rechargeable batteries** if JP2 is closed! The charging electronics are very simple. Other types (Li-Ion, NiMH) must not be charged (fire hazard!). If using normal alkaline batteries, **JP2 must be opened**.

16. **Chips:** Finally, insert the heart U2 (W65C02S CPU) and the programmed EPROM U1 into the sockets.

---

### Jumper Options

The badge has three jumpers for configuration:

1. **JP1 (CPU Type):** Selects the processor type.
   
   * **Open (Standard):** For the W65C02S (Western Design Center). This modern CMOS type has the "Vector Pull" (VPB) output at Pin 1 and must not be tied to ground.
   * **Closed:** For older NMOS types (MOS, Rockwell, UMC, Synertek) that require Ground (GND) at Pin 1. When using old CPUs, make sure to use a 2MHz variant (e.g., 6502AD, R6502AP).
   * *Recommendation:* Use the **W65C02S** (CMOS). It consumes less power, and the BadgeOS utilizes its extended instruction set.

2. **JP2 (Charging):** Controls the charging of AA batteries.
   
   * **Closed (Standard):** Charging function active. **Only for NiCd batteries!**
   * **Open:** Charging function disabled. Mandatory if standard 1.5V Alkaline batteries are used.

---

## Let's see it in action!

Now for the big moment.

1. Set SW2 to **OFF**.
2. Connect a stable 5V power source (via USB-C J2 or Pin Header J3).
3. Switch SW2 to **ON**.

The Power LED should light up, and you will be rewarded with the scrolling text **"6502 badge for VCF"** or **"6502 50th Birthday 1975-2025"** on the display!

**Testing Battery Operation:**

1. Set SW2 to **OFF**, disconnect external power source.
2. Insert the CR2032 (SRAM backup) and the 3x AA NiCd batteries.
   *Note:* In battery operation, the Power LED does not light up when the device is OFF (unlike when powered externally).
3. Set SW2 to **ON** – the computer should start.

If charging via USB, a full charge cycle takes about 6-8 hours. The runtime is 6-12 hours.

**Lanyard & Case:**
The board has four mounting holes for feet or a case. A lanyard can be attached to the top holes to wear the badge around your neck.

![Lanyard](images/Lanyards.jpg "Lanyard Title MOS 6502 - 50th Anniversary Computer Badge")

---

### Technical Details: Schematics & Architecture

Schematic of **The MOS 6502 – 50th Anniversary Computer Badge** > [PDF here](downloads/Schematic_v2.6.pdf) <

<img title="Schematic PCB" src="images/Schematic_PCB_v2.6.png" alt="Schematic PCB" style="zoom:25%;" data-align="left"><img title="Schematic Display" src="images/Schematic_Display_v2.6.png" alt="Schematic Display" style="zoom:25%;" data-align="left">

The badge is a complete, minimalist computer:

* **CPU (U2):** W65C02S @ 2 MHz.
* **Memory:** 32KB RAM (U4) and 32KB ROM (U1).
* **Logic (U3):** The 74HC139 handles address decoding for RAM/ROM (CS) and controls the LED segments.
* **I/O (U6/U7):** Two 74HC273 chips act as multiplexers and latches for the LEDs and the 7-segment display. Bit 7 additionally functions as the TX signal.

**RS232 Special Feature:**
No UART chip is used!

* **RX:** Runs via the IRQ pin (Pin 4) of the CPU (inverted by U3).
* **TX:** Runs via Bit 7 of the latch.
  The OS emulates a **Soft-RS232** (9600 Baud, 8N1). Via the USB-to-TTL adapter (CH340), you can connect the badge to modern PCs (PuTTY, Minicom).

---

### Memory Map

| Address | Start   | End     | Description      |
|:------- |:------- |:------- |:---------------- |
| **RAM** | `0000h` | `7FFFh` | 32 KB SRAM (U4)  |
| **ROM** | `8000h` | `FFFFh` | 32 KB EPROM (U1) |

---

### Input / Output & The "Crazy" Layout

The two latches (U6/U7) control LEDs and I/O. They share a common clock derived from a write pulse to the address space `8000h - FFFFh`.

To simplify the layout and save hardware, data and address lines are physically mixed "wildly" (D0 to D0, A4 to A4, etc.).

![Input-Output Schemata](images/Input-Output-Schema.png "Input-Output Schemata")

**Why this layout?**

1. Updates all 15 LED control bits with a single instruction (no flickering).
2. Minimal hardware (no UART needed).
3. Simpler PCB layout.

#### Controlling the LED Display

* **Data Bus (Bits 0-6):** Selects the segments (A-G).
* **Data Bus (Bit 7):** TX (Serial Output).
* **Address Bus (Bits 1-7):** Selects the digits (Cathodes).
* **Address Bus (Bit 0):** Selects the discrete LEDs.

Example: To turn on Segment A of the leftmost digit, you write `08h` to address `80FDh`.
*Data:* `00001000` (08h)
*Address:* `11111101` (FDh) -> Offset to Base `8000h` = `80FDh`.

**Note on Firmware:**
My version (`BadgeOS_50th`) supports all **7 discrete LEDs**. The original firmware by Lee Hart only controlled 5.

---

### Serial Port

The port uses **9600, 8, N, 1**.
You can connect a TTL-to-RS232 adapter to J3 or use the USB module (J2).

* **Terminal Settings:** 9600 Baud, 8 Data bits, No parity, 1 Stop bit.
* **Delay for Uploads:** Since the port is software-based (no hardware FIFO), you need delays when pasting text/code:
  * 20ms per character
  * 200ms after line break (LF/CR)

To set TX to Low, write `00h` (Bit 7=0); for High, write `80h` (Bit 7=1) to any address >= `8000h`.

---

## Software Description

After reset, the **Monitor** starts. It controls the scrolling text ("6502 50th Birthday...") and waits for serial input.

<img src="images/OS_Monitor.png" title="Screenshot Monitor Helpscreen" alt="Screenshot Monitor Helpscreen" style="zoom:50%;">

### Monitor Commands

The format is always: `SSSS.EEEE C <Return>` (Start address, End address, Command).
No spaces before the command!

#### Command Overview

| Command       | Syntax                  | Description                              |
|:------------- |:----------------------- |:---------------------------------------- |
| **Hex Dump**  | `[Start][ End]<Ret>`    | Displays memory content.                 |
| **Edit**      | `Addr:DD DD...`         | Writes data (DD) to memory.              |
| **Go**        | `AddrG`                 | Starts program at address (RTS returns). |
| **List**      | `AddrL`                 | Disassembles 20 lines of code.           |
| **Move**      | `Start.End>DestM`       | Copies memory range (forward).           |
| **Insert**    | `Start.End>DestI`       | Copies memory range (backward/insert).   |
| **Text**      | `S[Text]`               | Sets the LED scrolling text.             |
| **Upload**    | `AddrU`                 | Receives file from PC (XMODEM/CRC).      |
| **Download**  | `Start.EndX`            | Sends file to PC (XMODEM/CRC).           |
| **Basic**     | `@` (Cold) / `#` (Warm) | Starts EhBASIC.                          |
| **Assembler** | `!`                     | Starts the Mini-Assembler.               |
| **Help**      | `?`                     | Shows the help menu.                     |
| **Shutdown**  | `P*`                    | Protected Power Down (LEDs off, loop).   |

#### Detailed Description of Important Commands

**Hex Dump:**

* `5.2D<Return>` shows the range from 0005 to 002D.
* Without an address, the next 16 bytes are displayed.

**Edit Memory:**

* `1000:55 56 57<Return>` writes values 55h, 56h, 57h starting at address 1000h.

**Move Memory (Copy):**

* `1000.1FFF>2000M` copies the content of 1000h-1FFFh to 2000h.
* *Tip for Filling:* Set `1000:00`, then `1000.1FFE>1001M` copies 00 to the entire range.

**Mini-Assembler (`!`):**
Simple assembler for mnemonics.

* `!1000` sets start address.
* `LDA #FF` assembles the command.
* Empty line exits the assembler.
* *Caution:* WDC-specific opcodes (WAI, STP) are accepted but only work on CMOS CPUs.

---

### EhBASIC: Cold Start & Warm Start

**Cold Start (`@`):**
Initializes memory. Question for "Memory size?" can be answered with `Return` (for max) or `32768`.
Use the `SYS` command to return to the Monitor.

**Warm Start (`#`):**
Returns to BASIC without clearing the program in RAM.

EhBASIC is a powerful interpreter by Lee Davison. It supports Floating Point, Arrays, Strings, and much more.

> [EhBASIC Manual Download](downloads/EhBASIC-manual.pdf)

---

### System Internals (For Developers)

#### Important RAM Addresses (Zero Page & Buffer)

| Range     | Usage                               |
|:--------- |:----------------------------------- |
| `$00-$13` | EhBASIC                             |
| `$32-$3F` | Monitor Variables                   |
| `$E2-$E9` | LED Driver                          |
| `$EA-$ED` | Serial Driver                       |
| `$02A0`   | `Lbuff` (LED Text Buffer, 32 Bytes) |
| `$E4`     | `Lscn` (Scan Delay, 0=Refresh off)  |

#### LED Driver Variables

To program your own effects, these addresses are important:

* `Lptr` ($E2): LED Pointer.
* `Lscn` ($E4): Brightness/Scan Speed. Set to 0 to stop monitor refresh and use custom routines.
* `LEDchk1/2` ($E8/$E9): Checksums ($A5/$5A). If these are incorrect, the default text loads on reset.

#### Assembling the Source Code

The software is divided into modules (`sbc.asm` is the main file).
Use a 6502 Macro Assembler (e.g., the simulator `6502.exe`):

1. Open `sbc.asm`.
2. Set "Extra byte after BRK" to *disabled*.
3. Select Processor **65C02**.
4. Compile as Binary/Hex for start address `$8000` (32K ROM).

---

## Downloads/Firmware/Manuals

1. **Firmware (50th Edition):** [BadgeOS_32k_50th.rom](downloads/BadgeOS_32k_50th.rom) (BIN 32KB, supports 7 LEDs)
2. **Manual (German):** [Manual_50th_DE_2.6.pdf](downloads/Manual_50th_DE_2.6.pdf)
3. **Manual (English):** [Manual_50th_EN_2.6.pdf](downloads/Manual_50th_EN_2.6.pdf)
4. **Original Firmware:** [BadgeOS.zip](downloads/BadgeOS.zip) (only 5 LEDs)
5. **Schematic:** [Schematic_v2.6.pdf](downloads/Schematic_v2.6.pdf)
6. **Gerber Files:** [PCB Layout](gerber/)
7. **BOM (Excel):** [Parts List](bom/)
8. **Driver:** [CH340 USB Driver](https://www.arduined.eu/tag/ch340/)

---

## Ordering

The project is available as a "Shared Project" at PCBWay:

> [The MOS 6502 – 50th Anniversary Computer Badge @ PCBWay](https://www.pcbway.com/project/shareproject/The_MOS_6502_50th_Anniversary_Computer_Badge_1975_2025_439a8755.html)

---

## Troubleshooting

**Q: The Power LED is on, but the display flickers.**
A: Check the voltage at U2 Pin 8. It must be 4.5–5V. If the Step-Up converter gets <1.2V input, the voltage collapses.

**Q: Some LEDs are permanently on or off.**
A: Check U6 and U7 (74HC273) for solder bridges or cold solder joints.

**Q: Power LED on, but nothing else happens.**
A:

1. Check U3 (74HC139).
2. Are EPROM (U1) and CPU (U2) seated correctly? Is the correct firmware installed?
3. Check SRAM (U4) and Oscillator (X1).

**Q: No USB connection (Windows).**
A: Install the CH340 driver.

**Q: CH340 LED lights up even when Badge is off (in battery mode).**
A: This is normal. The module is powered by the battery to keep the IRQ pin High (otherwise the CPU won't start). This will be optimized in a future revision.

---

## Disclaimer

This project is a non-commercial hobby project. Building and using the **The MOS 6502 – 50th Anniversary Computer Badge** is entirely at your own risk. No guarantee for function, safety, completeness, or absence of errors is provided. The creator is not liable for any damages resulting from the assembly or use.

---

## Donations

I have put many hours into this project. If you would like to support my work:
[☕ Donate to the Coffee Fund (PayPal)](https://www.paypal.com/donate/?cmd=_s-xclick&hosted_button_id=Q8HXKYARXKT4L&ssrt=1714757590172)

Thank you very much!

---

## Credits

1. **Lee Hart, Daryl Rictor & Josh Bensadon:** For the brilliant original idea ([sunrise-ev.com](http://www.sunrise-ev.com/6502.htm)).
2. **Team MOS (Chuck Peddle, Bill Mensch, et al.):** For creating the 6502 ([team6502.org](https://www.team6502.org)).
3. **Bill Mensch:** Founder of the Western Design Center ([westerndesigncenter.com](https://www.westerndesigncenter.com)).
4. **Ben Eater:** For his inspiring "Build a 6502 computer" videos ([eater.net/6502](https://eater.net/6502)).
