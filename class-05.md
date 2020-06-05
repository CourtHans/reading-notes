# Class 5 reading notes

**HTML & CSS** *Jon Duckett*

- Chapter 5: “Images” (pp.94-125)
- Chapter 11: “Color” (pp.246-263)
- Chapter 12: “Text” (pp.264-299)

### Images

Since images can take longer to load than HTML code, it's a good idea to specify the size of the image so teh browser can render the rest of the text on the page while leaving the right amount of space ofr the image that is still loading.

***Three rules for creating images***
1. Save images in the right format
2. Save images at the right size
3. Measure images in pixels

*Online photo editors*  
www.photoshop.com  
www.pixlr.com  
www.splashup.com  
www.ipiccy.com  

Use JPEG for images with many different colors (like photographs) 
us GIF or PNG when saving images with few colors (like logos)

The images you use should be saved at the same width and height that you want them to appear on the page. It is best to source images that are the correct shape, if possible. 

When you want to add a caption, you could use the `<figure>` element as a container for your image and the caption. The tag for the caption is `<figcaption>`.

### Color

[Adobe Color Tool link](https://color.adobe.com/create)

Color helps bring your site to life!

There are three ways to specify colors in CSS:
1. RGB Values (red, green, blue - expressed as numbers b/w 0-255)
2. hex codes (6-digit codes that represent amount of r, g, and b in a color -preceded by a `#` - e.g. `#ee3e80`); hsl and hsla - hue, saturation, lightness, opacity
3. color names - there are 147 predefined color names recognized by browsers)

**Color pickers** can help you find the color you want

It is *critical* to ensure proper contrast between your background color and text for easy reading

**Hex values** represent values for red, green, and blue in dexadecimal code. If two digits/letters are the same within each grouping, they can be represented by a single.

**RGBA** is the value attributed to opacity for RGB colors with the "a" indicating alpha for opacity (represented as a decimal between 0 and 1 to indicate percentage of transparency).

CSS3 allows you to specify colors as HSL values, with an optional opacity - it's known as **HSLA** (hue, saturation, lightness, alpha (transparency)).

Since some browsers do not recognize RGBA, HSL or HSLA, it is a good idea to add an extra rule which specifies the color using a hex code, RGBA value, or color name *before* the rule that uses HSL or HSLA (in the case of unsupported RGBA, the color would appear solid).

### Text

The properties that allow you to control the appearance of text can be split into two groups.
1. Those that directly affect the ont and its appearance (e.g. typeface, bold, italic, size of text, etc.).
2. Those that would have the same effect on text no matter what font you were using (e.g. color, spacing b/w words, etc.)

Browsers don't have a standard set of typefaces they support, therefore, it is common to add the generic font name after your preferred choice of typefaces. **For example**
```
font-family; Georgia, Times, serif;
```
You can specify a list of fonts separated by commas so that if the user does not have your first choice of typeface installed, the browser can try to use an alternative font from t he list. It is also common to end with a generic font name fot that type (p. 269-270).

Setting font size in pixels is the best way to ensure that the type appears at the size you intended (but you can also use percentages and ems).

`@font-face` allows you to use a font, even if it is not installed on the computer of the person browsing.

You could also link to a CSS file and font files on google servers: www.google.com/webfonts

In CSS, the line-height property sets the height of an entire line of text, so the difference between teh font-size and the line-height is equivalent to the leading. Increasing the line-height makes the vertical gap between lines of text larger and can makethe text easier to read. A good starter setting is around 1.4 to 1.5em (best practice, use ems and not pixels).

`vertical-align` is **not** intended to allow you to vertically align text in teh middle of block level elements.

**Links** - you can set a style for links that have not yet been visited (`:link`) and/or links that have been visited (`:visited`). (These are pseudo-classes.)

`:hover`, `:active`, and `:focus` are three pseudo-classes that allow you to change the appearance of elements when a user is interacting with them.

When pseudo-classes are used, they should appear in this order:

1. `:link`
2. `visited`
3. `:hover`
4. `:focus`
5. `:active`

***More attribute selectors***

`[]` existence -matches a specific attribute  
`[=]` equality - matches a specific attribute with a specific value  
`[~=]` space - matches a specific attribute whose value appears in a space-separated list of words  
`[^]` prefix - matches a specific attribute whose value begins with a  specific string  
`[*=]` substring -matches a specific attribute whose value contains a specific substring  
`[$=]` suffix - matches a specific attribute whose value ends with a specific string.

<hr />

[Previous - Class 4 reading notes](class-03.md) 

[Return to Table of Contents](README.md)