# OGXHUB
![OGXHUB PCB](https://github.com/wiredopposite/OGXHUB/blob/main/Pictures/ogxhub_1.2.jpg?raw=true)

This is a custom 4 port USB hub meant to be installed inside the Original Xbox along with an [OGX360](https://github.com/Ryzee119/ogx360) running the latest firmware (supports Original Xbox controllers.) 

The Xbox motherboard plugs into an internally installed OGX360 via 2 Xbox motherbaord to USB Micro B x2 cables, the OGX360 plugs into the hub via a USB Type A to 4 pin connenctor, then the controller ports are plugged into the hub. This allows your controller ports to support any device the OGX360 supports with the use of an Xbox controller port to USB adapter (X2USB).

# Powering the hub
The hub can be powered either by USB from the OGX360 or via a 2 pin header labeled "DC" (connected to a +5V/GND source inside the Xbox), power via the DC header is automatically enabled by plugging it in. The easiest source would be the Molex hard drive power connector for a modular and solder-free install. Startech SATA adapters come with a power splitter you can plug the hub into, other adapters that don't will need a Molex power splitter.

If all you're using is a single Xbox 360 wireless PC adapter, you won't need a secondary power source plugged in.

# Mounting the hub
The hub is meant to be mounted on the metal RF shield, above the middle tab that holds the Xbox's faceplate in place. You can do this with a piece of double sided tape, just make sure the back of the hub is insulated from the shield. 

# Plugging USB devices into your controller ports
You can do this with either an Xbox to USB cable, or with the adapter I've designed (X2USB). Gerbers for the adapter are in the [Gerbers folder](https://github.com/wiredopposite/OGXHUB/tree/main/Gerbers), BOM is [here](https://github.com/wiredopposite/OGXHUB/tree/main/BOM).

# Version 1.6 Xboxes
Version 1.6 Xboxes have shorter controller port wires than other versions, they will need 2 cable extensions, both identical. The [wiring diagram](https://github.com/wiredopposite/OGXHUB/blob/main/Cables/OGXHUB%20Cable%20Diagram.pdf) for this extension can be found in the Cables folder.

# Support for lightguns
Lightguns have not been tested as I don't own any of the necessary hardware. I've included headers for video sync lines on the hub, so to test this, the Xbox motherboard to USB Micro B cables will need an additional 2 wires connected to a 2 pin wire housing ([SHR-02V-S-B](https://www.digikey.com/short/rdddn93j)) and then that needs to be plugged into "CLK_A" for ports 1 and 2 and/or "CLK_2" for ports 3 and 4. There is a [wiring diagram](https://github.com/wiredopposite/OGXHUB/blob/main/Cables/OGXHUB%20Cable%20Diagram.pdf) in the Cables folder to help you make your own cables.

# Limitations
- The OGX360 firmware is not currently capable of recognizing peripherals other than controllers, such as Xbox communicators or memory cards. Those devices will not work with the hub and neither will Xbox compatible USB flash drives. I do not anticipate DVD IR dongles working but have not tested this. 
- The SL2.1A USB hub is not capable of supporting the 8bitdo V2 Bluetooth adapter (the V1 works fine with the latest firmware). I'll explore some other USB hub IC options in the future, but I anticipate that any that work with the V2 will be considerably more expensive than the SL2.1A. I've tested several other cheap Chinese hub IC options with the same results.
