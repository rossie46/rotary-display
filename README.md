# rotary-display
Rotary encoder and display for controlling home-assistant entities
This Build includes a 3D printed case , wemos_D1_mini , rotary encoder and an ssd1306 OLED display module.
it is programmed via esp-home whic inturn controls and displays the values of homeassistant entities.
menu and sub menu system is supported so that you can categorize and organize the items in menu.

#### USE THE GITHACK HOSTED MENU GENERATOR FOR EASY FIRMWARE BUILD: 
            https://rawcdn.githack.com/mikosoft83/pithy_screen_menu_system/a62acf32be99deb8db09b108542ffee5c1e66067/menu_generator/index.html

The controller consist of:
1. Wemos_D1_mini                           you can use any esp8266 module
2. SSD1306                                 https://cdn-shop.adafruit.com/datasheets/SSD1306.pdf
3. Rotary encoder                          https://www.addicore.com/products/rotary-encoder-with-push-switch
4. TTP223 capacitive touch switches * 2    https://www.amazon.com/Anmbest-2-5-5-5V-Capacitive-Self-Lock-No-Lock/dp/B07K72N79J
5. 3D printed case

WIRING INSTRUCTIONS
*  encoderPinA    : D5
*  encoderPinB    : D6
*  encoderSwitch  : D7
*  i2cData        : D1
*  i2cClock       : D2
*  button1        : D3
*  button2        : TX

After wiring the connections, make sure you short out button1 pad A and button2 pad B for optimal working.
else D3 will be pulled down so that the esp goes to flash mode. The ttp223 module pulls down the connected gpio.
Or you can use a different pin if available.



Alternatiely you can use a menu system generator from https://github.com/mikosoft83/pithy_screen_menu_system
there is also a githack hosted version where you can easily add menu and items. I prefer doing so. https://rawcdn.githack.com/mikosoft83/pithy_screen_menu_system/a62acf32be99deb8db09b108542ffee5c1e66067/menu_generator/index.html
