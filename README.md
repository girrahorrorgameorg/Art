# Art
Textures should be 64x64 pixels

The colour palette is weird so you will need to change it in your software. The colour palette is here: https://quakewiki.org/wiki/Quake_palette It is also called colormap.lmp in the root of this repository.

Graphics for the game are stored in /gfx folder

To convert the lmp files to tga, use the lmp2tga.exe. Run it from the commandline in the same folder as the palette.lmp. When editing the file, make sure to keep the transparent colour correct.

If in doubt, save it and convert back to lmp using tga2lmp.exe. Then open up a hex editor (HxD for example) and check that there is a lot of FF everywhere (FF is the transparent colour). If you see a bunch of other random hex values, go to edit -> replace -> hex values. Then put in the bad hex value and set the correct one (FF). Then hit replace all and save. This should fix transparency issues with photoshop.
