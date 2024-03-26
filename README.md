# HMC5883-RK356x-driver
driver for HMC5883 3-Axis Digital Compass IC on RK356x

### hmc5883.h
driver file with notes.

### hmc5883.c
The demo program which can print the raw data from the hmc5883's register.

usage:
```bash
gcc hmc5883.c -o hmc5883
./hmc5883 /dev/i2c-5
```
you can change the i2c device from 5 to what you want.

### readGs.c
The demo program which can print the mag data processed rom the hmc5883's register. Using 15Hz, 001(1090Lsb/Gs)config.

usage:
```bash
gcc readGs.c -o readGs
./readGs /dev/i2c-5
```

## TODO
Add an easy-to-use feature for adjusting measure range.
