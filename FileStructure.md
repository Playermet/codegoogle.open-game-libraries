## Global Folders ##
  * **Game** folder
    * **Game/base** folder should contain all your games resources.
      * This includes both gpk files (archive files) as well as non archived files.
    * **Game/mods** folder should contain mod folders, that is if you support modding.
      * Each directory in the Mods folder is a possible mod.
  * **My Games** (in the user folder) folder should contain save games, configs and screenshots.

## Folders in the resource directories ##
A resource directory is a directory containing gpk files and unarchived resources.<br />
The Base folder and a Mod folder are both resource directories.<br />
Inside these directories you will want to have a clear structure on where to put files.

We are currently using this:
  * **decls/** contains all .decl and .xdecl files.
    * **decls/entities/** contains entity declarations
    * **decls/huds/** contains hud .xdecl files
    * **decls/maps/** contains level declarations (mapname, author, gametypes, etc)
    * **decls/guiSkins/** contains user interface skin .xdecl files
    * **decls/materials/** contains all Material Declarations
    * **decls/sounds/** contains all SoundDecls (sound volume, looping, min/max distance, etc.)
  * **fonts/** contains font files, that is for each font one folder, and each folder containing mulitple (different sizes) .fnt files + the needed images.
  * **gfx/** contains GUI, Hud, etc graphics
  * **maps/** contains level data.
  * **models/** contains 3d model files
  * **sounds/** contains all sound files.
  * **textures/** contains world and model textures.
  * **videos/** contains all video files.