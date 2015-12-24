## RoundDown ##
When an image width or height is not a power of 2, it will be resized to the closest power of 2.<br />
If you enable RoundDown, and the closest power of 2 is bigger than the original size, it will choose the lower power of 2 instead.<br />
RoundDown limit is a size below which RoundDown will be ignored.<br />
For example, if you set the RoundDown limit to 64 it won't do the RoundDown if the lower power of 2 is below 64.

## PicMip ##
PicMip is a forced reduction in size. The image width/height will be divided by (2 x PicMip value).<br />
In [og::Image](LibraryImage.md), no reduction will go below 1 px and the textures will always be scaled down to the maximum texture size of the gfx card if above.