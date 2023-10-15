The *kernel* is a computer program that is at the core of a computer's [[operating system]]. It has complete control over everything that occurs in the system. [^1]

The *kernel* interacts with the [[shell]] and other programs, as well as the computer's [[hardware]], including the [[processor]], [[memory]], and disk drives. [^1] 

Kernel parameters can be accessed through a pseudo [[file system]] `/sys`
```bash
cat /sys/class/input/mouse0/device/name
Logitech USB Optical Mouse
cat /sys/class/hwmon/hwmon3/temp1_crit
120000
cat /sys/class/leds/input2::scrolllock/brightness
0
```
- Some system variables can be changed on the fly
```bash
sudo bash -c "echo 1 > /sys/class/leds/input2::scrollock/brightness"
```
[^1]: https://www.linfo.org/kernel.html