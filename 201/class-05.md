# HTML Images, CSS Color & Text
In `class-05` we will talk about HTML image and CSS color & text.
## HTML :
### HTML IMAGE :
Why we use images in web site:
Image say many words, and great images help make the difference between an average-looking site and a really engaging one.
### Adding Images :
`<IMG>` tag is used to insert images in any webpage. Its two main attributes are as follows:
* **SRC** : It specifies the URL of the image.
* **ALT** : It specifies an alternate text for an image.
We use `<img>` tag like follows:
```
<img src="img.jpg" alt="image">
```
### Image Size - Width and Height :
The `width` and `height` attributes always define the width and height of the image

you can use the width and height attributes : inline like follows :
```
<img src="img.jpg" alt="image" width="500" height="600">
```
And you can use it in CSS as follows :
```
img {
  width: 100%;
  height: 50%;
}
```
### Supported Image Formats :
1. **JPEG** (Joint Photographic Expert Group image) :
    * Good choice for lossy compression of still images.
2. **PNG** (Portable Network Graphics) :
    * PNG is preferred over JPEG for more precise reproduction of source images, or when transparency is needed.
3. **GIF** (Graphics Interchange Format) :
    * Good choice for simple images and animations.
4. **WebP** (Web Picture format) :
   * Excellent choice for both images and animated images.
5. **SVG** (Scalable Vector Graphics) :
    * Vector image format; ideal for user interface elements, icons, diagrams, etc., that must be drawn accurately at different sizes.
6. **APNG** (Animated Portable Network Graphics) :
    * Good choice for lossless animation sequences.
7. **AVIF** (AV1 Image File Format) :
    * Good choice for both images and animated images due to high performance and royalty free image format. It offers much better compression than PNG or JPEG with support for higher color depths, animated frames, transparency etc. Note that when using AVIF, you should include fallbacks to formats with better browser support.
## CSS
### Color in CSS :
Color can really bring your pages to life.
### Text Color :
You can set the color of text by adding `color` : attribute followed by the value as follows :
```
h1{ 
    color:red;
}
```
### Background Color :
You can set the background color for HTML elements by adding `background-color` : attribute followed by the value as follows :
```
h1{
     background-color:DodgerBlue;
}
```
### CSS Fonts :
Choosing the right font for your website is important! Choosing the right font has a huge impact on how the readers experience a website. The right font can create a strong identity for your brand. Using a font that is easy to read is important. The font adds value to your text. It is also important to choose the correct color and text size for the font.

### Font Family :
You can set the font family for HTML elements by adding `font-family` : attribute followed by the value as follows :
```
h1{
     font-family:Georgia, Times, serif;
}
```
### Font Size :
The `font-size` property in CSS is used to specify the height and size of the font. It affects the size of the text of an element. Its default value is medium and can be applied to every element.

You can set the font size for HTML elements by adding `font-size` : attribute followed by the value as follows :
```
h1 {
  font-size: 15px;
}
```
## TL;DR :
Use JPEG format for all images that contain a natural scene or photograph where variation in colour and intensity is smooth. Use PNG format for any image that needs transparency or for images with text & objects with sharp contrast edges like logos. Use GIF format for images that contain animations.

### JPEG vs PNG vs GIF :
You should be aware of a few key factors.

First, there are two types of compression: `Lossless` and `Lossy`.
* **Lossless** : means that the image is made smaller, but at no detriment to the quality.
* **Lossy** : means the image is made (even) smaller, but at a detriment to the quality. If you saved an image in a Lossy format over and over, the image quality would get progressively worse and worse.

There are also different colour depths (palettes): `Indexed color` and `Direct color`.
* **Indexed** : means that the image can only store a limited number of colours (usually 256), controlled by the author, in something called a Color Map.
* **Direct** : means that you can store many thousands of colours that have not been directly chosen by the author.
### JPEG - Lossy / Direct :
JPEGs images were designed to make detailed photographic images as small as possible by removing information that the human eye won't notice. As a result it's a Lossy format, and saving the same file over and over will result in more data being lost over time. It has a palette of thousands of colours and so is great for photographs, but the lossy compression means it's bad for logos and line drawings.
### PNG-8 - Lossless / Indexed

PNG is a newer format, and PNG-8 (the indexed version of PNG) is really a good replacement for GIFs. Sadly, however, it has a few drawbacks: Firstly it cannot support animation like GIF can (well it can, but only Firefox seems to support it, unlike GIF animation which is supported by every browser). Secondly it has some support issues with older browsers like IE6. Thirdly, important software like Photoshop have very poor implementation of the format.
### GIF - Lossless / Indexed only

GIF uses lossless compression, meaning that you can save the image over and over and never lose any data. The file sizes are much smaller than BMP, because good compression is actually used, but it can only store an Indexed palette. This means that for most use cases, there can only be a maximum of 256 different colours in the file. That sounds like quite a small amount, and it is.

GIF images can also be animated and have transparency.

Good for: Logos, line drawings, and other simple images that need to be small. Only really used for websites.

***Reference*** :

* [JPEG vs PNG vs GIF ](https://stackoverflow.com/questions/2336522/what-are-the-different-usecases-of-png-vs-gif-vs-jpeg-vs-svg)