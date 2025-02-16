# Installing Custom Arduino Board

## Prerequisites
- Arduino IDE 1.6.4 or later
- Working internet connection

## Installation Steps

1. Open Arduino IDE

2. Navigate to Preferences
   - File > Preferences (Windows/Linux)
   - Arduino > Preferences (macOS)

3. Add Custom Board Manager URL
   - In "Additional Board Manager URLs" field, paste:
     `https://raw.githubusercontent.com/Mister-Industries/arduino-board-index/refs/heads/main/package_tiny_core_index.json`
   - For multiple URLs, separate with commas

4. Open Board Manager
   - Tools > Board > Boards Manager
  
5. Install ESP32 Boards/Tools
   - Search for `esp32`
   - Select `esp32` package (v3.1.1) by Espressif 
   - Click "Install"

5. Install iotaCore Custom Board
   - Search for `tinyCore`
   - Select `tinyCore ESP32 Boards` package (v2.0.0) by MR.INDUSTRIES 
   - Click "Install"

6. Select Board
   - Tools > Board > Select `tinyCore ESP32-S3 No PSRAM`
   - Make sure Upload Mode is set to `UART0 / Hardware CDC`
   - Make sure USB Mode is set to `Hardware CDC and JTAG`

## Troubleshooting
- Verify URL is correct and accessible
- Check internet connection
- Restart Arduino IDE if installation fails
- Ensure you have the latest Arduino IDE version

## Support
Send us an email at support@mr.industries or join our [Discord](https://discord.gg/hvJZhwfQsF) for help!
