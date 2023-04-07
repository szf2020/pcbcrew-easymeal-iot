# PCBCrew Easymeal IoT

SP32 based vending machine controller board with Ethernet, Wi-Fi, and 4G LTE connectivity

| 3D Preview                                                     | PCBA                                                       |
| -------------------------------------------------------------- | ---------------------------------------------------------- |
| ![pcbcrew-easymeal-iot-3d-preview](./doc/image/3d-preview.png) | ![pcbcrew-easymeal-iot-pcb-assembly](./doc/image/pcba.png) |

* ESP32-S3
* Wiznet W5500 Ethernet Controller
* Mini-PCIe connector for a Quectel/Simcom 4G LTE module
* RS232 UART port via push-pull connector
* Dual MDB connectors for vending macine interfacing
* On-board backup 18650 battery holder and charger
* DS1337 RTC and CR2032 battery holder
* DIP8 connector for 24Cxx EEPROM
* A few buttons and LEDs
* USB 2.0 Type-C connector for debugging

## Pin Assignments

### Quectel EC25

| Modem         | PCIe    | ESP32-S3 |
| ------------- | ------- | -------- |
| MODEM_RST     | PCIE_22 | GPIO_35  |
| MODEM_UART_TX | PCIE_13 | GPIO_44  |
| MODEM_UART_RX | PCIE_11 | GPIO_43  |
| MODEM_RTS     | PCIE_25 | GPIO_39  |
| MODEM_CTS     | PCIE_23 | GPIO_40  |

### Simcom SIM7600

(todo)
