# On Air Signal Function

- **Created by:** Timo Toups

A script to add two 'On Air' buttons to the UI of an MCX, MCXD, or WPX device, and control two or more BCN beacon lights.

The script uses both 'script to script' communication and OSC messages:

- The 'script-to-script' communication is there to signal the current _onAir_ state to other Green-GO devices using the same configuration.
- The OSC endpoints (`/studio/onair/x`) are mainly meant to allow external control (e.g., a lighting console) over the _onAir_ state. If needed the control script can send OSC packets to a defined IPv4 address (`targetOSC`); to enable this you need to uncomment all lines starting with `//sendOscAction` in `mcx_wpx-onAir-control.gg5t`.

It is possible to change the colors used to signal _onAir_ during runtime by sending an OSC packet to any Green-GO device running the 'onAir...' scripts. The OSC message needs to contain one integer between 1 - 9.

The script consists of multiple parts and has individual script files for each device. Devices supported in this version are: BCN (receiver), MCX (sender/receiver), MCXD (sender/receiver), WPX (sender/receiver).
