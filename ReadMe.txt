Voodoo4/5 Wide Driver
Version 1.1

**************************************************************************************************************************************
Voodoo Series Driver Kit:			1.0
Voodoo Series Win9x 2D/3D Display Drivers:	4.13.01.0028
Glide 2.X Driver:				1.00.01.0106		(glide2->glide3 wrapper)
Glide 3.X Driver:				3.10.00.2620		(Koolsmoky glide 2610 source)
OpenGL Driver Version:				MesaFx 6.2.0.2		(OpenGL ICD)
**************************************************************************************************************************************

Release Notes
=======================================================================
Version 1.1
- Fixed occasional lock-up on game start
- Added back sse2 texture downloads, that were removed from v1.0
- Fixed eventual crash from switching between windowed and fullscreen in glide
- Alt-tab wont crash openGl games anymore

Version 1.0:
- Added extended resolutions (
	- 16:9 	- 1280x720, 1360x768, 1600x900, 1920x1080
	- 16:10	- 1280x800, 1440x900, 1680x1050, 1920x1200
	- 21:9	- 1680x720, 1792x768, 1920x800
- Increased max refresh rate from 120hz to 144hz for Glide and OpenGl games
- Added Glide resolution override
- Added 16bit force to mesaFx from 3dfxTools
- Fixed quake2 1280x960@60hz sometimes(always) resulting in black screen
- Some quality of life fixes from latest sourceforge glide source


What's in the distribution?
=======================================================================
This distribution contains Voodoo drivers and control panel for 
Windows 9x/ME. The DirectDraw portion of the drivers supports Direct3D 
when using DirectX 7.x, DirectX 8.x and DirectX 9.x.

Supported Hardware
=======================================================================
This driver set is for the VSA chip based Voodoo4/5. 


Installation
=======================================================================
* Extract the drivers, and double click ->"SETUP.EXE"<-


Extra notes
=======================================================================
- MesaFx 16bit overrides are enabled by default, disable it, for default MesaFx behaviour. 
Or 16bit will be used in all openGl games. This is important, should be used as a fps boost in older openGl games,
specialy Quake 2 engine ones. But for Quake3(for example), no need.

- If your using mostly VGA output, run the extra registry file for 1920x1080.
It will override the timing for this resolution and vga, with the ones provided by 3dfx.
\Extra\Win98\98_Set1080p_vga.reg

- Glide override resolution, was tested with Unreal engine games, it might work for others, or not ...
If it works, FOV has to be adjusted in-game. If default fov is 90 at 4:3, then its 106 for 16:9 and 121 for 21:9.
But fov is a personal prefference.

Game specifics:
- Quake 2: In some cases it will set higher gamma, that will also affect other openGl games. When outside the game,
go to 3dfx tools/gamma settings and move the gamma slider and apply. Move back to 1.3.
- Nfs5 - Green-ish smoke when burning rubber, force 32bit glide rendering in 3dfx tools.
- Unreal tournament - Glide running slower than other APIs. Glide has some extra settings enabled by default.
Open console "~", enter "preferences", it will open advanced settings. Under Glide disable Detail textures and Volumetric lights.

=======================================================================
ND 2022
Glide sourceforge project: 	https://sourceforge.net/projects/glide/
Koolsmoky:			https://www.3dfxzone.it/koolsmoky/
Mesa3d:				https://www.mesa3d.org/