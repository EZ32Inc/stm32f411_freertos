# stm32f411_freertos
Basic FreeRTOS setup for popular blackpill (STM32F411 microcontroller based board).

In `main.c`:
- Main clock is set at 96MHz
- 2 tasks created based on led_task function to illustrate complex blinking pattern

## Instructions
- If your toolchain folder is not in global PATH variable then you need to create GCC_PATH variable with toolchain folder as value.
- `make all` 
- use your favourite tool to flash the device.


## For this to work with ESP32JTAG

After ESP32JTAG P3 of 3 lines SWD/SWCLK/GND is connected to target STM32F411, power on ESP32JTAG and then target board, run VSCode+Cortex-debug and use it to open this folder, press F5 to start download and debug.

