# Suska-IV FPGA Configuration

Here You will find new Corefiles to update the Suska-IV-B when available.
Coretype | Version | Download Link | md5sum
--- | --- | --- | ---
Suska4-Falcon-B | 20251224 | [SUSKA_IV_B_FALCON_2K25B.rbf](SUSKA_IV_B_FALCON_2K25B.rbf) | 8e9add40c6a36248421fad1fe18b0461
Suska4-Falcon-B | 20251224 | [SUSKA_IV_B_FALCON_2K25B.sof](SUSKA_IV_B_FALCON_2K25B.sof) | 5acee7f3f9629a35ed6b0fa86719737a
Suska4-Falcon-B | 20251224 | [SUSKA_IV_B_FALCON_2K25B.pof](SUSKA_IV_B_FALCON_2K25B.pof) | 163141c34460035f4fa200f675d119cc


## Howto install
- sof - Files can be loaded for trial without permanent changes to the system. They are loaded to the FPGA using the JTAG Connnector and the Quartus SW
- pof - Files are loaded into the Configflash of the board, deleting the old Core. They are loaded to the ConfigFlash using the AS Connnector and the Quartus SW
## Do not use the rbf-File in case as-getid returns: Silicon-ID: 17 ** unknown **<br>Update the Firmware first: [AVR-Firmware](../Firmware/)
- rbf - Files are loaded into the Configflash of the board, deleting the old Core. See the [howto-rbf](howto-rbf.txt) for details.

## What is new in the last version 2K25B (251224)
- MMU/Cache - fixes: Mint030 works now with memory protection and Cache
- Cache temporally reduced to 256 byte Instruction and Data (will be set to 4k again later) 
