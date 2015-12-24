## Description ##

You could, for example, store sound attributes or entity definitions inside a .decl file.

## Examples ##
You can store multiple declarations in one file. Starting with the decl Type followed by the name and a set of key/value pairs encapsuled in { }<br />
Notice the **inherit** key/value set, which says "inherit all properties of the specified declaration".<br />
Since inherit will be solved after parsing files, it doesn't matter in what file or at what position in the file the base declaration is.

An entity .decl file could look like this:
```
 entityDecl player {
 	"entityType"	"ogPlayer"
 	"health"		"100"
 	"maxhealth"		"100"
 	"armor"			"100"
 	"maxarmor"		"100"
 }
 
 entityDecl moveable_base {
 	"entityType"	"ogMoveable"
 	"speed"		"10"
 }
 entityDecl moveable_box {
 	"inherit"	"moveable_base"
 	"maxDistance"	"8"
 }
```

A sound .decl file could look like this:
```
 soundDecl vehicles_helicopter {
 	"minDistance"	"1"
 	"maxDistance"	"20"
 	"volume"	"1"
 	"loop"		"1"
 
 	"sound"		"sounds/helicopter.wav"
 }
 
 soundDecl ambience_fire {
 	"minDistance"	"1"
 	"maxDistance"	"20"
 	"volume"	"1"
 	"loop"		"1"
 
 	"sound"	"sounds/fire.ogg"
 }
```
## See Also ##
  * [.xdecl description](XDeclFile.md)
  * [Parser Friendly Text Files](ParserFriendlyTextFiles.md)