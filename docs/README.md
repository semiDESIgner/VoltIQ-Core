 USB-C IN ──> Charger/BMS ──> Battery ──> Boost 5V ──> Load Output (USB-C VBUS)
                      │                 │
                      │                 ├─> Current sense (CHG/DSG) ──> ESP32 ADC
                      │                 └─> Battery voltage divider ──> ESP32 ADC
                      │
                      └─> NTC temp ────────────────────────────────> ESP32 ADC

 ESP32 ──SPI──> TFT LCD
 ESP32 ──GPIO─> MOSFET/Relay control (power path / load switching)
