# Suska-IV Atmega Firmware

The Source code of the AVR-Firmware is here: [Suska-Firmware git](https://github.com/umatthe/suska-firmware)<br>
Here You find a short [Userguide](https://github.com/umatthe/suska-firmware/blob/master/suska/doc/userguide.txt) to the Shell at the AVRUART<br>
This diectory contains the latest official binary.<br>
To update the AVR-Firware on Suska_IV-B:
- download binary [system-bf.hex](system-bf.hex)
- make sure that no SD-Card is inserted in the AVR-µSD-SLot
- avrdude -c avrispmkII -p m649 -U f:w:./system-bf.hex -P usb -F
