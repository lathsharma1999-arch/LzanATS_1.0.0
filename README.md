# ATS Mini V4B Firmware (LzanATS)

Custom firmware for the ATS Mini V4B (16 MB flash) with ESP32-S3 and Si4732.
Version **LzanATS 1.0.0 (24NOV2026)**. Built with ESPHome.

## What's new
- Menu in 9 categories
- FT8 waterfall + message details (country, distance, bearing, SNR)
- Advanced DSP settings for FM and AM DXing
- Antenna auto-peak, live audio level meter
- RDS: RadioText+, programme type name, country code
- DX profile by default, radio boots as you left it
- Boot logo, About screen, IP address in menu
- More Home Assistant controls

## Features
FM, LW, MW, SW (2.3-26.1 MHz) with AM, LSB, USB and CW | FT8 on 9 bands |
RDS, LW/MW/SW station names with UTC schedules, Sri Lankan FM names |
60 favourites, DX log, Scan & Store, band scope | 4 themes, quiet mode |
Home Assistant, web page, hotspot, OTA update

## Files
| File | Use |
|---|---|
| LzanATS_1.0.0.factory.bin | Full image. Flash at address 0x0 over USB |
| LzanATS_1.0.0.ota.bin | Update file. Upload on the radio's web page |
| ATS_Mini_V4B_LzanATS_User_Guide.pdf | User guide |

## Install (USB)
esptool.py --chip esp32s3 write_flash 0x0 LzanATS_1.0.0.factory.bin

## Update (WiFi)
Open http://RADIO-IP-ADDRESS and upload the .ota.bin file.
