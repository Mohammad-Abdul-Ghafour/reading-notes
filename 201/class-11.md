# Audio, Video, Images
## Images :
Today we will Talk about images and some of it's properties.

### Controlling sizes of images in CSS :
Sometimes, it is required to fit an image into a certain given dimension. We can resize the image by specifying the `width` and `height` of an image.

And we can align images using float property.

### Main Properties for Images :
1. **`background-image`**
    * The *`background-image`* property sets one or more background images for an element.
2. **`background-repeat`**
    * The *`background-repeat`* property sets if/how a background image will be repeated.
    * property can have four values:
        * `repeat`
        * `repeat-x`
        * `repeat-y`
        * `no-repeat`
        * `fixed`
        * `scroll`
3. **`background-attachment`**
    * The *`background-attachment`* property sets whether a background image scrolls with the rest of the page, or is fixed.
4. **`background-position`**
    * The *`background-position`* property sets the starting position of a background image.
## Search Engine Optimizatio (SEO) :
Search engine optimization helps visitors find your sites when using search engines.

Analytics tools such as Google Analytics allow you to see how many people visit your site, how they find it, and what they do when they get there.

To put your site on the web, you will need to obtain a domain name and web hosting.

## Audio in HTML :
The HTML **`<audio>`** element is used to play an audio file on a web page.
The **`controls`** attribute adds audio controls, like play, pause, and volume.

Example :

```
<audio controls>
  <source src="horse.ogg" type="audio/ogg">
  <source src="horse.mp3" type="audio/mpeg">
Your browser does not support the audio element.
</audio>
```
1. **`autoplay`**
    * Udes to start a video automatically,
2. **`muted`**
    *   Add *`muted`* after *`autoplay`* to let your video start playing automatically but muted.

## Videos in HTML :
The **`<video>`** tag is used to embed video content in a document, such as a movie clip or other video streams.The **`<video>`** tag contains one or more **`<source>`** tags with different video sources. The browser will choose the first source it supports.

Example :

```
<video width="320" height="240" controls>
  <source src="movie.mp4" type="video/mp4">
  <source src="movie.ogg" type="video/ogg">
Your browser does not support the video tag.
</video>
```

### Videos Properties :
1. **`autoplay`**
    * Udes to start a video automatically,
2. **`muted`**
    *   Add *`muted`* after *`autoplay`* to let your video start playing automatically but muted.
