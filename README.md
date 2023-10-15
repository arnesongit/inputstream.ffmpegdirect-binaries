# inputstream.ffmpegdirect-binaries

This repository contains the compiled binaries for the Kodi addon [inputstream.ffmpegdirect](https://github.com/xbmc/inputstream.ffmpegdirect)<br>
for Linux on platforms for x86_64 (PC), armv7 and aarch64 (ARM Linux, e. g. for Raspberry Pi 4B).

The reason for this is that the compiled versions for Linux platforms doesn't contain the dash demultiplexer by default.<br>
On other platforms like Windows, MacOS and Android the inputstream.ffmpegdirect adddon has the built-in dash demultiplexer.

Because the [TIDAL2](https://github.com/arnesongit/plugin.audio.tidal2) addon uses MPEG-Dash streams with FLAC content,
you will need a working version of the inputstream.ffmpegdirect addon.

You can build this addon by yourself like I described [here](https://github.com/arnesongit/plugin.audio.tidal2/blob/master/README-Dash.md).<br>
If you have no experience compiling in a Linux environment, you can use the binaries which I published here.<br>
You can install it with the "Install from ZIP" method in Kodi. Be sure, that you disable the automatic update for this addon after you installed it!

Choose your version:

- 19.0.3 is for Kodi Matrix
- 20.5.0 is for Kodi Nexus
- 21.2.0 is for Kodi Omega (Alpha)
<p>
- armv7 is for Linux on 32-Bit ARM platforms like Raspberry Pi 4B / Compute Module CM4 / LibreELEC 10 or 11 on RPi4
- aarch64 is for Linux on 64-Bit ARM platforms like XBian for Raspberry Pi or LibreELEC 12 Alpha
- x86_64 is for Linux on a 64-Bit Linux distribution for PC hardware.<br>
  It's compiled for [Ubuntu 22.04.3 LTS](https://ubuntu.com/download/desktop). Other 64-Bit Linux versions will probably work.<br>
  The version for LibreELEC 10.0.4 is compiled on Ubuntu [20.04.6 LTS](https://ubuntu.com/download/desktop/thank-you?version=20.04.6&architecture=amd64), because it need older glibc libraries.

I tested on following platforms:

Raspberry Pi 4B / Compute Module CM4:
- LibreELEC 10.0.4 with [inputstream.ffmpegdirect-19.0.3-linux-armv7.zip](https://github.com/arnesongit/inputstream.ffmpegdirect-binaries/raw/main/inputstream.ffmpegdirect-19.0.3-linux-armv7.zip)
- LibreELEC 11.0.3 with [inputstream.ffmpegdirect-20.5.0-linux-armv7.zip](https://github.com/arnesongit/inputstream.ffmpegdirect-binaries/raw/main/inputstream.ffmpegdirect-20.5.0-linux-armv7.zip)
- LibreELEC 12.0 nightly 20231006 with [inputstream.ffmpegdirect-21.2.0-linux-aarch64.zip](https://github.com/arnesongit/inputstream.ffmpegdirect-binaries/raw/main/inputstream.ffmpegdirect-21.2.0-linux-aarch64.zip) (it's a 64-Bit version)
- XBian 2023.09.29 with [inputstream.ffmpegdirect-20.5.0-linux-armv7.zip](https://github.com/arnesongit/inputstream.ffmpegdirect-binaries/raw/main/inputstream.ffmpegdirect-20.5.0-linux-armv7.zip)<br>
  Here I had to install libatomic1 via 'sudo apt install libatomic1' to make it work.
- OSMC 2023.08-1 with [inputstream.ffmpegdirect-20.5.0-linux-armv7.zip](https://github.com/arnesongit/inputstream.ffmpegdirect-binaries/raw/main/inputstream.ffmpegdirect-20.5.0-linux-armv7.zip)

PC:
- Ubuntu 20.04.3 LTS with Kodi 20.2 and [inputstream.ffmpegdirect-20.5.0-linux-x86_64.zip](https://github.com/arnesongit/inputstream.ffmpegdirect-binaries/raw/main/inputstream.ffmpegdirect-20.5.0-linux-x86_64.zip)
- LibreELEC 10.0.4 with [inputstream.ffmpegdirect-19.0.3-LE10-x86_64.zip](https://github.com/arnesongit/inputstream.ffmpegdirect-binaries/raw/main/inputstream.ffmpegdirect-19.0.3-LE10-x86_64.zip)
- LibreELEC 11.0.3 with [inputstream.ffmpegdirect-20.5.0-linux-x86_64.zip](https://github.com/arnesongit/inputstream.ffmpegdirect-binaries/raw/main/inputstream.ffmpegdirect-20.5.0-linux-x86_64.zip)
- LibreELEC 12.0 nightly 20231007 with [inputstream.ffmpegdirect-21.2.0-linux-x86_64.zip](https://github.com/arnesongit/inputstream.ffmpegdirect-binaries/raw/main/inputstream.ffmpegdirect-21.2.0-linux-x86_64.zip)
