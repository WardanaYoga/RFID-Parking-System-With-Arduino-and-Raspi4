# RFID-to-Raspberry-Pi4

**SETUP RASPBERRY Pi**
1. sudo raspi-config
2. pilih interface options
3. pilih spi
4. pilih enable
5. pilih oke
6. cek spi apakah sudah ada lsmod | grep spi
7. jika tidak ada restart raspi dengan sudo reboot
8. lalu cek lagi

**INSTALASI LIBARY RFID MFRC522**
1. sudo apt update
2. sudo apt upgrade
3. python3 pip install spidev
   Pustaka spidev membantu menangani interaksi dengan SPI dan merupakan komponen kunci dalam tutorial ini karena kita membutuhkannya agar
   Raspberry Pi dapat berinteraksi dengan RFID RC522
4. python3 -m pip install mfrc522

SDA connects to Pin 24.
SCK connects to Pin 23.
MOSI connects to Pin 19.
MISO connects to Pin 21.
GND connects to Pin 6.
RST connects to Pin 22.
3.3v connects to Pin 1.
