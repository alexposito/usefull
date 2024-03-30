# Linux
## Block HID USB
A way to protect against Rubber Ducky.

Create a file, for example: `/etc/udev/rules.d/50-USBHID.rule`

Write the following there: `SUBSYSTEMS=="usb", DRIVERS=="usbhid", ACTION=="add", ATTR{authorized}="0"`

More info:

https://revolutionpi.com/forum/viewtopic.php?t=1091

https://lukasharris.com/2021/02/05/blocking-usb-rubber-ducky-attacks/

https://www.usb.org/defined-class-codes

