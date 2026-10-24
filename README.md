# Embedded Systems Knowledge Base & Datasheet Repository

A curated technical reference library for embedded C firmware development on ARM Cortex-M microcontrollers (**STM32F4**, **STM32G0**, **STM32G4**, **STM32F7**) and peripheral ICs.

This repository serves as a centralized offline knowledge base containing official reference manuals, datasheets, programming guides, and application notes.

---

## Quick Navigation

### 1. MCU Datasheets (`mcu_datasheets/`)

| Target MCU | Package / Specs | Key Peripherals | Document Link |
| :--- | :--- | :--- | :--- |
| **STM32F401CC** | UFQFPN48 / Cortex-M4 @ 84 MHz, 256 KB Flash | ADC 12-bit, DMA, USART, SPI, I2C, USB FS | [STM32F401CC_Datasheet.pdf](mcu_datasheets/STM32F401CC_Datasheet.pdf) |
| **STM32G031F6** | TSSOP20 / Cortex-M0+ @ 64 MHz, 32 KB Flash | ADC 12-bit, Timers, USART, I2C, SPI | [STM32G031F6_Datasheet.pdf](mcu_datasheets/STM32G031F6_Datasheet.pdf) |
| **STM32G474** | LQFP48..128 / Cortex-M4F @ 170 MHz, Math Accel | HRTIM (Hi-Res Timer), Dual ADC, CORDIC, FMAC | [STM32G474_Datasheet.pdf](mcu_datasheets/STM32G474_Datasheet.pdf) |
| **STM32F767ZI** | LQFP144 / Cortex-M7 @ 216 MHz, 2 MB Flash | Dual Precision FPU, Chrom-ART, Ethernet, FMC | [STM32F767ZI_Datasheet.pdf](mcu_datasheets/STM32F767ZI_Datasheet.pdf) |

---

### 2. Core & Reference Manuals (`core_and_reference_manuals/`)

| Document ID | Title | Description | Document Link |
| :--- | :--- | :--- | :--- |
| **PM0214** | STM32 Cortex-M4 Programming Manual | Architecture, Thumb-2 ISA, NVIC registers, SysTick, FPU | [PM0214_Cortex_M4_Programming_Manual.pdf](core_and_reference_manuals/PM0214_Cortex_M4_Programming_Manual.pdf) |
| **PM0223** | STM32 Cortex-M0+ Programming Manual | Architecture, Thumb ISA, NVIC registers, SysTick for Cortex-M0+ (STM32G0) | [PM0223_Cortex_M0plus_Programming_Manual.pdf](core_and_reference_manuals/PM0223_Cortex_M0plus_Programming_Manual.pdf) |
| **RM0368** | STM32F401 Reference Manual | Detailed memory map, RCC clock tree, peripheral register maps (RCC, GPIO, TIM, ADC, DMA, I2C, USART) | [RM0368_STM32F401_Reference_Manual.pdf](core_and_reference_manuals/RM0368_STM32F401_Reference_Manual.pdf) |
| **RM0444** | STM32G0x1 Reference Manual | Full register reference for STM32G0 line (RCC, GPIO, EXTI, DMA, TIM, ADC, USART, I2C, SPI) | [RM0444_STM32G0x1_Reference_Manual.pdf](core_and_reference_manuals/RM0444_STM32G0x1_Reference_Manual.pdf) |
| **ES0334** | STM32F76xxx / F77xxx Device Errata | Silicon limitations, hardware bugs, and official ST workarounds | [ES0334_STM32F76xxx_Errata_Sheet.pdf](core_and_reference_manuals/ES0334_STM32F76xxx_Errata_Sheet.pdf) |
| **UM1725** | STM32F4 HAL and LL Drivers User Manual | STMicroelectronics official API reference for HAL & Low-Layer libraries | [UM1725_STM32F4_HAL_LL_Drivers.pdf](core_and_reference_manuals/UM1725_STM32F4_HAL_LL_Drivers.pdf) |
| **UM3083** | STM32G0 Series IEC 60730 / 61508 Self-Test Library | Class B functional safety library user guide (CPU, RAM, ROM, Watchdog diagnostics) | [UM3083_STM32G0_IEC60730_SelfTest_Library.pdf](core_and_reference_manuals/UM3083_STM32G0_IEC60730_SelfTest_Library.pdf) |

