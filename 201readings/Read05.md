# Read: 05 - HTML Images; CSS Color & Text

## Chapter 5: images.

Adding an image:
``` 
<img src=”image URL” alt=”image description to be displayed before if the image doesn’t load title=”this is to display extra information, and it appears in the tooltip, when the user hovers on the image”>
``` 

Also, there is the **<figure></figure>** tag. This is used to add images with their captions. You can have more than one image in this tag, if they have the same caption.
``` 
<figure>
	<img src=”URL img1”> 
	<img src=”URL img2”>
	<figcaption> write down caption here</figcaption>
</figure>
```

Good-Practice list: 
+ Put all of your images in one folder in the project, and sometimes in sub-folders if there are many of them.
+ Three rules for creating images for your website:
1.	Use the right format
2.	Use the right size (as you want it to be in the website)
3.	Use the right resolution -for bitmap images (most laptops **72ppi)
+ Images formats: 
1.	JPEG   for images with diverse colors, but with large areas that have the same or close colors.
2.	PNG/GIF  for images that have large areas with exactly the same colors, and some colors on them. 

## Chapter 11: Color

There are many formats of using colors in CSS, for example: RGB, HEX, and color names.
CSS allows for specifying the colors of foreground, background, and text. When choosing the colors, you should pay attention to the contrast.

### Keywords: 
+ Opacity
+ HSL
+ rgba

## Chapter 12: Text

Text is a basic content in web pages. Its styling is important for readability and compatibility with page design. 

(font-weight  **Bold**  emphasis, contrast, font-style   _italic_ , Stretch)
(Serif, Sans-Serif, Monospace)
Font size(px, percentage,ems 
``` @font-face {
Font-family
Src
Format } ```

**Remember** that browsers do not support all types of fonts, you must provide many formats to suit all of them. 
Use this website for converting: https://www.fontsquirrel.com/ 
Text-transformation  uppercase, lowercase, capitalize 
Text-decoration  underline, overline, line through, blink
Text-align/ vertical-align /indent 




