# FTMS for Schwinn IC7 indoor cycling spinning bikes

This is an ESP-32 based ftms-server which I edited for my Schwinn IC7 bike. Originally built for [jamesjmtaylor's](https://github.com/jamesjmtaylor/esp32-ftms-server)
 stationary bike stand.  It uses the [Indoor Bike Data characteristic](https://www.bluetooth.com/wp-content/uploads/Sitecore-Media-Library/Gatt/Xml/Characteristics/org.bluetooth.characteristic.indoor_bike_data.xml) of the FTMS BLE service.

I used platformio plugin for VSCode to compile and upload the firmware to a [D1 mini ESP32](https://www.az-delivery.de/en/products/esp32-d1-mini#product-descriptions)

I added two 1k resistors:
  one soldered to GPIO27 and one to the GND next to it to avoid breaking the board.

![resistor pins](https://github.com/damndemento/esp32-ftms-server-ic7/blob/main/D1_resistor_pins..jpg)

Then I splitted a [0.5m 3.5mm mono cable](https://www.amazon.de/gp/product/B011SSAUM0/ref=ppx_yo_dt_b_asin_image_o07_s00?ie=UTF8&psc=1) into half and drilled the wires together and soldered them to the resistors on the board.

![resistors](https://github.com/damndemento/esp32-ftms-server-ic7/blob/main/D1_resistors.jpg)

This is how it looks like

![cables](https://github.com/damndemento/esp32-ftms-server-ic7/blob/main/D1_with_cables.jpg)

Then you can connect it to your bike without harming the IC7 - just disconnect the display from the sensor and plug the D1 mini ESP32 in between - et voilá - your IC7 speaks FTMS now.

Ready to connect to Zwift, WahooRGT or similar...

actually it is powered with 5v via the usb jack - but I'm planning to add a rechargable battery and a shield for charging... and last but not least a little case to fit.

 have fun!
