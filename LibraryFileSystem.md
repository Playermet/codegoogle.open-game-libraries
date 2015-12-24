## Description ##
The interface is loosely based on idTech's filesystem and has some additional features.<br />
So if you are currently using idTech's filesystem, you should be able to easily adapt your code to use this library.

## Features ##
  * Compressed zip file loading
  * Endian safe file reading and writing (Little Endian)
  * Win32, Linux and possibly mac compatible
  * Mod directory support
  * Configurable ( different save locations, own checksum calculation, .. )
  * Various possibilities to restrict access to specific filetypes and archives only.
    * ( For example for lightweight servers, but fully checked clients )
  * Full Unicode support (UTF-8)

## List of authors ##
  * Santo Pfingsten (TTK-Bandit)

## Includes ##
  * `<`[og/FileSystem.h](http://code.google.com/p/open-game-libraries/source/browse/trunk/Libraries/Include/og/FileSystem.h)`>`
    * Includes everything needed, also includes:
    * `<`[og/Shared/FileSystemCore.h](http://code.google.com/p/open-game-libraries/source/browse/trunk/Libraries/Include/og/Shared/FileSystemCore.h)`>` and
    * `<`[og/Shared/File.h](http://code.google.com/p/open-game-libraries/source/browse/trunk/Libraries/Include/og/Shared/File.h)`>`
    * ( for details on the FileSystemCore and File interfaces see [Shared](LibraryShared.md) )

## Dependencies ##
  * [Shared](LibraryShared.md)
  * [Common](LibraryCommon.md)
  * [zLib](http://www.zlib.net/)