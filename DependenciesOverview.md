## List of dependencies ##
(3rd party libraries, not needed for all libraries)
  * [libJPEG](http://www.ijg.org/)
  * [libPNG](http://www.libpng.org/pub/png/libpng.html)
  * [zLib](http://www.zlib.net/)
  * [libOgg / libVorbis](http://www.vorbis.com/)
  * [OpenAL Soft](http://kcat.strangesoft.net/openal.html)
  * [OpenGL](http://www.opengl.org/)
  * [Direct-X](http://msdn.microsoft.com/en-us/directx/default.aspx)
  * [Visual Leak Detector 2.1](http://vld.codeplex.com/) ( optional )

## Details ##

This shows by which libraries these dependencies are used by:
  * libJPEG and libPNG
    * Image
      * Font
  * zLib
    * libPNG
    * FileSystem
  * libOgg and libVorbis
    * Audio
  * OpenAL Soft
    * Audio
  * OpenGL
    * Gloot
  * Direct-X
    * Fable
  * Visual Leak Detector 2.0b
    * All OG Libraries
  * Shared - Needed by all OG Libraries
  * Common
    * Audio
    * Console
    * Fable
    * FileSystem
    * Font
    * Gloot
    * Image
    * Model
  * Math
    * Font
    * Model
    * Image
    * Audio
    * Fable
    * Gloot
  * FileSystem
    * Console
  * Image
    * Font

That Common is used by all OG Libraries does not mean that they are needed in the interface of those libraries too.<br />
For example you don't need to use classes from the Common library to access the Gloot interface.<br />
This shows which libraries actually use classes from the Common library in their interface:
  * Audio
  * Console
  * Model

The same goes for the Math Library:
  * Audio
  * Console
  * Model