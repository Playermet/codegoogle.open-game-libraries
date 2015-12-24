## Features ##

This is needed by all libraries, gives commonly used features like FileSystemCore interface ( in case you want to use your own filesystem ), SystemInformation and Threading

## Classes and Features ##
  * FileSystemCore Interface
    * Use this if you want to add your own filesystem instead of using the OG [FileSystem](LibraryFileSystem.md)

  * Format (Typesafe text formatting)

  * Hash:
    * FNV( Compute 32 and 64 bit hashes of strings )
    * SecureHash ( Secure Hash Algorithm: SHA1 )

  * String (UTF-8)

  * SysInfo (retrieves CPU, RAM and OS information)
    * DateTime (Retrieve date & time)

  * Timer (for Profiling)

## List of authors ##
  * Santo Pfingsten (TTK-Bandit)
  * Ensiform

## Includes ##
  * `<`[og/Shared.h](http://code.google.com/p/open-game-libraries/source/browse/trunk/Libraries/Include/og/Shared.h)`>`
    * Includes everything except the following
  * `<`[og/Shared/SecureHash.h](http://code.google.com/p/open-game-libraries/source/browse/trunk/Libraries/Include/og/Shared/SecureHash.h)`>`
    * Secure Hash Algorithm ( SHA-1 )
  * `<`[og/Shared/FileSystemCore.h](http://code.google.com/p/open-game-libraries/source/browse/trunk/Libraries/Include/og/Shared/FileSystemCore.h)`>`
    * Basic Interface for FileSystem Access, also includes File.h
  * `<`[og/Shared/File.h](http://code.google.com/p/open-game-libraries/source/browse/trunk/Libraries/Include/og/Shared/File.h)`>`
    * Basic File Interface ( read/write )

## Dependencies ##
  * None