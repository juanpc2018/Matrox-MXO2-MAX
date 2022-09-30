## Matrox MXO2 with MAX </p>

O2 = Oxygen </br>
MAX = Optonal DSP HW h.264 encoder *probably just a different Firmware, Non-MAX HW may be the same, *Unconfirmed. </p>

was a very nice AV Capture Export Device, </br>
similar to Blackmagic UltraStudio Extreme 4k, but FullHD. </p>

i/o: </br>
SDI & HDMI 1080p3O </br>
NTSC, Analog S-Video, Component & Composite, </br>
unbalanced AES/EBU, Surround Analog Audio. </p>

MAX DSP h.264 encoder: </br>
similar to Matrox CompressHD PCIe,  </br>
better than elgato Turbo h.264 HD usb. </p>

problem is driver support: </br>
Matrox does Not want to realease Developer SDK to create linux drivers or fix bugs or update drivers. </p>

in OSX: </br>
there are 2 drivers, </br>
Official v4.6 and Vosic Unofficial driver. </p>

Official has MAX support, and direct App support: </br>
AVID ProTools HD, MediaComposer, Adobe MediaEncoder, FinalCutPro, Compressor, and others. </br>
No Quicktime support. </p>

Unofficial driver works from Yosemite 10.10 upto OSX HighSierra 10.13.6 </br>
does Not have MAX, </br>
but has QuickTime support for QuickTimePlayer Recorder, OBS, Zoom, etc... </p>

Windows 8.1 y W10: </br>
to install drivers Requires to disable: </br>
Signature Driver Enforcement. </p>

in OBS Windows webcam emulator does Not have sound, common problem in OBS for Windows. </br>
but official Matrox h.264 Max Recorder works ok. </p>

In Windows, there are 2 ways to Inject Video to OBS for Live Stream. </br>
A) Directly, Matrox Webcam Emulator, Requires CPU for Recording + CPU or GPU for Streaming.*Not Recomended. </br>
B) Recoding to HDD/SSD with Matrox MAX h.264 to a known folder, known file name, </br>
then create a VLC source in OBS [+] Add File, select File, Play Always, No Loop. </br>
That way OBS will Play/Stream the MAX encoded file, only requires GPU for Streaming, No CPU at all. </br>
Matrox MAX h.264 for Windows is best option for recording with MAX DSP. </br>
similar 2-software to/from SSD method is required for BlackMagic h.264 Pro Recorder *also DSP + MXPTiny for Windows. </p>

what is Better? </br>
BlackMagic h.264 Pro Recorder or Matrox MAX? </br>
MXO2 Rack has Near 0-Latency HDMI/SDI Monitor Output. </br>
BlackMagic Pro Recorder requires an HDMI/SDI Y-Splitter at the input, </br>
IF Y-HDMI/SDI Splitter is 8-Bit, the extra 10/12-Bits are lost, </br>
MXO2 is 1080p30 & Pro Recorder is 1080p60 </br>
when using UHD 4K camera SDI/HDMI, Scaling can be done in different ways: </br>
Directly on Camera, Droping Bits & Frames, Unknown quality. </br>
With dedicated HW Scaler like science-image.com Flow 4K, FPGA custom algorithm or similar DECIMATOR 12G-CROSS 4K </br>
Recording from 4K HDMI/SDI to NDI in OBS, scaling is done in CPU </br>
but also requires more CPU & GPU for Recording & Streaming. </br>
CPU is less efficient, requires fans at 2000RPM, power hungry. </br>
The idea is to Avoid CPU at all cost, NDI is for longer than SDI cable, compatible with IP 12G SFP+ Network </br>
Basically NDI is to replace BNC for Lc-Lc FiberOptic OM1/2/3/4/5. </br>
NDI requires 2-units to Encode & Decode from/to IP Network to/from HDMI/SDI. </br>
Using the CPU for Encoding h.264 / h.265 / VP9 Makes No sense, NDI is Not a replacement for DSP HW encoding. </br>
science-image.com Flow 4K is a cheaper versions of NDI Studio 4K-SH, Flow4K has No Tally Lioght and No NDI encoder/decoder. </p>

OSX Matrox Ventura capture is very outdated: </br>
OSX SnowLeopard, OSX Lion or OSX Mountain Lion, maybe OSX Mavericks. </br>
Matrox compatibility .pdf claims Tested on OSX Yosemite 10.10.4 </br>
Ventura Capture is very bad, </br>
QuickTime Player Recorder or OBS for OSX are much better. </p>

OSX Oficial driver v4.6.O with MAX works upto: </br>
OSX HighSierra 1O.13.6 </br>
FinalCutPro 1O.4.3 </br>
Apple Compressor 4.4.1 </br>
Adobe Media Encoder CS6, CC.2O14, CC.2O15 No Mercury. </br>
No Quicktime. </br>
No Mojave 1O.14.0 </p>

OSX Mohave 10.14 requires 64-Bit Only drivers, No 32-Bit/64-Bit hybrid driver. </br>
MAX can encode UHD4K h264 in Adobe CS6 </p>

h.264 5Mbps VBR Max 7.5Mbps is recomended for YouTube, required for: LBRY, Odysee, etc... </p>

QuickTime Recorder HighQuality mode records in ProRes. </p>

Transcoding is better in OSX with FinalCutPro + Compressor + GPU + MAX </br>
Very fast & Silent, very power efficient. </br>
standard CPU encoding requires Fans at 2000rpm to avoid thermal throtling. </br>
with MacsFanControl. </p>

DSP is much better than CPU. </br>
but Handbrake.fr does Not support MAX h264 codec. </p>

works with: </br>
Matrox PCIe card </br>
Matrox ExpressCard34 + Sonnet ExpressCard Pro to Thunderbolt2 adapter. </br>
Matrox Thunderbolt2 adapter / dock. </p>


MXO2 Rack MAX has a nice stable DDS internal digital clock generator, </br>
can work with unstable SD & HDMI signals and reclock, </br>
similar to AIDA G-CON HDMI </br>
also has Genlock input and passthrough to reclock using a much higher quality clock with true TCXO, OCXO or 10M reference. </p>
