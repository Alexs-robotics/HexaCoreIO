# HexaCoreI/O
The HexaCoreIO PCB is a robust, multifunctional controller designed specifically for hexapod robots. It integrates essential functionalities such as servo control, power distribution, and communication interfaces into a single, efficient board. This board is ideal for robotics enthusiasts, researchers, and engineers who require high performance and scalability. DMA is supported.
# Specifications
![alt text](https://github.com/Alexs-robotics/HexaCoreIO/blob/main/System%20Overview.png?raw=true)

Microcontroller: STM32H730ZBT6
Power Distribution: <b/>
- Integrated power lines of maximum 15V supporting up to 5A per servo channel. <b/>
- Safe input voltage range: 15V (safe max), 20V (absolute max). <b/>

<a/> Servo Control: <b/>
- 21 PWM channels for servos, Powered by dual PCA9685 ICs. <b/>

<a/> Sensors: <b/>
- 21 x ACS712 current sensors for servo power monitoring (5A max per sensor). <b/>

<a/> Storage: <b/>
- MicroSD card slot supporting SDMMC1 interface. <b/>

<a/> Communication Interfaces: <b/>
- I2C, SPI, UART, CAN, and Ethernet. <b/>
- I2S for audio or data streaming. <b/>

<a/> Peripheral Support: <b/>
- Integrated NRF24L01+ module for wireless communication. <b/>
- Quad-SPI for external flash and RAM (up to 125 MB). <b/>

<a/> Debugging and Programming: <b/>
- SWD (Serial Wire Debug) interface. <b/>

<a/> Other Features: <b/>
- Onboard LEDs for status indication. <b/>
- Analog multiplexer for additional signal routing. <b/>

# Description
The HexaCoreIO is a high-performance main controller board tailored for complex robotics applications like hexapods. The board includes the STM32H730 microcontroller, offering powerful computational capabilities while maintaining energy efficiency. The integrated power lines, rated at 5A per channel, ensure reliable and consistent power delivery to up to 21 servos simultaneously.
Each servo channel includes a dedicated ACS712 current sensor, enabling real-time current monitoring for advanced diagnostics and feedback control. The board's robust storage capabilities include both MicroSD and Quad-SPI flash support for large datasets, making it suitable for AI-driven robotics.

For communication, HexaCoreIO supports multiple protocols, including I2C, SPI, UART, and Ethernet, ensuring seamless integration into diverse robotic systems. The NRF24L01+ module further enhances the system's capabilities by offering reliable wireless communication.

With integrated debugging interfaces and onboard LEDs, HexaCoreIO is also designed to simplify development and troubleshooting. Its modular and expandable architecture makes it a future-proof choice for robotics projects.

Applications
Hexapod and multi-legged robotic systems.
Advanced robotic arms requiring precise servo control.
Research projects involving real-time data monitoring and feedback.
AI-enabled robotic platforms.
Getting Started
Power Supply: Connect a regulated 5V power source to the input pins. Ensure the current capacity matches your servo requirements.
Servo Connection: Plug in your servos to the PWM pins. Each channel supports up to 5A.
Microcontroller Programming: Use the SWD interface for programming and debugging with STM32CubeIDE or similar tools.
Expand Functionality: Connect sensors, wireless modules, or additional peripherals using I2C, SPI, UART, or Ethernet.

# License
This design is open-source under the Apache Version 2.0 License. Contributions and modifications are encouraged!

# TO-DO

- Drivers
- Testing code
