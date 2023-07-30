
How to disable LAN-side DHCP on a GL.iNet 300M router:

SSH to the device using root@[LAN IP ADDRESS].
The password is the admin password used to access the web interface.

cd /etc/config

now edit the file 'dhcp' - 
find the section of the file that starts with "config dhcp 'lan'"
add a new line to that section: "option ignore '1'"

reboot the router: "reboot now"

and it should reboot 
