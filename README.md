# uos3-receiver-server

## Planned Features

* rtl_tcp (SDR# compatible) output on port 1234 (8-bit I/Q, upsampled to 250KS/s)
* Full quality output on port 1235 (16-bit I/Q, native 192KS/s) 
* Seperate local port (1236?) for authenticated control of gain settings.

## TODO

* Sample chunks of 192 * 2 channel * 16-bit frames
* Resample to chunks of 250 * 2 * 8 for SDR# compatibility (0.25 MSPS)
  * Should also be compatible with websdr
* TCP Server outputs (circular buffer feed of chunks)
* Integrate FCDPP control on local UDP(?) port

## Authors

* Phil Crump <phil@philcrump.co.uk>
