
Chromeless YouTube Video Player
=============

Implementing a Chromeless YouTube video player and custom controls

Features
-------

* support for mobile browsers and tablets


### Holder Element

    <div id="player"></div>

Here we create an element to house the video we are playing. 


### Player Controls 

    <div id="player-controls">
        <ul>
            <li class=play><a href="#">play</a></li>
            <li class="pause"><a href="#">pause</a></li>
        </ul>
    </div>

Build out elements to define video play controls


### Video Debug Data

     <div id="videoInfo">
        <p>Current Time: <span id="videoCurrentTime">0</span> | Duration: <span id="videoDuration">0</span></p>

        <p>Bytes Total: <span id="bytesTotal">0</span> | Start Bytes: <span id="startBytes">0</span> | Bytes Loaded: <span id="bytesLoaded">0</span></p>

Show video play time and progress meter data

### Seek through video 

      <p class=seek-demo><a href="#">jump to 2:00</a></p>
      <p class=seek-demo2><a href="#">jump to 4:00</a></p>

Create links to skip to designated point in video

### Video progress
      <div id=seek_video_slider>
          <div id="knob"></div>
      </div>

Generate video play progress holder

### Load iframe

      var tag = document.createElement('script');
      tag.src = "http://www.youtube.com/player_api";
      var firstScriptTag = document.getElementsByTagName('script')[0];
      firstScriptTag.parentNode.insertBefore(tag, firstScriptTag);

This code loads the IFrame Player API code asynchronously.





Contributing
------------

1. Fork it.
2. Create a branch (`git checkout -b my_markup`)
3. Commit your changes (`git commit -am "added code"`)
4. Push to the branch (`git push origin my_markup`)
5. Create an [Issue][1] with a link to your branch


