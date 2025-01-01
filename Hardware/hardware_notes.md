# Hardware Connections

## Connecting ESP01 WiFi Module to the Microcontroller
The ESP01 communicates using the UART protocol, requiring TX and RX lines to be connected to the microcontroller.

### Connections:
- **ESP01 TX** → **PD5 (RX)** of the microcontroller  
- **ESP01 RX** → **PD6 (TX)** of the microcontroller (through a voltage divider to step down 5V to 3.3V for compatibility)  
- **ESP01 VCC** → **3.3V power source**  
- **ESP01 GND** → **GND**  
- **ESP01 CH_PD** → **VCC (3.3V)** to enable the module  

---

## Connecting the LCD to the Microcontroller
The LCD is configured in 4-bit mode to reduce pin usage.

### Pin Assignments:
- **LCD RS** → **PD7**  
- **LCD EN** → **PD6**  
- **LCD D4** → **PD5**  
- **LCD D5** → **PD4**  
- **LCD D6** → **PD3**  
- **LCD D7** → **PD2**  
- **LCD VCC** and **GND** → Connected to a **5V power source** and **GND**  
- **LCD V0 (contrast pin)** → Connected via a **10K potentiometer** to adjust contrast  

This setup allows the LCD to operate efficiently with minimal GPIO usage.
