## Micropython-Camera

# build software 
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