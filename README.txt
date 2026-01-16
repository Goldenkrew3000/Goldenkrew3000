Hello, my name is Goldenkrew3000, and welcome to my GitHub profile :)
I (unfortunately) live in Australia.

You can contact me at:
 - (Discord) goeunbyul
 - (Twitter) goldenkrew3000

A list of my main projects:

OSSP (https://github.com/goldenkrew3000/OSSP_OpenSource)
OSSP is a versatile audio player (Targeting Subsonic/OpenSubsonic servers but eventually local playback) with
native support for custom audio pipelines to add filters (Equalizers, Pitch changing, Reverb etc) on UNIX/Unix-like
operating systems (Also works under WSL, but I am NOT adding Win32 support).
Now, you might think that this is kind of pointless, like just run an equalizer in another program. BUT - On operating
systems such as FreeBSD or macOS, Equalizers are often paid (macOS), or just don't really exist (FreeBSD). Not to mention
other features like Filters, Pitch adjustment, Reverberation etc.
This is my main project, and probably the thing I am most proud of, but keep in mind that this is also just a hobby
project and development is not consistent.

Desk Clock (https://github.com/goldenkrew3000/DeskClock) *Private until I finish it*
--

T720 PostmarketOS (https://github.com/goldenkrew3000/T720-PostmarketOS)
An abandoned effort of porting the Samsung Galaxy T720 (SM-T720) to Mainline Linux.
There is a working touchscreen driver, and some other half reverse engineered and reimplemented drivers
for the PMIC and Fuel gauge.
P.S. This was abandoned due to a horrific Dual MIPI DSI screen for GPU acceleration. Thanks Samsung >:(

Hojuix (https://github.com/goldenkrew3000/Hojuix)
Hojuix is a simple x86_64 monolithic kernel (Development currently on pause).
It uses Limine as a bootloader, and mlibc as it's libc (Although those changes are not pushed yet).
Due to my absolutely horrific memory management system, it only boots on half the hardware I have tested,
but weirdly, it doesn't work under Coreboot with EDK2. Memory allocation is horrifically slow so the
memory management system needs a rewrite anyway.

And some of my other mini projects:

liburiescape_lcue (https://github.com/goldenkrew3000/liburiescape_lcue)
This is a very small C library that can URI escape a string.
Most of the code in this library has been extracted from libcurl (verison 8.15.0) and modified
to work out-of-tree for projects that run in environments where libcurl is too expansive.
Why specifically libcurl: Every other small URI escaping library I tried ran into an issue every so often
when ran thousands of times, so I used libcurl's implementation as a battle-tested base (Also it works).

Nuphy Air60 v2 QMK Fork (https://github.com/goldenkrew3000/nuphy_air60v2_qmk)
This is a fork of the official QMK firmware released by Nuphy for the Air60 v2 keyboard.
This fork has been made for personal use, and contains many patches that no one else would want.
The patches are:
 - Removed most of the lighting effects, and added a completely white effect (Although in person,
   it has a slightly blue tint due to how non RGBW LED diodes appear)
 - Works in FreeBSD natively
 - The USB VID/PID are set to a Logitech K120 (To help with extreme edge cases in unique operating
   systems)
