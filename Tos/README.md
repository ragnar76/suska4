# Suska-IV TOSTOOLS
Binaries of the useful TOS progams like UIPTOOL and TOSPATCH are located on the Suska-IV SDCard-Image.<p>
## ROM Collections (8MB with 16 512k TOS-Slots):<br>
[r-b4dbg.img](r-b4dbg.img) ETOS-Current 250927<br>
Generated using: __cat etoscurr.img etosdebug.img etosdebug.img etosdebug.img etosdebug.img etosdebug.img etosdebug.img etosdebug.img etosdebug.img etosdebug.img etosdebug.img etosdebug.img etosdebug.img etosdebug.img etosdebug.img  etoscli.img >r-b4dbg.img__<br>
OS-Switches:
<br>xx0000xxxx ETOS 250927
<br>xx1111xxxx ETOS 250927 CLI only on HDMI and MFP-UART (38400bd 8N1)
<br>xx0xx1xxxx ETOS 250927 Debug Output on MFP-UART (38400bd 8N1)
<br>xx1xx0xxxx ETOS 250927 Debug Output on MFP-UART (38400bd 8N1)
## Howto copy a Collection to the TOS-Flash
- copy Collection to µSD-Card (FAT 16/32)
- insert Card into µSD-Slot
- power up Suska-IV-B
- connect to AVR-Shell
- ls                                          (check if collection file is on card)
- f-erase all                                 (to erase the TOS Flash)
- ... wait for red LED to stop blinking ...
- f-write 0 r-b4dbg.img                       (writes Collection and boots when finished)
