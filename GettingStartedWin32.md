## What you need ##
  * A C++ IDE, I'd recommend Visual C++ 2008, since there is also a free version ( Express Edition )
  * [Visual Leak Detector 2.0b](http://vld.codeplex.com/) ( you can do without by uncommenting the OG\_VISUAL\_LEAK\_DETECTOR define in the Setup.h )
  * [Direct-X SDK](http://www.microsoft.com/downloads/en/details.aspx?displaylang=en&FamilyID=3021d52b-514e-41d3-ad02-438a3ba730ba) ( If you want to use [Fable](LibraryFable.md) )
  * [Premake 4](http://industriousone.com/premake) (if you want to update/create project or make files)

## How to set up ##
  1. Install your IDE
  1. [Install and set up Visual Leak Detector](http://vld.codeplex.com/documentation)
  1. Install the Direct-X SDK and set it up the same way as VLD ( add include and library directories to your IDE )
  1. If you don't use Visual Studio 2008, you'll need to create project/make files for your IDE. Check out Premake4 for how to do it.
  1. Load and build all solutions in this order:
    1. Thirdparty
    1. Libraries
    1. Examples

Correct me if I missed something.