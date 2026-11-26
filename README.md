# 3dfx Wide driver
3dfx Wide driver for Windows 98

<img width="2448" height="1843" alt="IMG_20260726_175645" src="https://github.com/user-attachments/assets/66d7033f-4d5c-4390-ae55-e4a9fac18864" />

For Voodoo 4/5 video cards, on Windows 98!
<br/> <br/>
Download the drivers from Releases. \
Extract the drivers, and double click ->"<b>SETUP.EXE</b>"<-
<br/><br/>
More informations, benchmarks... Are avaliable here:
<br/>
[Vogons forum / The Changeling 3dfx Voodoo 5 5500](https://www.vogons.org/viewtopic.php?t=85416&start=120)
<br/><br/>

## Quick additional informations
### Glide resolution override
Glide override will force the selected resolution in glide games, example 1920x800 or 1920x1080. \
<img width="437" height="469" alt="Driver5" src="https://github.com/user-attachments/assets/ca6cdfa0-dc03-4c86-a8bd-3bc3fc65b517" />


As of now, the only games, that seem to work with it, are Unreal engine games (Unreal, Unreal tournament, DeusEx, Rune, Undying...).

#### Additional games that are patched in the driver
See <b>\WidescreenPatches</b> folder in the driver for per-game information.
<br/>
<b>PATCH WILL ONLY WORK WITH THE CORRECT VERSION OF THE GAME!!!</b>
- Diablo II Lord of Destruction
- Driver
- Gta 2
- Ignition
- MDK
- Turok Dinosaur Hunter

### OpenGL overrides
By default color and texture depth(bits) will default to whats set for the system/desktop color depth. You can force 16bit or 32bit for more control what the games do. \
<img width="437" height="469" alt="Driver1" src="https://github.com/user-attachments/assets/0e0fcf4d-dfc7-4152-bace-8827fc1d49f7" />

### Refresh rate toggle
Can be used to force higher refresh rate. \
<img width="437" height="468" alt="Drivers1" src="https://github.com/user-attachments/assets/4f40d721-3f02-4d37-aecc-01a622311af9" />

It will work on d3d, glide and opengl. \
If you are changing the refresh rate of the video adapter in windows settings, this will reset and you will have to set it again in 3dfx tools. \
<br/>
Higher refresh rate comes with a (small) performance penalty.
- q3 went from 71fps(60hz) to 69fps(100hz)
- ut went from 44fps(60hz) to 43fps(100hz)

It will try to get the highest refresh rate. So if you have it set at 144hz and at certain resolution its max 85hz, it will use 85hz. \
If another resolution has 120hz, it will use that. If you max out at 60hz, it will use that. \
Default is 60hz.

### OpenGL Enable Trilinear texture filtering
Will disable multitexturing and enable Trilinear texture filtering support. \
Its a harware limitation with only 2 TextureMappingUnits. You either have Multitexturing OR single-pass Trilinear. 
<img width="437" height="469" alt="Driver3" src="https://github.com/user-attachments/assets/fc4323c1-5c82-4f33-9788-af15de989521" />

Trilinear texture filtering <b>still has to be enabled in-game</b> either in games settings or setting texture filtering to GL_LINEAR_MIPMAP_LINEAR.

<b>Remember to disable it back, if not using Trilinear</b>, since multitexturing stays disabled with this feature enabled, for all filtering modes in OpenGL!

### OpenGL API Version
By default OpenGL v1.2 featureset is enabled, this is a safe choice between speed and compatibility, most of the featureset is supported in the hardwarre. 3dfx own driver had v1.1. For more game compatibility you can enable higher versions, up to OpenGL v1.5, but since not everything is supported on the hardware, some features will run on the CPU or be advertised and "faked". So use it as a compatibility toggle if you run into issues with "newer" OpenGL games. \
<img width="437" height="469" alt="Driver4" src="https://github.com/user-attachments/assets/531d65f1-20f6-4579-8577-cdad058d2eb1" />

### Doom 3
The driver can run Doom 3, set OpenGL to v1.5 and set an environment variable <b>set FX_GL_FAKE_EXTENSIONS=1</b> for the game to run. \
<img width="1920" height="800" alt="glide_20261124_003153" src="https://github.com/user-attachments/assets/30e89188-c0c4-4ad6-8b82-eb6dcdffea9f" />
