# (W)BPX Single Channel UI

- **Forum Discussion:** [Link](https://greengoconnect.com/index.php?p=/discussion/495/creating-a-single-channel-ui-mode)
- **Created by:** Timo Toups

A script that overrides the UI or a WBPX or BPX belt pack to become a single-channel user interface.

> Note: As is, this script ignores the sports variants, as it facilitates colors on the screen to indicate button functionality.

To make this script function, you have to respect a few requirements:

- The device or user's device profile must have the `2ch` UI mode configured
- The device's or user's second channel must be unassigned (empty)
- The script only displays the first channel, and it must be assigned

If one of the above requirements is not met, the UI will not be used, and the script will default to the currently configured UI mode.

This script depends on the user's channel configuration and adjusts accordingly. You can, for example, make all four buttons act as talk buttons if you _disable_ the channel's `Call Mode`

> Note: I am unaware of how to mount an encoder's click event. The first button's function is not overwritten to allow for channel mute and flex mode button-combinations.
