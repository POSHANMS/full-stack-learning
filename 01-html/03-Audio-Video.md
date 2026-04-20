<!--Audio Elements-->

<audio src="https://cdn.freecodecamp.org/curriculum/js-music-player/cruising-for-a-musing.mp3" controls></audio>

<p>The controls attribute enables users to manage audio playback, including pausing or resuming playback. </p>
<br>
<hr>

<!--Loop-->

<audio
src="https://cdn.freecodecamp.org/curriculum/js-music-player/can't-stay-down.mp3"
loop
controls

> </audio>
> <br>

<hr>

<!--Muted-->

<audio
src="https://cdn.freecodecamp.org/curriculum/js-music-player/can't-stay-down.mp3"
loop
controls
muted

> </audio>
> <br>

<hr>

<audio controls>
  <source src="audio.ogg" type="audio/ogg" />
  <source src="audio.wav" type="audio/wav" />
  <source src="audio.mp3" type="audio/mpeg" />
</audio>
<p>The browser will first start with the ogg type, and if it can't play the audio, then it'll move down to the next type in the list.</p>
<br>
<hr>

<!--Video Element-->

<video
src="https://archive.org/download/BigBuckBunny_124/Content/big_buck_bunny_720p_surround.mp4"
loop
controls
muted
width="400"

> </video>
> <br>

<hr>

<!--Poster Attribute-->

<video
src="https://archive.org/download/BigBuckBunny_124/Content/big_buck_bunny_720p_surround.mp4"
loop
controls
muted
poster="https://peach.blender.org/wp-content/uploads/title_anouncement.jpg?x11217"
width="400"

> </video>

<!-- Optimize Media Assets-->

Three tools to consider when using media, such as images, on your web pages:

1. The size ->
   A smaller resolution results in a smaller file size.
   Your images should be the same scale as the rendered size on the page.

2. The format ->
   Two of the most common file formats are PNG and JPG, but these are no longer the most ideal formats for serving images.
   you should consider using a more optimized format, like WEBP or AVIF.

3. The compression ->
   Tools like pngcrush work well for lossless formats like PNG, which can be compressed without any quality loss since the original data can be perfectly reconstructed.
   JPG, for example, uses lossy compression — each time a JPG is re-saved or re-compressed, some image data is permanently discarded, resulting in degraded quality.

 <!--Different Types of Images Licenses--!>

Images are considered intellectual property, this means that they are protected by copyright regulations
This means that you cannot use them in your web page unless you do one of three things: obtain written permission from the copyright holder, purchase a license from the copyright holder, or incorporate the image in a way that falls under fair use.

That third point is a bit tricky. Fair use requires that your use of the image is both limited and transformative. Some examples of fair use would be to comment on or review the art or create a parody of the image.

Most search engines will allow you to filter image results by a license. There are also sites like Pixabay and Unsplash, which offer free-to-use images.

<!--SVGs--!>
PNG and JPG are classified as raster formats. This essentially means that they are pixel-based, with the data tracking the color value in each pixel.

SVG stands for a scalable vector graphic
A vector graphic tracks data based on paths and equations to plot points, lines, and curves. 
SVG can be scaled to any size without impacting the quality.

SVGs specifically have the added benefit of storing data in XML. This means you can use them directly in your code as raw HTML with the svg element. It also means you can programmatically change the color of the image.

<svg width="100" height="100" viewBox="0 0 100 100" xmlns="http://www.w3.org/2000/svg">
  <circle cx="50" cy="50" r="45" stroke="black" stroke-width="4" fill="yellow" />
  <circle cx="35" cy="40" r="5" fill="black" />
  <circle cx="65" cy="40" r="5" fill="black" />
  <path d="M35 65 Q50 80 65 65" stroke="black" stroke-width="4" fill="transparent" />
</svg>

The svg element is the container for the whole drawing. It sets up the space where all the shapes appear. Everything you want to draw with SVG, such as circles, lines, or paths, goes inside the svg element.

The circle element is used to make the face and the eyes. One large circle forms the yellow face, and two smaller circles make the eyes.

The path element is used to draw the smile. It creates a curved line for the mouth.
Each SVG element has attributes that control its appearance and position within the drawing area.
