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
<img width="436" height="468" alt="GlideOverride" src="https://github.com/user-attachments/assets/ae6b5bcd-c0dc-422a-9994-f46e67b7e4e2" />


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

### OpenGl overrides
MesaFx will default OpenGl games to 32bit if the game doesnt specificly sets it, most Quake 2 engine games! So its usefull there if you want to play in 16bit. \
<img width="436" height="468" alt="OpenGLForce" src="https://github.com/user-attachments/assets/cccdce03-b135-444b-9adb-47ce979d60d5" />


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
<img width="437" height="469" alt="Trilinear" src="https://github.com/user-attachments/assets/aeec4c37-e481-44d6-bff6-4a5c63c4d855" />

Trilinear texture filtering <b>still has to be enabled in-game</b> either in games settings or setting texture filtering to GL_LINEAR_MIPMAP_LINEAR.

<b>Remember to disable it back, if not using Trilinear</b>, since multitexturing stays disabled with this feature enabled, for all filtering modes in OpenGL!



