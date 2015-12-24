## Features ##

The idea is to have a model loader that can be used for any rendering engine.<br />
It should be able to do static models as well as skeletal animated models.<br />
It should have importers for the most popular formats, so there is no need for special plugins.<br />
But it should also have a native binary model format for fast loading.<br />
Currently importing works including the skeletal information, but it's only static models for now.

Model Import for:
  * ASE ( Unreal )
  * MD3 ( Quake 3 )
  * MD5 ( Doom 3 )
  * SKM ( QFusion )
  * SMD ( Halflife )

## List of authors ##
  * Santo Pfingsten (TTK-Bandit)

## Includes ##
  * `<`[og/Model.h](http://code.google.com/p/open-game-libraries/source/browse/trunk/Libraries/Include/og/Model.h)`>`
    * Includes everything needed

## Dependencies ##
  * [Shared](LibraryShared.md)
  * [Common](LibraryCommon.md)
  * [Math](LibraryMath.md)