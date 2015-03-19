gifplayer
===========

Customizable jquery plugin to play and stop animated gifs. Similar to 9gag's
New: Video support (webm, mp4)

###Basic Usage

1. Add a preview of the gif or video file to your website
2. Specify a ‘data-src’ attribute with the path to the animated gif or video, or simply have an image with the same same and the .gif extension in the same folder of the ‘preview’ image
3. Include jquery.js, gifplayer.js and gifplayer.css on your site
4. Call the .gifplayer() method for the desired images

```html
<img id="banana" src="img/banana.png"/>
 
<script>
	$('.gifs').gifplayer();
</script>
```

###Options

Options can be setup in two ways: 
1. Setup as an object when initializing the plugin: 
```javascript
$('#banana').gifplayer({ label: 'play' });
```

2. Setup as data attributes in the preview image: 
```html
<img src="banana.png" data-label="play">
```

Option	|Values	|Default
--- | --- | ---
label	| A value for the label in the circle over the image	|‘gif’
playOn	| Event that triggers playing the animated gif	|'click', 'hover', 'auto'
mode | Load an animated gif file or a video | 'gif', 'video'
src | Source for the animation |
waitUntilLoaded | Would you wait until the animation file has been fully loaded to play, or start playing right away | true, false

