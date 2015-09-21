# TechWriting
Kalan Matthews 2015

To run this program you must first have the latest version of Java
Then: 
  -Select Start -> Computer -> System Properties -> Advanced system settings -> Environment Variables -> System variables -> PATH.
  -Prepend C:\Program Files\Java\jdk1.X.X.XX\bin; to the beginning of the PATH variable.
    -X.X.XX is the version that you downloaded.

**This program takes an image that is selected by the user and converts it into an ASCII image**
-The first two lines are importing the java io and java util libraries
-After creating the public class "AsciiImage", variables "shades" "pixel" "width" and "height" are created, these will represent the shades of the pixels from darkest to lightest, an array of characters for the pixels variable, a specified width and a specified height
-A constructor with the arguments of int w and int h creates a new Ascii Image of the specified width and height of the image.
  -The nested for loop iterates through the pixel array and designates the shades.
-The next few lines are to shrink the image in the case that the selected image is larger than the max width/height
-From Lines 38-76,an object is created in which ascii characters replace the pixels in the image
-From Lines 79-83, the actual image itself is created from the scaled down version of the selected image
-The toString funcion returns the new image as a new string, so that the image can be opened in any text editor
