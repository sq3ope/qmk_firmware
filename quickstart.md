# Setting Up Your QMK Environment

Follow the instrucions at: https://docs.qmk.fm/#/getting_started_build_tools

Configure the defaults:
1. `qmk config user.keyboard=redox/rev1/base`
1. `qmk config user.keymap=sq3ope`

# Editing my keymap

Edit the file `~/qmk_firmware/keyboards/redox/keymaps/sq3ope/keymap.c`
# Building Firmware

`qmk compile`

# Flashing the firmware
1. `qmk flash`
1. Wait until you see
    > Waiting for USB serial port - reset your controller now ......
1. Press layer3 (_adjust) button + Q button
1. Wait for message
    > avrdude done.  Thank you.

Now connect the other half of keyboard by USB and repeat. Note that now you have to use P button instead of Q to reset the controller in step 3.
