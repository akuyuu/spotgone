# spotgone
Thing for downloading tracks from spotify through yt but iirc i gave up on last binary part but other than that it (presumably) works<br>
to be fair there are many things i couldve done better so yeah be prepared for some average practices
<br>
## Installation
clone this repo, cd to it and go build it, there are no external dependencies (although you do need ffmpeg(?) & ytdlp)
## Usage
### -id
    Mandatory, ID of the playlist/album, can also be a link
    `./spg ... -id <id>`
### -b
    Mandatory, path to the ytdlp binary which is going to be used to download content
    `./spg ... -b "/path/to/binary"...`
### -t
    Used to specify type of the spotify download, can be either album or playlist (or any case of a/p)
    `./spg ... -t playlist ...`
### -d
    Download path, by default creates folder named "Downloads"
    `./spg ... -d "/some/path" ...`
### -f
    Downloaded file format, can be any of aac, alac, flac, m4a, mp3, opus, vorbis, wav, mp3 by default
    `./spg ... -f m4a ...`
### -r
    Number of downloader goroutines to launch, 5 by default
    `./spg ... -r 10 ...`