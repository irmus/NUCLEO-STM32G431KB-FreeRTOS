## new_task

Create a FreeRTOS task **WITHOUT** using CubeMX. 

There are two tasks in this example. The first is *defaultTask* generated by CubeMX. It runs on 1s interval and always turn on on-board LED. The second is *offTask* defined by source code in main.c file. This task runs on 1.1s interval and always turn off on-board LED. Difference in interval makes harmonics at blinking timing of LED.

### CubeMX Settings
- Project is generated with STM32CubeIDE
  - Pinout & Configuration
    - System Core
      - SYS
        - Debug : Trace Asynchronous Sw
        - Timebase Source : TIM17
    - Middleware
        - FREERTOS
        - Interface : CMSIS_V2
        - Advanced settings
            - USE_NEWLIB_REENTRANT : Enabled
  - Project Manager
    - Code Generator
      - [x] Generate peripheral initialization as a pair of '.c/.h' files per peripheral

