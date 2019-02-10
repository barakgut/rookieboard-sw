# RookieBoard SDK

## Debugging
Debugging and Flash programming are done by the SWD interface on the *STM32L071C8* via *FT2232H* using *OpenOCD*.

### OpenOCD
Use the *OpenOCD* clone at *utils* directory. *OpenOCD* build is *0.10.0+dev-00689-g6c2020eb-dirty (2019-02-09-17:42)*.
For build and install *OpenOCD* follow the *README* in OpenOCD's directory.
In './configure' stage make sure to put '--enable-ftdi' flag.

To run OpenOCD change to *utils/openocd* directory and run the following command:
```sh
sudo openocd -f board/rookieboard.cfg
```
In other shell open telnet by:
```sh
telnet localhost 4444
```
