# OGXHUB

![OGXHUB PCB](https://github.com/wiredopposite/OGXHUB/blob/main/Pictures/ogxhub_1.2.jpg?raw=true)

This is a custom 4 port USB hub meant to be installed inside the Original Xbox along with an OGX360 running the latest firmware (supports Original Xbox controllers.) 

The Xbox motherboard plugs into an internally installed OGX360 via 2 Xbox motherbaord to USB Micro B x2 cables, the OGX360 plugs into the hub via a USB Type A to 4 pin connenctor, then the controller ports are plugged into the hub. This allows your controller ports to support any device the OGX360 supports with the use of an Xbox controller port to USB adapter.

# Powering the Hub

This hub can be powered by either USB from the OGX360 or by plugging a 2 pin connector into the header labeled "DC" and connecting that to a +5V/GND source inside the Xbox. The easiest source would be the Molex hard drive power connector for a completely modular and solder-free install.

If all you're doing is using a single Xbox 360 wireles PC adapter, you do not need a secondary power source plugged in.

# Support for Lightguns

Lightguns have not been tested as I don't own any of the necessary hardware. I've included headers for video sync lines on the hub so to test this, the Xbox motherboard to USB Micro B cables will need an additional 2 wires connected to a 2 pin wire housing ([SHR-02V-S-B](https://www.digikey.com/short/rdddn93j)) and then that needs to be plugged into CLK1 for ports 1 and 2 or CLK2 for ports 3 and 4. There will be a wiring diagram in the Cables section to guide you through crimping your own cables.

# Version 1.6 Xboxes

Version 1.6 Xboxes have shorter controller port wires than the other versions, they will need 2 extra wire extensions, both identical. The diagram for this extension can be found in the  Cables folder.

# PCB BOM
| Qty | Designator | Description | Value/Model | Digikey/Mouser URL | LCSC URL |
| --- | --- | --- | --- | --- | --- |
| 7 | C1,C2,C3,C4,C5,C6,C7 | CAP 10UF 16V 0805 | CL21B106KOQNNNE (Example) | https://www.digikey.com/short/7h5p2595 | https://www.lcsc.com/product-detail/Multilayer-Ceramic-Capacitors-MLCC-SMD-SMT_Samsung-Electro-Mechanics-CL21B106KOQNNNE_C95841.html |
| 2 | CLK_A,CLK_B | CONN HEADER SMD R/A 2POS 1MM | SM02B-SRSS-TB (Optional) | https://www.digikey.com/short/581p59ht | https://www.lcsc.com/product-detail/Wire-To-Board-Wire-To-Wire-Connector_JST-Sales-America-SM02B-SRSS-TB-LF-SN_C160402.html |
| 1 | DC | CONN HEADER R/A 2POS 2MM | DF3A-2P-2DS | https://www.digikey.com/short/tb7h47jn | https://www.lcsc.com/product-detail/Wire-To-Board-Wire-To-Wire-Connector_HRS-Hirose-DF3A-2P-2DS_C531024.html |
| 1 | F1 | PTC RESET FUSE 8V 2A 1812 | MF-MSMF200-2 (Example) | https://www.digikey.com/short/r82m779t | https://www.lcsc.com/product-detail/Resettable-Fuses_TLC-Electronic-TLC-MSMD200_C262032.html |
| 1 | OGX360 | CONN HEADER R/A 4POS 2MM | DF11-4DP-2DS(24) | https://www.digikey.com/short/b8j8995n | https://www.lcsc.com/product-detail/Wire-To-Board-Wire-To-Wire-Connector_HRS-Hirose-DF11-4DP-2DS-24_C202087.html |
| 2 | PORT_A,PORT_B | CONN HEADER R/A 12POS 2MM | S12B-PHDSS(LF)(SN) or DF11-12DP-2DS(24) | https://www.digikey.com/short/h3p7p53v | https://www.lcsc.com/product-detail/Wire-To-Board-Wire-To-Wire-Connector_JST-Sales-America-S12B-PHDSS-LF-SN_C161673.html |
| 2 | R1,R2 | RES 10K OHM 5% 1/8W 0805 | RC0805JR-0710KL (Example) | https://www.digikey.com/short/jn5md3r4 | https://www.lcsc.com/product-detail/Chip-Resistor-Surface-Mount_YAGEO-RC0805JR-0710KL_C100047.html |
| 1 | U1 | SOP-16 USB HUB | SL2.1A | - | https://www.lcsc.com/product-detail/USB-ICs_CoreChips-SL2-1A_C192893.html |
| 1 | U2 | SOT-583 Power Distribution Switch | TPS2116DRLR | https://mou.sr/3kZ73wz | https://www.lcsc.com/product-detail/Power-Distribution-Switches_Texas-Instruments-TPS2116DRLR_C3235557.html |
| 1 | Y1 | CRYSTAL 12.0000MHZ SMD | J49SMH-F-G-G-K-12M0 (Example) | https://www.digikey.com/short/cj73h43j | https://www.lcsc.com/product-detail/Crystals_JGHC-49SBT12000181060_C390753.html |
