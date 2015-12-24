## Description ##
The **Common** library is the first Library we worked on.<br />
Back then it was named ogShared. We renamed it when refactoring the code.<br />
This library contains various classes and functions for creating games.<br />
This library contains various container types, string processing,<br />
and other usefull things that make your everyday game code a lot easier.<br />
The math part of this library has been separated into a new Library [Math](LibraryMath.md).

## Classes and Features ##

  * Containers:
    * Allocator (allocates a list of objects instead of manually allocating each object)
    * CmdArgs (tokenizes a string into command-line arguments)
    * Dict/DictEx (fast access dictionaries for things like entity settings)
    * DynBuffer (easy buffer allocation/resizing/freeing)
    * HashIndex (Fast access to string based indices)
    * List classes
      * LinkedList (optimized for fast insert/remove)
      * List (list growing with a granularity for faster memory allocation)
      * ListEx (optimized for bigger items)
        * StringList (string lists)
    * StringPool/PoolString (store less copies of often used strings in memory)
    * Queue/Stack (push & pop lists)

  * Text:
    * Lexer (UTF-8 text file parser)
    * Parsers:
      * DeclParser (.decl file parser)
      * XDeclParser (.xdecl file parser)

  * Thread helpers:
    * C++0x oriented thread design using boost::threads until the compilers support c++0x.
    * Enhanced thread handling
    * Thread local storage
    * Multithreaded job manager
    * Multithreaded preload manager
    * Lock free queue ( single producer / single consumer )
    * Low lock queue ( multi producer / multi consumer )
    * Event queue

## List of authors ##
  * Santo Pfingsten (TTK-Bandit)
  * Ensiform
  * George Alysan (Muggen)

## Includes ##
  * `<`[og/Common.h](http://code.google.com/p/open-game-libraries/source/browse/trunk/Libraries/Include/og/Common.h)`>`
    * Includes everything except the following
  * `<`[og/Common/Thread/Thread.h](http://code.google.com/p/open-game-libraries/source/browse/trunk/Libraries/Include/og/Common/Thread/Thread.h)`>`
    * Threads interface
  * `<`[og/Common/Thread/LockFreeQueue.h](http://code.google.com/p/open-game-libraries/source/browse/trunk/Libraries/Include/og/Common/Thread/LockFreeQueue.h)`>`
    * LockFreeQueue and LowLockQueue
  * `<`[og/Common/Thread/ThreadLocalStorage.h](http://code.google.com/p/open-game-libraries/source/browse/trunk/Libraries/Include/og/Common/Thread/ThreadLocalStorage.h)`>`
    * Thread Local Storage
  * `<`[og/Common/Thread/JobManager.h](http://code.google.com/p/open-game-libraries/source/browse/trunk/Libraries/Include/og/Common/Thread/JobManager.h)`>`
    * Job Manager
  * `<`[og/Common/Thread/PreloadManager.h](http://code.google.com/p/open-game-libraries/source/browse/trunk/Libraries/Include/og/Common/Thread/PreloadManager.h)`>`
    * Preload Manager

## Dependencies ##
  * [Shared](LibraryShared.md)
  * boost::threads ( just until c++0x is ready )