# Alpaca-OwO

Obtainable w/ rOna I/O board.

![Alpaca-OwO-front](./assets/Alpaca-OwO-front.webp)

## Features

- Familiar form factor
- Removable screw terminals makes reconnecting buttons more convenient
  - Tool-less spring terminal option available (when using Phoenix 1952348)
- Rich I/O
  - Analog stick port
  - Simultaneous access to hardware SPI, I2C and basic UART via EXT port
  - SparkFun Qwiic/Adafruit STEMMA-QT compatible I2C quick connect port
  - Possibility to support various proprietary gamepad/joystick interfaces with RP2040 PIO and spare GPIO on EXT port

## Pin assignments

Below is the preferred pin assignment for this board. Note that every pin can be remapped or re-purposed when necessary and this list only serves as a guideline. Still, follow this list when developing firmware if you wish to keep wiring compatibility with other fightstick PCBs and preserve the meaning of the silk screens.

### Pluggable terminal ports

| RP2040 Pin | GP2040 Pin | Label | Purpose |
| ---------- | ---------- | ----- | ------- |
| 0 | DPad Down | D | D-Button Down |
| 1 | DPad Up | U | D-Button Up |
| 2 | DPad Left | L | D-Button Left |
| 3 | DPad Right | R | D-Button Right |
| 4 | A1 | PS | PS Button |
| 5 | S1 | SHR | Share Button |
| 6 | S2 | OPT | Option Button |
| 7 | B3 | SQR | Square Button |
| 8 | B4 | TRI | Triangle Button |
| 9 | R1 | R1 |R1 Button |
| 10 | L1 | L1 | L1 Button |
| 11 | B1 | XRO | Cross Button |
| 12 | B2 | CIR | Circle Button |
| 13 | R2 | R2 | R2 Button |
| 14 | L2 | L2 | L2 Button |

### Ext port, I2C quick connect and analog stick port

| RP2040 Pin | GP2040 Pin | Label | Purpose |
| ---------- | ---------- | ----- | ------- |
| 15 | A2 | TP | Touchpad Click Button |
| 16 | - | DI | SPI0 DI |
| 17 | - | CS | SPI0 CS |
| 18 | - | CLK | SPI0 CLK |
| 19 | - | DO | SPI0 DO |
| 20 | - | TX | UART1 TX |
| 21 | - | EXT/RX | UART1 RX |
| 22 | R3 | R3 | R3 Button |
| 23 | L3 | L3 | L3 Button |
| 24 | Display | SDA | I2C0 SDA |
| 25 | Display | SCL | I2C0 SCL |
| 26/ADC0 | - | RY | Analog Stick RY |
| 27/ADC1 | - | Stick/RX | Analog Stick RX |
| 28/ADC2 | - | LY | Analog Stick LY |
| 29/ADC3 | - | LX | Analog Stick LX |

## Terminal block options

Any pluggable terminal block plugs that mate with a Phoenix MINI COMBICON MC terminal block header should be usable with Alpaca-OwO. Notable configurations include the [basic screw terminal (1840447)](https://www.phoenixcontact.com/en-us/products/pcb-plug-mc-1510-st-35-1840447), the [tool-less spring terminal (1939989)](https://www.phoenixcontact.com/en-us/products/pcb-plug-fk-mcp-1510-st-35-1939989) and the [low profile spring terminal (1952348)](https://www.phoenixcontact.com/en-us/products/pcb-plug-fmc-1510-st-35-1952348). Generic replacements of these connectors can be found on Aliexpress or LCSC. Note that the locking variants will not fit and thus not supported.
