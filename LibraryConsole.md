## Description ##
The **Console** library consists of 3 parts:
  * CVarSystem
  * CmdSystem
  * Console Window
    * Win32: A real window with a RichText log field and background image.
    * Linux: TTY Console (capable of remote control)
    * MacOS: Will probably be like Win32 too.

This offers the possibility of easily adding console commands, cvars and using them in runtime to develop/debug a game.<br />
It will also be possible to access the log & autocompletion features for ingame use.

## List of authors ##
  * Santo Pfingsten (TTK-Bandit)

## Includes ##
  * `<`[og/Console.h](http://code.google.com/p/open-game-libraries/source/browse/trunk/Libraries/Include/og/Console.h)`>`
    * Includes everything needed

## Dependencies ##
  * [Shared](LibraryShared.md)
  * [Common](LibraryCommon.md)
  * [Math](LibraryMath.md)
  * [FileSystem](LibraryFileSystem.md) ( I'll try to get rid of this dependency )