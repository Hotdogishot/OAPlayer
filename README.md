# OAPlayer - lightweight, usable, beautiful HTML5 Video Player

## Quick Start
Add these tags to your document's `<head>`:

```html
<link href="OAPlayer.min.css" rel="stylesheet">
<script src="OAPlayer.min..js"></script>
```
Next, using OAPlayer.js is simple just create container `<div id="video_player_container"></div>` element.
Next, initialize manually using the `new OAPlayer({})` function:

```js
var player = new OAPlayer({
                el: "#video_player_container", // (required) Main container
                url: "", // (required) Video url
                type: "video/mp4", // Video type
                title: null, //  (Optional) Video title
                poster: null, // (Optional) Video poster
                logo: null, // (Optional) Add logo to right bottom of player
                autoplay: false,
                muted: false,
                volume: 50,
                autosave: false, 
                forward: false, // (Optional) add a (5sec) forward button
                backward: false, // (Optional) add a (5sec) backward button
                pip: true,
                subtitles: [ // (Optional) Add subtitles, make sure it contains valid JSON!
                {language:"English", src:"./english_sub.vtt", srclang:"en"},
                {language:"Arabic", src:"./arabic_sub.vtt", srclang:"ar"}
                ], 
                cookies_exp: 3000,
                theme: {
                    primary: '#f39c12',
                    controls: '#ffffff',
                    primarytext: '#ffffff',
                    trackheight: "4px",
                    thumbsize: "12px"
                }
             });
```
