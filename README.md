## Micropython esp 32 camera 
## Build firmware for esp32 camera 
## Add Boot.py and main.py file micropython will run boot on the start then main file
# Check more information about micorpython http://docs.micropython.org/en/latest/

# build micropython software 
    python3 build.sh

# build software 
    python3 build.sh

# make file
    # Inside micropython/ports/esp32 
    # Makefile line 12 -> usb-port PORT /dev/tty
    # firmware path line 22 -> change to "firmware-"
    python3 make.sh

# Flash esp
    python flash_esp.sh

# Push file into esp32
    ampy --port /dev/tty.usbserial-A50285BI put boot.py

