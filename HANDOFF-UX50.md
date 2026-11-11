# UX50 core experiment

This branch preserves an experiment based on upstream commit `3f854ef352544d4cf207716679d62dbedd3fd6c5`. It adds a 480 × 320 display mode, a limited Sony tick-timer register shim, keyboard event injection through the ARM bridge, and embedded API methods to send keys and save sessions.

The changes are a handoff, not an upstream-ready implementation. Review the timer shim and keyboard behavior, including effects on non-Sony guests. Build and test keyboard input, session round-trip and UX50 behavior with a lawfully obtained ROM. No new build or runtime test was done when this branch was prepared.

The save-session API serializes ROM and guest state. Treat resulting images as sensitive and potentially copyrighted. Do not add ROMs, session files, generated probes or local user data to this branch. Review GPL obligations before redistribution.
