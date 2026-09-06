sh scripts i made to make my life easier

## dark-add

a script that adds/removes urls from my DarkReader.json pywal16 template disabledFor section (derived from https://github.com/eylles/pywal-extra/blob/master/templates/darkreader/darkreader.json), because adding them manually is a huge pain

### usage:

the first argument is a mode, and the following arguments should be urls.

#### modes:

a - adds urls

d - deletes urls

`dark-add a 'google.com'`

## crop-img

a script that crops an image into a perfect square, because i needed that functionality for my next script....

### usage:

the first argument is the name of an image file, and the second argument is the name of the expected output. the third argument optionally allows you to specify the -gravity of the imagemagick cropping (https://imagemagick.org/command-line-options/#gravity) (Center by default)

`crop-img 'in.png' 'out.png' East`

## mus-img

my mp3 player requires my mp3's album art to be a perfectly square jpg. this script does that for me :)

### usage

the first argument is an image file for the album art (set it to `-` if you want to use album art embedded in the audio/video file), and the second argument is the audio/video file. the output will be an mp3 file regardless of the input.

`mus-img - 'song.mp3'`

`mus-img 'art.png' 'song.mp3'`
