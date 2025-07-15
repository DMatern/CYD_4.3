# CYD_4.3
Basic Code to drive the CYD 4.3" Capacitive Touch display hardware

# Key Features and Specifications:

	Microcontroller: 	ESP32-S3, a dual-core 32-bit processor with Wi-Fi and Bluetooth capabilities.
	Display: 					4.3-inch IPS TFT LCD with 800x480 resolution.
	Touch: 						Capacitive touchscreen for user interaction.
	Storage: 					16MB Flash and 8MB PSRAM.
	Connectivity: 		Supports Wi-Fi 802.11b/g/n/e/i and Bluetooth 4.2.
	Interfaces: 			UART, SPI, I2C, PWM, ADC, DAC, and more.
	Other Features: 	TF card slot, USB Type-C port. 

# Drivers

> General

	4Display			= TFT_eSPI / Bodmer https://github.com/Bodmer/TFT_eSPI
 	Touchscreen   = XPT2046 / PaulStoffergen
	NeoPixel      = FastLED
	WiFi          = WiFi.h  (arduino ESP32 core)
	BlueTooth     = BLE 	(Arduino ESP COre) https://github.com/nkolban/esp32-snippets/blob/master/cpp_utils/tests/BLE%20Tests/SampleServer.cpp
 	TF Card       = SD.h    (arduino core)
	Flash Memory  = SPIMemory / Marzogh

> Connectors
	
	Header P1 (4 pins) (UART): Gnd, Rx, Tx, +5V
	Header P2 (4 pins) (SPI): IO13, IO12, IO11, IO10
	Header P3 (4 pins) (USB/UART): IO20, IO19, IO18, IO17
	Header P4 (4 pins) : IO18, IO17, +3.3v, Gnd

> Pin	Usage

	GPIO 0	BOOT_BTN
	GPIO 1	LCD_B4
	GPIO 2	TFT_BL
	GPIO 3	LCD_B1
	GPIO 4	LCD_G5
	GPIO 5	LCD_G0
	GPIO 6	LCD_G1
	GPIO 7	LCD_G2
	GPIO 8	LCD_B0
	GPIO 9	LCD_B3
	GPIO 10	SD_CS
	GPIO 11	SD_MOSI
	GPIO 12	SD_SCK
	GPIO 13	SD_MISO
	GPIO 14	LCD_R4
	GPIO 15	LCD_G3
	GPIO 16	LCD_G4
	GPIO 17	NC
	GPIO 18	CTP_INT*
	GPIO 19	CTP_SDA
	GPIO 20	CTP_SCL
	GPIO 21	LCD_R3
	GPIO 33	NA
	GPIO 34	NA
	GPIO 35	NC / NA
	GPIO 36	NC / NA
	GPIO 37	NC / NA
	GPIO 38	CTP_RST
	GPIO 39	LCD_HSYNC
	GPIO 40	LCD_DE
	GPIO 41	LCD_VSYNC
	GPIO 42	LCD_PCLK
	GPIO 43	U0TXD
	GPIO 44	U0RXD
	GPIO 45	LCD_R0
	GPIO 46	LCD_B2
	GPIO 47	LCD_R2
	GPIO 48	LCD_R1

## 📘 Documentation  

[CYD Specifacations](./ESP32-4827S043%20Specifications.pdf)

[CYD Board Layout](./Board%20Layout.pdf)

