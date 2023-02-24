# pico-ice-zephyr

Basic Setup (for Linux):

Follow this guide from Zephyr for a global installation up until the "build blinky" part:
https://docs.zephyrproject.org/latest/develop/getting_started/index.html

Extract the Zephyr SDK from above guide in $HOME so resulting path would be: $HOME/zephyr-sdk-X.XX.X

In your location of choice run the following commands:

 - sudo west init -m https://github.com/josuah/pico-ice-zephyr pico-ice-zephyr
 - cd pico-ice-zephyr
 - west update
 - west build pico-ice-zephyr --board=rpi_pico
 
 This should produce a zephyr.UF2 file located in ../pico-ice-zephyr/build/zephyr/
 
 To flash, copy the UF2 file to the pico storage.
