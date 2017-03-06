# chippro-vu-meter

# Installation
Requires
- python-alsaaudio
- CHIP_IO

# Usage

In order to work properly, the sunxi codec needs to be put into two channel "Mic1,Mic2" input mode.
To do this, run:

```
/sbin/modprobe sun4i-codec #if not built-in
/usr/sbin/alsactl restore #if not run by default
/usr/bin/amixer -c 0 cset numid=6 4 #set codec input mode
```

After that, you should be able to run the script!

Enjoy!
