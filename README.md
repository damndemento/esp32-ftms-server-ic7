# esp32-ftms-server-ic7

This is an ESP-32 based ftms-sensor that I edited for my Schwinn IC7 bike. Originally built for [jamesjmtaylor's](https://github.com/jamesjmtaylor/esp32-ftms-server)
 stationary bike stand.  It uses the [Indoor Bike Data characteristic](https://www.bluetooth.com/wp-content/uploads/Sitecore-Media-Library/Gatt/Xml/Characteristics/org.bluetooth.characteristic.indoor_bike_data.xml) of the FTMS BLE service.

I used platformio plugin for VSCode to compile and upload the firmware to a [D1 mini ESP32](https://www.az-delivery.de/en/products/esp32-d1-mini#product-descriptions)

I added two 1k resistors:
  one soldered to GPIO27 and one to the GND next to it to avoid breaking the board.

Then I splitted a [0.5m 3.5mm mono cable](https://www.amazon.de/gp/product/B011SSAUM0/ref=ppx_yo_dt_b_asin_image_o07_s00?ie=UTF8&psc=1) into half and connected the wires again and soldered them to the resistors on the board.

![resistors](https://github.com/damndemento/esp32-ftms-server-ic7/blob/main/D1_resistors.jpg)

![resistor pins](https://github.com/damndemento/esp32-ftms-server-ic7/blob/main/D1_resistor_pins.jpg)

![cables](https://github.com/damndemento/esp32-ftms-server-ic7/blob/main/D1_with_cables.jpg)
