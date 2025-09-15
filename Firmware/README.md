# Suska-IV Atmega Firmware

To update the AVR-Firware on Suska_IV-B:
- download binary [system-bf.hex](system-bf.hex)
- make sure that no SD-Card is inserted in the AVR-µSD-SLot
- avrdude -c avrispmkII -p m649 -U f:w:./system-bf.hex -P usb -F
