# tubeturbo
Download and convert video of youtube

## Version
__Test version__

## Licence
Creative Commons Attribution 4.0
http://www.safecreative.org/work/1707102922177-tubeturbo

## Requirements
* ffmpeg https://ffmpeg.org/
Save to same folder or path `?:Windows\System32\`

### Arguments

* --url | -u `string` url of youtube
* --format | -f `string` format to output
  * formats video available: `mp4` `flv` `webm` `3gp` `mov`
  * formats audio available: `acc` `mp2` `mp3`
  * --initial | -i `int` in seconds To select the start of the video
* --gif | -g Indicates whether it is converted to gif
  * --gif-initial | -gi `int` in seconds default `0`
  * --gif-duration | -gd `int` in secons default `3`
* --change | -c `string` change output file name, Use quotation marks

### Examples

Convert file in mp3 format

`tubeturbo --url https://www.youtube.com/watch?v=... --format mp3`

Create a gif file

`tubeturbo --url https://www.youtube.com/watch?v=... --gif --gif-initial 5 --gif-duration 3`


Change file name output

`tubeturbo --url https://www.youtube.com/watch?v=... --format mp3 --change "mi file name"`
