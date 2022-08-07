Matrox-MXO2-MAX

O2 = Oxygen

MAX = DSP HW h.264 encoder.

was a very nice AV Capture Export Device,
similar to Blackmagic UltraStudio Extreme 4k, but FullHD.

i/o:
SDI & HDMI 1080p3O, 
NTSC, Analog S-Video, Component & Composite,
unbalanced AES/EBU, Surround Analog Audio..

MAX DSP h264 encode:
similar to Matrox CompressHD PCIe, 
better than elgato Turbo h.264 HD usb.

problem is driver support:
Matrox does Not want to realease Developer SDK to create linux drivers or fix bugs or update drivers.

in OSX:
there are 2 drivers,
Official v4.6 and Vosic Unofficial driver.

Official has MAX support, and direct App support:
AVID ProTools HD, MediaComposer, Adobe MediaEncoder, FinalCutPro, Compressor, and others.
No Quicktime support.

Unofficial designed for Yosemite works upto OSX HighSierra,
does Not have MAX,
has QuickTime support, for QuickTimePlayer Recorder, OBS, Zoom, etc...

Windows 8.1 y W1O:
to install drivers Requires to disable:
Signature Driver Enforcement.

in OBS Windows webcam emulator does Not have sound.
but official Matrox H264 Max Recorder works ok.

OSX Official Matrox Ventura capture is very outdated, OSX SnowLeopard, OSX Lion or OSX Mountain Lion,
maybe OSX Mavericks.

Matrox compatibility .pdf claims Tested on OSX Yosemite 10.10.4
Ventura Capture is very bad, 
QuickTime Player Recorder or OBS are much better.

OSX Oficial driver v4.6.O with MAX.
works upto:
OSX HighSierra 1O.13.6
FinalCutPro 1O.4.3
Apple Compressor 4.4.1
Adobe Media Encoder CS6, CC.2O14, CC.2O15 No Mercury.
No Quicktime.
No Mojave 1O.14.0

OSX Mohave 10.14 requires 64-Bit Only drivers, No 32-Bit/64-Bit hybrid driver.

MAX can encode UHD4K h264 in Adobe CS6

h.264 5Mbps VBR Max 7.5Mbps is recomended for YouTube, required for: LBRY, Odysee, etc...

QuickTime Recorder HighQuality mode records in ProRes.

Matrox MAX h.264 for Windows is best option for recording h264 with MAX.

Transcoding is better in OSX with FinalCutPro + Compressor + GPU + MAX
Very fast & Silent, very power efficient.

standard CPU encoding requires Fans at 2000rpm to avoid thermal throtling.
with MacsFanControl.

DSP is much better than CPU.
but Handbrake.fr does Not support MAX h264 codec.

works with:
Matrox PCIe card
Matrox ExpressCard34 + Sonnet ExpressCard Pro to Thunderbolt2 adapter.
Matrox Thunderbolt2 adapter / dock.


MXO2 Rack MAX had a nice stable DDS internal digital clock generator,
can work with unstable SD & HDMI signals and reclock,
similar to AIDA G-CON HDMI
also has Genlock input and passthrough to reclock using a much higher quality clock with true TCXO or OCXO.
