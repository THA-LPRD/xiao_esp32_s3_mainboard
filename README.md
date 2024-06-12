# XIAO ESP32-S3 Main Board PCB
## Main Board PCB for the first project at Technical University of Applied Science Augsburg
### Explanation
This repo contains the KiCad 8 files for the Main Board of the project. \
Necessary files are located in the src folder, whilst the 3D-models, symbols and footprints can be found in the models, symbols, and footprints folders.
### Functionality
The Main Board is designed to be a host board for XIAO ESP32-S3 board. \
XIAO ESP32-S3 Documentation can be found under this link: https://wiki.seeedstudio.com/xiao_esp32s3_getting_started/ \
The PCB is designed to be powered by a battery (I used two Li-Ion 5400 mAh batteries connected in parallel and connected to a 1S 2 MOSFETs BMS. \
The main functionality of the board is to power an e-paper display and upload pictures to it using SPI protocol. The e-paper display in question is this one: https://www.waveshare.com/7.3inch-e-paper-hat-f.htm \
The PCB is equipped with an external button, which I used to refresh the display on demand (show a new picture), a switch that switches between 3.3V and 5V as Vcc for the display, as some Waveshare displays need 5V to operate. \
There are no mounting holes as the PCB is mounted in a 3D printed housing.
### TODOs
The main branch contains the old schematic with no subsheets and is a bit unpleasant to follow. I added subsheets to the feature_subsheets branch but updating the PCB from that schematic will cause problems with the net names and connections.
