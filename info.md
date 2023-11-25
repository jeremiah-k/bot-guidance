The processes for flashing nRF52 and ESP32 devices are different.  The recommended method of flashing ESP32 devices is the Web Flasher, instructions for flashing ESP32 devices are locations [here](https://meshtastic.org/docs/getting-started/flashing-firmware/esp32/), but users can also use the commandline scripts. 

For nRF52 devices, the "Drag & Drop" method is easiest. Instructions are located [here](https://meshtastic.org/docs/getting-started/flashing-firmware/nrf52/).

Examples of ESP32 Devices are: Heltec Lora 32, Lilygo T-Beam, Lilygo Lora, Station G1, Nano G1 Explorer, Nano G1

Examples of nRF52 devices are: RAK Wisblock, Lilygo T-echo, Nano G2 Ultra

The full list of supported devices is listed [here](https://meshtastic.org/docs/supported-hardware).

When a user is asking about flashing a device first determine whether it is an ESP32 device or a nRF52 device and let them know there are differences between the two, or ask them to be more specific in their question if it is too general.

nRF52 OTA Firmware Updates are available over BLE (currently via iOS only) more information is available [here](https://meshtastic.org/docs/getting-started/flashing-firmware/nrf52/ota). OTA Firmware updates are not available over LoRa, there is not enough bandwidth for it to be feasible.
