# trim.lua
mpv script to create a trim of video files without transcoding.\
Utilizes ffprobe to fetch accurate keyframes.


# Install
```
curl https://raw.githubusercontent.com/aerobounce/trim.lua/master/trim.lua >> ~/.config/mpv/scripts/trim.lua
```


# How to use
`h`: Saves trim start position\
`k`: Saves trim end position
- On second press with the same position invokes write out of a clip.

`shift+h`: Seek to trim start position\
`shift+k`: Seek to trim end position\
`Shift+LEFT`: Seek forwards relatively by minimum keyframes\
`Shift+RIGHT`: Seek backwards relatively by minimum keyframes


# Todo
- [ ] More accurate keyframe fetching.


# Differences from other similar scripts
- This script is aimed only for extraction of clips with **no-transcoding**.
- Without encoding, precise video trimming becomes quite tricky with ffmpeg.
    - As far as I know there is no software that can do it accurately.
    - This script is here to achieve that.
