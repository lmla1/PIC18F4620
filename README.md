# PIC18F4620 Projects

This repository contains a collection of **C and header (.h) files** for various applications using the **PIC18F4620** microcontroller. The projects are developed for Linux using `pk2cmd` to program the microcontroller.

## About the PIC18F4620
The **PIC18F4620** is an 8-bit microcontroller from **Microchip** featuring:
- 40MHz maximum operating frequency (with 10 MIPS performance)
- 64KB Flash Program Memory
- 3.3KB RAM
- 1KB EEPROM
- Multiple I/O ports with **LAT** registers for better output control
- Integrated **USART, SPI, I²C** for serial communication

📄 **[PIC18F4620 Datasheet](https://ww1.microchip.com/downloads/aemDocuments/documents/OTH/ProductDocuments/DataSheets/39626e.pdf)**

## Programming the PIC18F4620 with `pk2cmd`
To program the **PIC18F4620** on Linux using a **PICkit2** programmer, use the following command:

```bash
pk2cmd -M -PPIC18F4620 -F firmware.hex
```

### **Basic Commands:**
- **Erase the PIC:**
  ```bash
  pk2cmd -E -PPIC18F4620
  ```
- **Verify the programmed firmware:**
  ```bash
  pk2cmd -V -PPIC18F4620 -F firmware.hex
  ```
- **Read back the program memory:**
  ```bash
  pk2cmd -R -PPIC18F4620 -F readback.hex
  ```

📌 **More details on `pk2cmd`:** [GitHub Repository](https://github.com/psmay/pk2cmd)

## Repository Contents
This repository includes:
- **.c and .h files** for various PIC18F4620 applications
- Example configurations for **GPIO, UART, ADC, Timers, and Interrupts**
- Sample code snippets to simplify embedded development

## Contributing
Feel free to contribute by adding new features or fixing bugs. Open an issue or submit a pull request!

---
🚀 **Happy coding with the PIC18F4620!**
