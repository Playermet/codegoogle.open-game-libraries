## Features ##
  * TGA, PNG, JPEG, DDS file loading
  * TGA, PNG, JPEG file storing
  * [RoundDown and PicMip](ImageQuality.md) at load time
  * Min/Mag filter changes in runtime
  * Reload all images (when changes where done or the gl context was lost)
  * Preload images in separate threads using the PreloadManager
  * Reload images using the PreloadManager (optional)

## List of authors ##
  * Santo Pfingsten (TTK-Bandit)

## Includes ##
  * `<`[og/Image.h](http://code.google.com/p/open-game-libraries/source/browse/trunk/Libraries/Include/og/Image.h)`>`
    * Includes everything needed

## Dependencies ##
  * [Shared](LibraryShared.md)
  * [Common](LibraryCommon.md)
  * [Math](LibraryMath.md)
  * [libJPEG](http://www.ijg.org/)
  * [libPNG](http://www.libpng.org/pub/png/libpng.html)