# Video Element + embedding

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
<video 
    controls="controls"
    poster="musicimage.jpg"
    width="160px"
    height="150px">
        <source src="videofile.m4v" type="video/mp4 ">
        <source src="videofile.ogv" type="video/ogg">
        <a href="videofile.mov">Download this file</a>(.mov)
</video>
```

Controller for Video File: 

[](codepen://Kaatje/GobeEm)


**Converting Video file to OGG Vorbis Codec:**

Free web converter: http://www.mirovideoconverter.com


---

#Embedding  to display flash

```html
<video controls="controls">
    <source src="videofile.m4v" type="video/mp4 ">
    <source src="videofile.ogv" type="video/ogg">
    <a href="videofile.mov">Download this file</a>(.mov)
</video>
```


