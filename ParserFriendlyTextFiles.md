## About ##

**Parser Friendly Text Files** are UTF-8 encoded text files starting with a [Byte Order Mark](http://de.wikipedia.org/wiki/Byte_Order_Mark).

## Comments ##
These files can contain single line comments and multiline comments:
```
// C++ style comments end with the next newline.
/*
   You can add multiline comments too
   Just like in C
*/
```

## Tokens ##
When these text files are parsed for tokens, a token ends when a whitespace (space, tab, newline) or a single character token is found.<br />
Some tokens are single character, i.e. they end after the character itself: { } ( ) , ; $ = /<br />
You can avoid this behavior and add for example full sentences by putting them into quotes.<br />
Quotes can be done with either " or '. Depending on which you start with, it will search for the same char to end the string.

## Escape characters ##
You can escape some characters inside a quoted string:
  * \n creates a newline
  * \t creates a tab
  * \" creates a "
  * \' creates a '

## Example ##
The folling file:
```
 say( "hello \"world\"" /* you can't see me */ ); // can't see this either
```
..would result in these tokens:
  * say
  * (
  * hello "world"
  * )
  * ;

## See also ##
Use the Lexer class to create your own parser.