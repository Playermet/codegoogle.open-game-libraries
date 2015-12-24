## Description ##
The `Open`**GL** **O**`bject` **O**`riented` **T**`oolkit` is a library similar to SDL, GLFW, SFML, etc,<br />
but it is quite different as its sole purpose is to create OpenGL windows, handle monitors and<br />
capture keyboard & mouse input from the user. Everything else does not belong here.

Gloot uses some (heavily rewritten) code from GLFW 2.6 ( Camilla Berglund, http://glfw.sourceforge.net/ ).

## Features ##
  * Heavily rewritten GLFW 2.6 code( Object Oriented, optimized )
    * ..by now, there's not much left of the original code.
  * Create multiple windows
  * Create OpenGL 1,2,3,4 contexts
  * Window messages are handled in a different thread, which enables:
    * Moving and resizing windows without the game freezing
    * Smooth drawing without hickups
  * Do fast fullscreen toggle (without losing OpenGL context)
  * Use native or custom resolution.
  * Support for Multiple monitors (when you toggle fullscreen on the 2nd monitor, it will do it there.)
    * with some extra code on the client, dual monitor drawing should be no problem, maybe even tripple monitor?.
  * Possibility to change Gamma
  * Extended keyboard input code (more keys, simplified input handling)
  * RAW Mouse input ( Win32 ) and native input
  * Joystick code has been removed, working on a separate library for this purpose tho
  * Input is very basic, nothing is stored inside gloot, since you will store your own array mostly anyway.
    * Besides, sometimes it's good to have keyrepeating, for example in the menu, chat or developer console.
  * A seperate header file for input constants/interfaces, so you don't have to mix opengl/gloot headers into your gamelogic files.
  * Removed GLFW threading code for the most part, since there are way better libraries to perform multithreading out there.
  * Removed image loading, there are other libraries much better for that kinda stuff.
  * Full unicode (UTF-8) support

## Planned ##
  * Linux Support (work in progress)
  * Mac support (rewritten from scratch, the glfw mac code is not very popular within the mac community)
  * A few more demo applications
  * More optimizations

## List of authors ##
  * Santo Pfingsten (TTK-Bandit)
  * Some Code used from: [Camilla Berglund](http://glfw.sourceforge.net/)

## Includes ##
  * `<`[og/Gloot.h](http://code.google.com/p/open-game-libraries/source/browse/trunk/Libraries/Include/og/Gloot.h)`>`
    * Includes everything except for glmin.h
  * `<`[og/Gloot/Input.h](http://code.google.com/p/open-game-libraries/source/browse/trunk/Libraries/Include/og/Gloot/Input.h)`>`
    * Only the input specific part of Gloot ( in case you don't want to expose the rest to some part of your code )
  * `<`[og/Gloot/Window.h](http://code.google.com/p/open-game-libraries/source/browse/trunk/Libraries/Include/og/Gloot/Window.h)`>`
    * Only the window specific part of Gloot ( in case you don't want to expose the rest to some part of your code )
  * `<`[og/Gloot/Monitor.h](http://code.google.com/p/open-game-libraries/source/browse/trunk/Libraries/Include/og/Gloot/Monitor.h)`>`
    * Only the monitor specific part of Gloot ( in case you don't want to expose the rest to some part of your code )
  * `<`[og/Gloot/glmin.h](http://code.google.com/p/open-game-libraries/source/browse/trunk/Libraries/Include/og/Gloot/glmin.h)`>`
    * Minimal OpenGL includes

## Dependencies ##
  * [Shared](LibraryShared.md)
  * [Common](LibraryCommon.md)
  * [Math](LibraryMath.md)