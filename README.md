[mirror only - development is done on my own git server]

# cam

Cam controls cameras, or is supposed to. It is supposed to be more useable than the abominable web interface these things tend to come with. It is a simple script to control Xiongmai and related cameras using the `anyka_ipc` command daemon and `NETSDK` interface. It might work on others as well, it might not work at all. It works for me, mostly.

Use: `cam <camera_number|'all'> <command> [parameters]`

## configuration

You will need to edit the script to configure your camera IP addresses. If you changed the username and password on the device you can enter these as well but it is by no means guaranteed to work since it is quite probably that username `admin` and a blank password is hardcoded somewhere in the firmware on your camera.

Run the script without any parameters to see the available commands. Some commands take parameters, use `can 1 [command] -H` to see the available parameters and the accepted value ranges.

This script is based on what I could discern from a firmware dump parts of which I ran through Ghidra.
