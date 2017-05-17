# shield_flasher
Flashing the Mr Beam shield via serial and a PCF8575 reset.

```
cp autoreset /usr/bin
cp avrdude-autoreset /usr/bin
mv /usr/bin/avrdude /usr/bin/avrdude-original
ln -s /usr/bin/avrdude-autoreset /usr/bin/avrdude
```