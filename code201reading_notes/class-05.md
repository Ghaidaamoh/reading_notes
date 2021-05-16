# HTML& CSS book:

**chap5:**

- Adding Images:
  - img: To add an image into the page you need to use an *img* element. This is an empty 
   element (which means there is no closing tag). It must carry the following two attributes:
  - src: This tells the browser where it can find the image file.
    This will usually be a relative URL pointing to an image on your own site. 
  - alt: This provides a text description of the image which describes the image if you cannot see it.
  - title: You can also use the title attribute with the *img* element to provide additional information 
   about the image. Most browsers will display the content of this attribute in a tootip when the user hovers over the image.

- Height & Width of Images:

  **height:** This specifies the height of the image in pixels.

  **width:** This specifies the width of the image in pixels.

- Where to Place Images in Your Code:
  Where an image is placed in the code will affect how it is displayed. 
  Here are three examples of image placement that produce different results:

1. before a paragraph: The paragraph starts on a new line after the image.
2. inside the start of a paragraph: The first row of text aligns with the bottom of the image.
3. in the middle of a paragraph: The image is placed between the words of the paragraph that it appears in.

**Figure and Figure Caption**

- figure: Images often come with captions. HTML5 has introduced a new figure element to contain images and their caption 
   so that the two are associated.
- figcaption: The figcaption element has been added to HTML5 in order to allow web page authors to add 
  a caption to an image.
  
**chap11:**
**Color:**

- Color not only brings your site to life, but also helps convey the mood and evokes reactions.
- There are three ways to specify colors in CSS: RGB values, hex codes, and color names.
- Color pickers can help you find the color you want.
- It is important to ensure that there is enough contrast between any text and the background color
 (otherwise people will not be able to read your content).
- CSS3 has introduced an extra value for RGB colors to indicate opacity. It is known as RGBA.
- CSS3 also allows you to specify colors as HSL values, with an optional opacity value. It is known as HSLA.

**Pick a Color:**
![color](https://www.w3schools.com/colors/img_colormap.gif)

**chap12:**
**- Text:**

- Specifying Typefaces font-family:
    The font-family property allows you to specify the typeface that should be used for 
    any text inside the element(s) to which a CSS rule applies.
- Size of Type font-size:
    The font-size property enables you to specify a size for the font. There are several ways to specify the size of a font. 
    The most common are: Pixels are commonly used because they allow web designers very precise control over how much space 
    their text takes up.
- You can control the space between lines of text, individual letters, and words. Text can also be aligned to the left, right, 
    center, or justified. It can also be indented.

## Blog Post:

 **JPEG vs PNG vs GIF — which image format to use and when?**
- TL;DR:
    Use JPEG format for all images that contain a natural scene or photograph where variation in colour and intensity is smooth.

    Use PNG format for any image that needs transparency or for images with text & objects with sharp contrast edges like logos.

    Use GIF format for images that contain animations.

- Compression:
  Compression can be of two types — lossless and lossy. In lossless compression, it is possible to reconstruct the original image
  from the compressed image because there is no information loss during compression.

**JPEG:** is a lossy compression specification that takes advantage of human perception.
**PNG:** is a lossless image format using DEFLATE compression. No data is lost during compression and no compression 
  artefacts are introduced in the image. 

**GIF:** is also a lossless image format that uses LZW compression algorithm. It was favoured over PNG for simple graphics
  in websites in its early days because the support of PNG was still growing.

- Transparency:
  *JPEG* images don’t support transparency and are hence not usable for such cases.

  *PNG* images support transparency in two ways — inserting an alpha channel that allows partial transparency or 
  by declaring a single colour as transparent (index transparency).

  *GIF* images support transparency by declaring a single colour in the colour palette as transparent (index transparency). 
  Because of absence of partial transparency, the edges (specially rounded or too-detailed edges) get a poor jagged effect.  