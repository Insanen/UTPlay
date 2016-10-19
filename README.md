![UTPlay - YouTube Music Player](UTPlay.png)
### Welcome to UTPlay.
YouTube Playlist with class - This simple script will allow you to integrate any YouTube Public Playlist into a CSS3 and Javascript audio player.  YouTube Playlist will allow you to get only the sound out of your videos by hiding the block of the video frame.
If your having issues playing your playlist, Please make sure your playlist is not private.

[Submit a bug](https://github.com/Insanen/UTPlay/issues)

### Install
* Download files from `src` folder.
* Include files inside `src` on your page.
  `<link rel="stylesheet" type="text/css" href="src/utplay.min.css">`
  `<script src="src/utplay.min.js"></script>`

### How to use it
Simple, After adding the script dependencies use the html markup to add your player in place.

```
<div align="center">
    <iframe id="video" name="x" src="//www.youtube.com/embed/?list=YOUR_PLAYLIST&amp;index=0&amp;listType=playlist&amp;enablejsapi=1&amp;fs=0&amp;rel=0&amp;showinfo=0&amp;modestbranding=1&amp;iv_load_policy=3&amp;controls=0&amp;autoplay=0&amp;loop=0"
        frameborder="0" allowfullscreen></iframe>

    <div class="buttons">
        <a class="myPlayBtn" id="play-button" href="#play-button-shape">
            <div class="play"></div>
        </a>
        <a class="myPauseBtn" id="pause-button" href="#pause-button-shape">
            <div class="pause"></div>
        </a>
        <a class="myNxtBtn" id="next-button" href="#next-button-shape">
            <div class="nxt"></div>
        </a>
    </div>

```

Now this is the only part that gets a bit tricky, You will need to find your YouTube Playlist ID and place it within the HTML markup of Iframe.

For my example, I am going to take a playlist I've created for this project `https://www.youtube.com/playlist?list=PLr7KBbNMX5CTXyY1_GKjHAzrIPJRs6Cpo` so my ID for this playlist will be `PLr7KBbNMX5CTXyY1_GKjHAzrIPJRs6Cpo`.
Yes so pretty much everything after `playlist?list=This_Is_Your_Id`.

After we obtaining our YouTube Playlist ID, We go ahead and plug it inside our iframe markup, like this;

```
<div align="center">
    <iframe id="video" name="x" src="//www.youtube.com/embed/?list=PLr7KBbNMX5CTXyY1_GKjHAzrIPJRs6Cpo&amp;index=0&amp;listType=playlist&amp;enablejsapi=1&amp;fs=0&amp;rel=0&amp;showinfo=0&amp;modestbranding=1&amp;iv_load_policy=3&amp;controls=0&amp;autoplay=0&amp;loop=0"
        frameborder="0" allowfullscreen></iframe>

    <div class="buttons">
        <a class="myPlayBtn" id="play-button" href="#play-button-shape">
            <div class="play"></div>
        </a>
        <a class="myPauseBtn" id="pause-button" href="#pause-button-shape">
            <div class="pause"></div>
        </a>
        <a class="myNxtBtn" id="next-button" href="#next-button-shape">
            <div class="nxt"></div>
        </a>
    </div>

```  

## Change Theme color

![UTPlay - YouTube Music Player](UTPlay-Pix.png)

It's quite simple, the CSS will handle the change by only adding a new class next to the already existing class `buttons` We are going to integrate the Pix theme by doing this code instead.

```
<div align="center">
    <iframe id="video" name="x" src="//www.youtube.com/embed/?list=PLr7KBbNMX5CTXyY1_GKjHAzrIPJRs6Cpo&amp;index=0&amp;listType=playlist&amp;enablejsapi=1&amp;fs=0&amp;rel=0&amp;showinfo=0&amp;modestbranding=1&amp;iv_load_policy=3&amp;controls=0&amp;autoplay=0&amp;loop=0"
        frameborder="0" allowfullscreen></iframe>

    <div class="buttons pix">
        <a class="myPlayBtn" id="play-button" href="#play-button-shape">
            <div class="play"></div>
        </a>
        <a class="myPauseBtn" id="pause-button" href="#pause-button-shape">
            <div class="pause"></div>
        </a>
        <a class="myNxtBtn" id="next-button" href="#next-button-shape">
            <div class="nxt"></div>
        </a>
    </div>

```  

Pretty much the only line that changed was `<div class="buttons">` to `<div class="buttons pix">`...

Happy Coding www.insanen.com
