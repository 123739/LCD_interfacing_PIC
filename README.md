# LCD_interfacing_PIC
This project demonstrates how to interface a 16x2 character LCD with the PIC18F4520 microcontroller

# 16x2 LCD Interfacing with PIC18F4520

## Description
This project demonstrates how to interface a 16x2 character LCD with the PIC18F4520 microcontroller using Embedded C. The LCD is operated in **4-bit mode** to save GPIO pins, and the code is written using **MPLAB X** and compiled with the **XC8 compiler**. Custom messages are displayed on the screen.

## Tools & Components Used
- **Microcontroller**: PIC18F4520  
- **LCD**: 16x2 Alphanumeric LCD (HD44780 compatible)  
- **Compiler**: MPLAB X IDE with XC8  
- **Simulation**: Proteus (optional)  
- **Other**: Potentiometer (for contrast), Resistors, Wires, Breadboard

## Key Concepts Covered
- LCD interfacing
- Command/data transmission logic
- Delay handling
- Pin-level control and timing
- Embedded C programming using XC8

## Project Structure
├── LCD.c (Source code)
├── LCD_PIC_simulation.mp4 (Project Simulation)
├── LCD_PIC.pdsprj (Proteus file)


## ⚙️ How It Works
The LCD is controlled using 6 GPIO pins:
- **RS** – Register Select
- **RW** – Read/Write (often tied to GND for Write-only mode)
- **EN** – Enable pin

The program initializes the LCD, sends commands to set it up in 4-bit mode, and then displays a series of strings (e.g., `"Hello, Anwesha!"`, `"PIC18F4520 LCD"`).

## How to Run
1. Clone/download the repository.
2. Open `main.c` in MPLAB X IDE.
3. Compile using the XC8 compiler.
4. Load the hex file into Proteus or burn to the PIC18F4520 hardware.
5. Observe the LCD display the intended message.

## Notes
- Ensure proper delays between sending command and data.
- You can expand this project by adding scrolling text, sensor values, or dynamic updates.
  
Feel free to fork this project and modify it to build multi-screen displays or integrate with keypad/memory modules.
