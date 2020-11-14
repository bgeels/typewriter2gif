# typewriter2gif
Small script that generates a gif of text that appears as though it's being typed.

## Dependencies
You must have Pillow installed to use this utility.
```
sudo pip3 install Pillow
```
## Options
```
./typewriter2gif --help
usage: typewriter2gif [--help] [-s STRING] [-fs FONT_SIZE] [-n NAME] [-d DURATION] [-w WIDTH] [-h HEIGHT]
                      [-va {top,middle,bottom}] [-ha {left,middle,right}] [-x X_OFFSET] [-y Y_OFFSET] [-c COLOR]
                      [-b BACKGROUND_COLOR] [-l LOOP]

Generates a .gif of text as if it is being typed

optional arguments:
  --help                Print the help message
  -s STRING, --string STRING
                        The string to type out in the image
  -fs FONT_SIZE, --font_size FONT_SIZE
                        The size of the font used
  -n NAME, --name NAME  The name of the output file
  -d DURATION, --duration DURATION
                        The duration of the gif
  -w WIDTH, --width WIDTH
                        The width of the image
  -h HEIGHT, --height HEIGHT
                        The height of the image
  -va {top,middle,bottom}, --vertical_align {top,middle,bottom}
                        How to vertically align the text
  -ha {left,middle,right}, --horizontal_align {left,middle,right}
                        How to horizontally align the text
  -x X_OFFSET, --x_offset X_OFFSET
                        Offsets the horizontal position of the text
  -y Y_OFFSET, --y_offset Y_OFFSET
                        Offsets the vertical position of the text
  -c COLOR, --color COLOR
                        The text color
  -b BACKGROUND_COLOR, --background_color BACKGROUND_COLOR
                        The background color
  -l LOOP, --loop LOOP  The number of times to loop. ( 0 is loop forever; omit this to not loop at all )
```

## Examples

#### Example 1
```
./typewriter2gif --s 'Hello World!' -c '#888000' -b '#333000' -fs 80 -h 50 -w 435
```

![foo](examples/1.gif)

#### Example 2 
```
./typewriter2gif --s 'Loop Forever!' -c '#000888' -b '#000222' -fs 65 -h 60 -w 435 -l 0 -va top
```

![foo](examples/2.gif)

#### Example 3
```
./typewriter2gif --s 'Twice from the bottom right now!' -c '#008880' -b '#004440' -fs 25 -h 50 -w 430 -va bottom -ha right -l 1 -d 100
```

![foo](examples/3.gif)
