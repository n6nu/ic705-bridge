# IC-705 Bridge

WiFi-attached **Icom IC-705** as a TCI / rigctld transceiver with RX and TX audio for
WSJT-X — no USB cable. The bridge talks to the radio over its built-in WiFi/LAN, which
keeps USB hash off the receive path.

Part of the [N6NU SDR Bridges](https://bridges.n6nu.org) family.

## Download

Current build (V3, close to release):
**[ic705-bridge-3.1.3-setup.exe](https://bridges.n6nu.org/beta/ic705-bridge-3.1.3-setup.exe)**

Take this one rather than the GitHub release: the v2.1.x installers were
packaged without the Microsoft Visual C++ runtime, so on a clean Windows
machine they start and close again immediately. This build carries the runtime
with it. It also stops the Settings dialog writing its own fallbacks over this
app's defaults -- on a fresh install, opening Settings and clicking OK used to
turn CAT and TCI off and move the CAT port, none of which you asked it to do.

Older releases: the [releases page](https://github.com/n6nu/ic705-bridge/releases).

## Setup

In WSJT-X, choose **TCI** as the radio and enable TCI audio. Both *Fake It* and
*Rig split* modes are supported.

The user guide PDF is at https://bridges.n6nu.org and is bundled in the installer
(Help → User Guide, F1).

73, Andreas, N6NU
