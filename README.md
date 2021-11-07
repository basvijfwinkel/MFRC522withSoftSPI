# MFRC522withSoftSPI
MFRC522 library with SoftSPI support so you can use any digital pin on the Arduino.

You can set the pin you would like to use in MFRC522.cpp
const uint8_t SOFT_SPI_MISO_PIN = 4; // Hardware pin Arduino Nano = 12
const uint8_t SOFT_SPI_MOSI_PIN = 3; // Hardware pin Arduino Nano = 11
const uint8_t SOFT_SPI_SCK_PIN  = 2; // Hardware pin Arduino Nano = 13

And you can use the library in the same way as the original MFRC522 library without any code changes.
#define RST_PIN  5 // (Hardware pin Arduino Nano = 9)
#define SS_PIN   6 // (Hardware pin Arduino Nano  = 10)
MFRC522 mfrc522(SS_PIN, RST_PIN);
