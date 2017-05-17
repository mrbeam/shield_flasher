# shield_flasher
Flashing the Mr Beam shield via serial and a PCF8575 reset.

##Installation

```
cp autoreset /usr/bin
cp avrdude-autoreset /usr/bin
mv /usr/bin/avrdude /usr/bin/avrdude-original
ln -s /usr/bin/avrdude-autoreset /usr/bin/avrdude
```

##Usage

```
avrdude -q -V -p atmega328p -c arduino -b 115200 -P /dev/ttyAMA0 -U flash:w:grbl.hex:i
```