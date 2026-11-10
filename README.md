STM32 Ethernet Communication with UDP (LwIP)
A simple Ethernet communication project for an STM32 board using
LwIP and the UDP protocol. The STM32 runs a UDP server and
reacts to messages received from a PC connected directly through an
Ethernet cable.
Project overview
The project demonstrates:
- Static IPv4 configuration on the STM32.
- Ethernet communication between a PC and an STM32 board.
- UDP server initialization with LwIP.
- Reception of UDP datagrams through an LwIP callback.
- GPIO control according to the received message.
When the first byte of a received UDP datagram is the character o, the
firmware sets GPIOI, GPIO_PIN_1. For any other first byte, it resets
that pin.
Hardware and software
Hardware
- STM32 board with an Ethernet MAC and a compatible Ethernet PHY.
- PC with an Ethernet port.
- Ethernet cable.
- Ethernet connection configured directly between the PC and STM32.
The exact STM32 board and PHY model should be added here if you want
the repository documentation to identify the hardware precisely.

Software
- STM32CubeIDE / STM32CubeMX
- STM32 HAL
- LwIP middleware
- Windows Command Prompt (for network tests)
This video can help.
Link : https://youtu.be/us_UEprqh2E
