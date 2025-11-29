# 3dfx Wide driver
3dfx Wide driver for Windows 98

![IMG_20250811_230445_tigr](https://github.com/user-attachments/assets/cf841022-f841-482c-bf3f-4d92b27e7661)

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
<img width="437" height="468" alt="slika1" src="https://github.com/user-attachments/assets/c330b942-07b3-4fdc-bf5f-9fd982bce76f" />

As of now, the only games, that seem to work with it, are Unreal engine games (Unreal, Unreal tournament, DeusEx, Rune, Undying...).

### MesaFx/OpenGl overrides
MesaFx will default OpenGl games to 32bit if the game doesnt specificly sets it, most Quake 2 engine games! So its usefull there if you want to play in 16bit. \
<img width="437" height="468" alt="slika4" src="https://github.com/user-attachments/assets/45f652ad-250f-4beb-a2bf-e413545bcbc3" />

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





