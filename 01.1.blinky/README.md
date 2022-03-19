## blinky

Simple blinky example with FreeRTOS.

Default task loops with 1s delay and toggles on board LED.

### CubeMX Settings
- Project is generated with STM32CubeIDE
  - Pinout & Configuration
    - System Core
        - SYS
        - Timebase Source : TIM17
    - Middleware
        - FREERTOS
        - Interface : CMSIS_V2
        - Advanced settings
            - USE_NEWLIB_REENTRANT : Enabled
  - Project Manager
    - Code Generator
      - [x] Generate peripheral initialization as a pair of '.c/.h' files per peripheral

