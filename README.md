# OGXHUB

This is a custom 4 port USB hub meant to be installed inside the Original Xbox along with an OGX360 running the latest firmware (supports Original Xbox controllers.) The Xbox motherboard plugs into an internally installed OGX360 via 2 Xbox motherbaord to USB Micro B x2 cables, the OGX360 plugs into the hub via a USB Type A to 4 pin connenctor, then the controller ports are plugged into the hub. This allows your controller ports to support any device the OGX360 supports with the use of an Xbox to USB adapter.

# Powering the Hub

This hub can be powered by either USB from the OGX360 or by plugging a 2 pin connector into the header labeled "DC" and connecting that to a +5V/GND source inside the Xbox. The easiest source would be the Molex HDD connector for a completely modular and solder-free install.

If all you're doing is using a single Xbox 360 wireles PC adapter, you do not need a secondary power source plugged in, but if you plan on using more than one powered device with the controller ports, you will want to connect the secondary +5V DC source.

# Support for Lightguns

Lightguns have not been tested as I don't own any of the necessary hardware required. I have included headers for video sync lines on the hub (placing them is optional) so to test this, the Xbox motherboard to USB Micro B cables will need an additional 2 wires (the yellow ones) connected to a 2 pin connector ([JST 02SR-3S](https://www.digikey.com/short/0zfjhm3b))
