# Balena tailscale
This project runs a tailscale docker image inside balenaOS. I use this to power my raspberry pi and use it as a router to create my own VPN service.

* Step 1:
Create your own tailscale account and obtain your own auth key. See: https://tailscale.com/kb/1085/auth-keys

* Step 2:
Setup BalenaOS and add OS to raspberry pi SD card: https://docs.balena.io/learn/getting-started/raspberrypi4-64/go/
Make sure you create a fleet

* Step 3:
Clone this git repo, change the TS_AUTHKEY in the docker-compose.yml. Download Balena CLI and balena push to your fleet via command **balena push fleetname**

* Step 4:
In the tailscale web panel, authorize your raspberry pi. Then authorize it as an exit note.

* Step 5:
Install tailscale client on your windows/android etc and select the appropiate exit node. Enjoy !


