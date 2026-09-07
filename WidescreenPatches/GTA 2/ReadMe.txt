Grand theft auto 2 v10.3

- Game version required. Retail + v10.3 patch.
- Run the "gta2 manager" and in video settings set the resolution for glide to 800x600!
  This is the one getting patched, leaving 640x480 alone for fallback.

- Set the Glide Resolution override in 3dfx Tools, ex 1920x1080
- Adjust the games width/height setting in the Registry. Two example .reg files are provided. 
You can just manually set it - make sure it matches the Glide override value selected.

[HKEY_LOCAL_MACHINE\SOFTWARE\DMA Design Ltd\GTA2\Screen]
"full_width"=1920 (as decimal)
"full_height"=1080 (as decimal)

- OPTIONAL copy this folders wideDriver.ini to games folder, next to the gta2.exe.
  This will give you additional settings:
	- aspect_fix=1 (enable/disable the aspect fix)
	- extra_zoom=0 (adjust camera zoom)
	- virtual_height=480 (UI elements scaling)
	
  More instructions in the .ini itself.

- Most override resolutions should work, tested 1600x1200, 1920x1080, 2560x1080. 
  One that wont work correctly is 1280x1024, since its 5:4, the only mode thats taller than 4:3.