---

### 3. Development Boards (`development_boards/`)

| Board | Target MCU | Key Features | Document Link |
| :--- | :--- | :--- | :--- |
| **Nucleo-144** (UM1974) | STM32F767ZI / STM32F4 / STM32G4 | ST-LINK/V2-1 on-board debugger, Ethernet RJ45, USB OTG, Arduino Uno V3 & ST Zio headers | [UM1974_STM32_Nucleo_144_User_Manual.pdf](development_boards/UM1974_STM32_Nucleo_144_User_Manual.pdf) |
| **Nucleo-32** (UM2591) | STM32G031K8 | Compact form factor, ST-LINK/V2-1, Arduino Nano pinout | [UM2591_STM32G0_Nucleo_32_User_Manual.pdf](development_boards/UM2591_STM32G0_Nucleo_32_User_Manual.pdf) |

---

### 4. Sensors & Peripheral ICs (`sensors_and_ics/`)

| Component | Description | Interface | Document Link |
| :--- | :--- | :--- | :--- |
| **MPU-6050** | 6-axis MotionTracking (3-axis Gyroscope + 3-axis Accelerometer) | I2C (up to 400 kHz), Auxiliary I2C | [MPU6050_6Axis_IMU_Datasheet.pdf](sensors_and_ics/MPU6050_6Axis_IMU_Datasheet.pdf) |
| **CD4051** | Single 8-Channel Analog Multiplexer / Demultiplexer | 3-bit binary address (A, B, C) + Inhibit | [CD4051_8Ch_Analog_Multiplexer_Datasheet.pdf](sensors_and_ics/CD4051_8Ch_Analog_Multiplexer_Datasheet.pdf) |

---

### 5. University Guides (`university_guides/`)

| Document | Organization | Topic | Document Link |
| :--- | :--- | :--- | :--- |
| **LETI STM32F4 Laboratory Manual** | SPbETU "LETI" | CMSIS-based labs: GPIO, SysTick, TIM PWM, ADC+DMA, I2C OLED, USART | [LETI_STM32F4_Laboratory_Manual.pdf](university_guides/LETI_STM32F4_Laboratory_Manual.pdf) |

---

## Repository Structure

```
embedded-knowledge-base/
├── README.md
├── mcu_datasheets/
│   ├── STM32F401CC_Datasheet.pdf
│   ├── STM32G031F6_Datasheet.pdf
│   ├── STM32G474_Datasheet.pdf
│   └── STM32F767ZI_Datasheet.pdf
├── core_and_reference_manuals/
│   ├── ES0334_STM32F76xxx_Errata_Sheet.pdf
│   ├── PM0214_Cortex_M4_Programming_Manual.pdf
│   ├── PM0223_Cortex_M0plus_Programming_Manual.pdf
│   ├── RM0368_STM32F401_Reference_Manual.pdf
│   ├── RM0444_STM32G0x1_Reference_Manual.pdf
│   ├── UM1725_STM32F4_HAL_LL_Drivers.pdf
│   └── UM3083_STM32G0_IEC60730_SelfTest_Library.pdf
├── development_boards/
│   ├── UM1974_STM32_Nucleo_144_User_Manual.pdf
│   └── UM2591_STM32G0_Nucleo_32_User_Manual.pdf
├── sensors_and_ics/
│   ├── MPU6050_6Axis_IMU_Datasheet.pdf
│   └── CD4051_8Ch_Analog_Multiplexer_Datasheet.pdf
└── university_guides/
    └── LETI_STM32F4_Laboratory_Manual.pdf
```
