# Audio Element

`<audio> </audio>`

**Attributes:** (optional)

- src
- type 
- autoplay 
- controls
- loop
- preload: none, metadata, auto
- title 

###Source Element###

`<source>`

self-contained, void --> specifies media file or MIME type
- **MP3 File**: type="audio/mpeg"
- **Vorbis Codec**: type="audio/ogg"


**Example**

with controller for audio  file

```html
<audio controls="controls">
    <source src="musicfile.mp3" type="audio/mpeg">
    <source src="musicfile.ogg" type="audio/ogg">
    <a href="musicfile.mp3">Download this file</a>
</audio>
```

