Matrox-MXO2-MAX

O2 = Oxygen

MAX = optonal DSP HW h.264 encoder. *probably just a different Firmware, Non-MAX HW may be the same. Unconfirmed.

was a very nice AV Capture Export Device,
similar to Blackmagic UltraStudio Extreme 4k, but FullHD.

i/o:
SDI & HDMI 1080p3O, 
NTSC, Analog S-Video, Component & Composite,
unbalanced AES/EBU, Surround Analog Audio..

MAX DSP h.264 encoder:
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
Signature Driver Enforcement. </p>

in OBS Windows webcam emulator does Not have sound. </br>
but official Matrox H264 Max Recorder works ok. </p>

In Windows, there are 2 ways to Inject Video to OBS for Live Stream. </br>
A) Directly, Matrox Webcam Emulator, Requires CPU for Recording + CPU or GPU for Streaming.*Not Recomended. </br>
B) Recoding to HDD/SSD with Matrox MAX h.264 to a known folder, known file name, </br>
then create a VLC source in OBS [+] Add File, select File, Play Always, No Loop. </br>
That way OBS will Play/Stream the MAX encoded file, only requires GPU for Streaming, No CPU. </br>
Matrox MAX h.264 for Windows is best option for recording with Matrox MAX. </br>
similar 2-software to/from SSD method is required for BlackMagic h.264 Pro Recorder + MXPTiny for Windows. </br>
what is Better? BlackMagic h.264 Pro Recorder or Matrox MXO2? </br>
MXO2 has Near 0-Latency HDMI/SDI Output </br>
BlackMagic Pro Recorder requires an HDMI/SDI Y-Splitter at the input, </br>
IF Y-HDMI/SDI Splitter is 8-Bit, the extra 10/12-Bits are lost. </br>
Matrox is 1080p30 & Pro Recorder is 1080p60, <br>
when using UHD 4K camera SDI/HDMI, Scaling can be done in different ways: </br>
Directly on Camera, Droping Bits & Frames, Unknown quality. </br>
With a HW Scaler like science-image.com Flow 4K, FPGA custom algorithm </br>
Recording from 4KI HDMI/SDI to NDI in OBS, doing 4K to FHD scaling in CPU, </br>
but also requires more CPU & GPU for Recording & Streaming. </br>
CPU is less efficient, requires fans at 2000RPM, power hungry. </br>
The idea is to Avoid CPU at all cost, NDI is for longer than SDI cable, compatible with IP 12G SFP+ Network </br>
Basically NDI is to replace BNC for Lc-Lc FiberOptic OM1/2/3/4/5. </br>
NDI requires 2-units to Encode & Decode from/to IP Network to/from HDMI/SDI. </br>
Using the CPU for Encoding h.264 / h.265 / VP9 Makes No sense. </p>

OSX Matrox Ventura capture is very outdated: </br>
OSX SnowLeopard, OSX Lion or OSX Mountain Lion, maybe OSX Mavericks. </br>
Matrox compatibility .pdf claims Tested on OSX Yosemite 10.10.4 </br>
Ventura Capture is very bad, </br>
QuickTime Player Recorder or OBS for OSX are much better. </p>

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


MXO2 Rack MAX has a nice stable DDS internal digital clock generator,
can work with unstable SD & HDMI signals and reclock,
similar to AIDA G-CON HDMI
also has Genlock input and passthrough to reclock using a much higher quality clock with true TCXO or OCXO.
