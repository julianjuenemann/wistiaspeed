## Synopsis

Wistia Speed options is a Bookmarklet that will let you speed up embedded Wistia videos.

## the Code

javascript:(function()%7Bvar speed %3D Wistia.api("wistia").playbackRate()%3Bif(speed %3D%3D%3D 3)%7Bspeed %3D 1%3B%7Delse%7Bspeed %3D speed %2B 0.5%3B%7DWistia.api("wistia").playbackRate(speed)%7D)()

## Motivation

I love YouTube's speed feature. Wistia should have the same.

## Installation

1. Drag the [WistiaSpeedUp](javascript:(function(\)%7Bvar speed %3D Wistia.api("wistia"\).playbackRate(\)%3Bif(speed %3D%3D%3D 3\)%7Bspeed %3D 1%3B%7Delse%7Bspeed %3D speed %2B 0.5%3B%7DWistia.api("wistia"\).playbackRate(speed\)%7D\)(\)) Bookmarklet into your bookmark bar
2. Find an embedded video
3. make sure it is playing the HTML5 Version of the video (right click on the video)
4. Click on the Bookmarklet to speed up your video by a factor of 0.5 x the speed.

##Functionality

Once activated the video will be speed up by a factor of 0.5x Another click will ad 0.5x to the speed till it reaches 3x the speed when it will reset to 1

- First Click: 1.5x speed
- Second Click: 2x speed
- Third Click: 2.5x speed
- Forth Click: 3x speed
- Fifth Click: reset to 1x speed

## API Reference

This Bookmarklet is based on the [JavaScript Player API](http://wistia.com/doc/player-api) of Wistia.


## License

The Bookmarklet is published under the MIT license
