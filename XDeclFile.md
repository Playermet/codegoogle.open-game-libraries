## Description ##

You could, for example, store the description for a Graphical User Interface or a Heads Up Display inside a .xdecl file.

## Examples ##
You start of writing the type of the node, followed by round brackets, which can contain attributes seperated by comma.<br />
Then if you don't need more, you can close it with a semicolon or add more attributes and subnodes within { }.<br />

An hud .xdecl file could look like this:
```
 hud( name='Default Hud' ) {
   author = 'TTK-Bandit & Ensiform';
   // Health Status Group
   group( point='535 420', size='100 50' ) {
     group( point='0 0', size='100 20' ) {
       image( point='0 0', size='100 20', src='gfx/healthprogressback.tga' );
       progressbar( point='2 0', size='96 20', src='gfx/healthprogress.tga', link='player_healthpc', flags='0', colorForHealth='1' );
     }
     text( point='0 30', size='100 20', link='player_health', format='%s HP', family='lucida', fontSize='20', align='1', colorForHealth='1' );
   }
 
   // FPS Display
   text( point='530 10', size='100 16', link='fps', visible='fps', format='^3%s fps', family='lucida', fontSize='16', align='1', color='1 1 0 1' );
 
   // Some Image
   image( point='0 360', size='120 120', src='gfx/tuxedo.png' );
 }
```

Notice how attributes can be set inside the round brackets, separated by comma but also can be set inside the { } brackets.
```
 image( point='0 360', size='120 120', src='gfx/tuxedo.png' );
```
creates the same results as:
```
 image( point='0 360', size='120 120' ) {
   src = 'gfx/tuxedo.png';
 }
```

## See Also ##
  * [.decl description](DeclFile.md)
  * [Parser Friendly Text Files](ParserFriendlyTextFiles.md)