# Suska-IV FPGA Configuration
Here You will find new Corefiles to update the Suska-IV-B when available.

## Howto install
- sof - Files can be loaded for trial without permanent changes to the system. They are loaded to the FPGA using the JTAG Connnector and the Quartus SW
- pof - Files are loaded into the Configflash of the board, deleting the old Core. They are loaded to the ConfigFlash using the AS Connnector and the Quartus SW
## For now do not use the rbf-File in case as-getid returns: Silicon-ID: 17 ** unknown **
- rbf - Files are loaded into the Configflash of the board, deleting the old Core. See the [howto-rbf](howto-rbf.txt) for details.

## What is new in the last version 2K25B (251224)
- MMU/Cache - fixes: Mint030 works now with memory protection and Cache
- Cache temporally reduced to 256 byte Instruction and Data (will be set to 4k again later) 

