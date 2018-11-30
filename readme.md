mini_player
====

foobar2000 component `foo_title` skin.

![preview](https://github.com/twilyze/foo_title_mini_player/blob/master/image/preview.png)


## Prerequisites
1. [foo_title](https://github.com/TheQwertiest/foo_title)  [(Download)](https://github.com/TheQwertiest/foo_title/releases)
1. [Playback Statistics](https://www.foobar2000.org/components/view/foo_playcount)


## Download
[Release page](https://github.com/twilyze/foo_title_mini_player/releases) 
`mini_player.zip`


## Usage
![usage](https://github.com/twilyze/foo_title_mini_player/blob/master/image/usage.png)

<br>

Edit `skin.xml` if you want to display only during playback.

```xml
<layer name="background" type="absolute-images">
<geometry type="absolute">
  <size x="384" y="48"/>    <!-- Default -->
  <position x="0" y="0"/>
</geometry>


<!-- Replacement code -->
  <!-- Displayed only during playback -->
  <size x="$if(%ispaused%,0,$if(%isplaying%,384,0))" y="48"/>

  <!-- Hide only while paused -->
  <size x="$if(%ispaused%,0,384)" y="48"/>

  <!-- Hide only while stopped -->
  <size x="$if(%isplaying%,384,0)" y="48"/>
```

## License
[cc0 1.0](https://github.com/twilyze/foo_title_mini_player/blob/master/LICENSE)
