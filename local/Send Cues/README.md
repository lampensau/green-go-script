# Static CUE Button Functions

- **Created by:** Timo Toups

This script overrides the default functionality of a defined range of buttons and touchscreen sections to handle CUE communication. A defined button sends a progressing CUE signal, starting with `Attention`, skipping `Ready` if not received, and ending with `GO`. A press on the corresponding touchscreen section will always cancel or stop any active CUE signal.

> Note: This script handles the second device page poorly. It currently simply shifts the given channel range by `+15`. This fits the default UI configuration but may be insufficient for custom user interfaces.
