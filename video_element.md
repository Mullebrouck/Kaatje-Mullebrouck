# Video Element

`<video> </video>`

**Attributes:** (optional)

- src
- type 
- autoplay 
- controls
- loop
- preload: none, metadata, auto
- title 
- height
- width
- poster (displays image when browser can not play video)

###Source Element###

`<source>`

self-contained, void --> specifies media file or MIME type
- **Video File**: type="video/mp4"
- **Vorbis Codec**: type="video/ogg"


**Example**

with controller for video file

```html
<audio controls="controls">
    <source src="musicfile.mp3" type="audio/mpeg">
    <source src="musicfile.ogg" type="audio/ogg">
    <a href="musicfile.mp3">Download this file</a>
</audio>
```

Controller for Audio File: 

[](codepen://Kaatje/GobeEm)


**Converting Audio file to OGG Vorbis Codec:**

http://audacity.sourceforge.net

Free web converter: http://www.archive.org



