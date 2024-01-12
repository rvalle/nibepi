# Docker setup in Ubuntu 20 

Build this docker on the target device
Ensure that the UART is enabled, and the container node user has permissions

- under /boot/firmware: disable bluetooth, enable uart
- using systemd disable getty on ttyS0 and ttyAMA0
- using udev add rules so that ttyAMA0 has rw group permission

user group IDs in container (tty, dialout, etc) must match host's ones.
