# HTML Multimedia Tags

HTML provides several tags to handle multimedia elements such as images, audio, and video. These tags allow you to embed and control various types of media directly within a web page. Below is an overview of the main HTML multimedia tags and their attributes.

## 1. `<img>`

The `<img>` tag is used to embed images in a web page. It is a self-closing tag.

**Attributes**:
- `src`: Specifies the path to the image file.
- `alt`: Provides alternative text for the image if it cannot be displayed.
- `width`: Specifies the width of the image.
- `height`: Specifies the height of the image.

**Example**:
```html
<img src="path/to/image.jpg" alt="Description of the image" width="600" height="400">
```

## 2. `<audio>`

The `<audio>` tag is used to embed sound content in a web page.

**Attributes**:
- `src`: Specifies the path to the audio file.
- `controls`: Adds audio controls such as play, pause, and volume.
- `autoplay`: Starts playing the audio automatically.
- `loop`: Repeats the audio after it finishes.
- `muted`: Mutes the audio.

**Example**:
```html
<audio src="path/to/audio.mp3" controls>
    Your browser does not support the audio element.
</audio>
```

## 3. `<video>`

The `<video>` tag is used to embed video content in a web page.

**Attributes**:
- `src`: Specifies the path to the video file.
- `controls`: Adds video controls such as play, pause, and volume.
- `autoplay`: Starts playing the video automatically.
- `loop`: Repeats the video after it finishes.
- `muted`: Mutes the video.
- `poster`: Specifies an image to be shown while the video is downloading or until the user hits the play button.
- `width`: Specifies the width of the video.
- `height`: Specifies the height of the video.

**Example**:
```html
<video src="path/to/video.mp4" controls width="600" height="400">
    Your browser does not support the video tag.
</video>
```

## 4. `<source>`

The `<source>` tag is used to specify multiple media resources for elements such as `<audio>` and `<video>`. It allows you to provide different file formats to ensure compatibility with various browsers.

**Attributes**:
- `src`: Specifies the path to the media file.
- `type`: Specifies the MIME type of the media file.

**Example**:
```html
<video controls width="600" height="400">
    <source src="path/to/video.mp4" type="video/mp4">
    <source src="path/to/video.ogg" type="video/ogg">
    Your browser does not support the video tag.
</video>
```

## 5. `<track>`

The `<track>` tag is used to specify text tracks for `<video>` and `<audio>` elements. These can be used for subtitles, captions, or other text-based information.

**Attributes**:
- `kind`: Specifies the kind of text track (`subtitles`, `captions`, `descriptions`, `chapters`, or `metadata`).
- `src`: Specifies the path to the track file.
- `srclang`: Specifies the language of the track text.
- `label`: Provides a user-readable title for the track.
- `default`: Specifies that the track should be enabled by default.

**Example**:
```html
<video src="path/to/video.mp4" controls width="600" height="400">
    <track kind="subtitles" src="path/to/subtitles.vtt" srclang="en" label="English">
    Your browser does not support the video tag.
</video>
```

## 6. `<figure>` and `<figcaption>`

The `<figure>` tag is used to group media content and the `<figcaption>` tag provides a caption for the content.

**Example**:
```html
<figure>
    <img src="path/to/image.jpg" alt="Description of the image">
    <figcaption>This is a caption for the image.</figcaption>
</figure>
```

## Summary

HTML provides robust support for embedding and controlling multimedia content through a variety of tags and attributes. By understanding and using these tags, you can create rich, interactive web experiences that incorporate images, audio, and video.