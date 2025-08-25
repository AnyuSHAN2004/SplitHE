# HE Split Keyboard Prototype

Hi there 

This repo contains the design files for my **Hall Effect (HE) split keyboard prototype**.  
I’m documenting and sharing the PCB work here in case it helps others, or if you’d like to give feedback / build on the design.  

---

## What’s Inside
- **altium files** → Altium 24.5.2 project files (schematics + PCB).  
  - These are the original source files.  
- **Split_Int.pdf** → exported schematic PDF (for anyone without Altium).  
- **/images/** → reference screenshots (layout views, schematics highlights, close-ups of RP2040 circuitry).  

---

## Quick Notes
- **MCU**: RP2040 (first time I’ve designed a custom MCU circuit, no breakout boards).  
- **Peripherals**: Hall Effect sensor → multiplexer → RC filter → OPA buffer → ADC.  
- **Board**: 4-layer, with solid inner ground planes.  
- **Connectors**:  
  - Top-right USB-C → real USB.  
  - Bottom-right USB-C → dummy connector for UART + power between halves.  
- **Power**: 5 V from USB → LDO down to 3.3 V.  
- **Analog power**: filtered from digital 3.3 V with ferrite bead + decoupling cap.  

---

## License
Currently released under the **MIT License** — see [LICENSE](LICENSE) for details.  
This means you’re free to use, modify, and redistribute the design. Attribution is appreciated.  

---

## Feedback
This is still an early prototype. I welcome any suggestions or pull requests, especially around:  
- RP2040 circuitry (USB, flash, oscillator, decoupling).  
- PCB layout improvements.  
- General design sanity checks.  

---

Thanks for checking this out, and happy hacking!  
