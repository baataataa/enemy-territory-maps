**************************************************************************
File:         saberpeakSource.zip
Author:       NOP
Release date: August 11, 2004
Website:      http://home.comcast.net/~saberpeak/
**************************************************************************

These are the source files for the enemy territory map saberpeak. I am 
releasing these files so they can be used by others for learning or level 
editing. 
You are free to distribute and use any portions of these files as prefabs 
in your own maps, as long as the final product is made available free to 
the public. There is only one very important condition:

IF YOU MAKE ANY CHANGES TO ANY CONTENT THAT IS LOADED WHEN THE 
GAME RUNS(I.E. CONTENT THAT IS NOT COMPILED SUCH AS TEXTURES, SHADERS OR MD3 MODELS), 
YOU MUST RENAME YOUR VERSIONS SO THAT NO NAME CONFLICTS OCCUR BETWEEN 
YOUR VERSIONS AND THE ONES IN SABERPEAK.
For example if you make changes to a texture, you need to rename it (or put it in a different path). 
As long as you follow this rule you are free to make any changes you want
including releasing different versions of the map(for example smaller versions
suited better for clan matches etc). But again don't use the word saberpeak at the
beginning of your map name(for example saberpeak_small or saberpeak_3vs3) for the reasons 
outlined above.
Note also that all the .ase models can be opened with a text editor if you want
to change the shaders/textures used on them.

Disclaimer: Use these files at your own risk. Although I tried to make the 
brushwork as efficient as possible, due to time constraints, some times the 
rule of "As long as it works it's good enough" was applied.

**************************************************************************


**********************INSTALLATION AND USAGE*****************************

Place the contents of each directory in the respective directories in your
etmain folder. You also need to download saberpeak.pk3 from the website to
get the complete list of textures, shaders and model files. Any files already in
saberpeak.pk3 were not included in this zip.

Detailed installation instructions:
MAP:      Place saberpeak.map in your etmain/maps folder.
TEXTURES: Place the SaberPeak_editor and the common folders in your etmain/textures folder.
          If you already have a common folder in your textures directory just copy
          the contents of the folder.
MODELS:   Place the saberpeak_ase folder in your etmain/models folder.
SHADERS:  Place the CONTENTS of the common.shader file in your common.shader file in your
          etmain/scripts folder. You can open the common.shader file with any
          text editor(for example Notepad). If you already have shaders with the same
          names in your common.shader file you may safely replace them with 
          the ones in the common.shader file that comes with this zip as they,
          give the same results.
PCX    :  Place the file called saberpeak.pcx in your etmain folder.
EASYGEN:  I have also included the original easygen file used to generate the 
          terrain called saberpeak.eng. Note that this file is included purely 
          for reference, as the terrain was heavily modified in radiant later on. 
          If you want to see what was left of the original easygen terrain select the 
          easygenTerrain func_group in radiant(the "floor" of the resort area is 
          also part of the easygen terrain.)
          To use it place easygen.eng anywhere you want and open it with easygen. 
          Then do import Alphamap and import the saberpeak.pcx file
          It shouldn't be very hard to assign the appropriate texture to each color
          to get the right texture distribution for the terrain. Just use the map
          as a reference.
.pk3:     Also don't forget to download saberpeak.pk3 from the release website and 
          place it in your etmain folder.

If you follow these steps correctly, you should see no brushes or models with 
the "SHADER NOT FOUND" or the "SHADER IMAGE MISSING" texture on them when you load the map in radiant.

**********************************************************************************

************************COMPILING NOTES***********************************
This map requires q3map2 2.5.14 or later to compile correctly.
The compile options used during compilation were as follows:
BSP: -meta
VIS: -vis
Light: -gamma 2 -compensate 4 -patchshadows -external -lighmapsize 512 -samples 3 -shade

NOTE: The lightmaps were modified in photoshop after compile to remove some 
unwanted shadows in certain areas. This is why if you compile the map with the above options
it might not match exactly the version in saberpeak.pk3
*************************************************************************

DON'T REINVENT THE WHEEL. USE, REUSE, AND THEN USE AGAIN.

*************************************************************************