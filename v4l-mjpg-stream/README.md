v4l-mjpg-stream
===============
A systemd service that uses a Video4Linux capable
camera to stream JPEG images over HTTP using mjpg-streamer.

Raspberry Pi Camera Module
==========================
If you're using this service with a Raspberry Pi Camera Module,
you need to load its Video4Linux driver. You can do this
using `modprobe bcm2835_v4l2`. To also load the driver at boot, run
`echo bcm2835_v4l2 > /etc/modules-load.d/rpi_camera_module_v4l.conf`
as root. See `man modules-load.d` for more information.
