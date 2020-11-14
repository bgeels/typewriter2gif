# typewriter2gif
Small script that generates a gif of text that appears as though it's being typed.

## Dependencies
You must have Pillow installed to use this utility.
```
sudo pip3 install Pillow
```

## Examples

#### 1.) 
```
./typewriter2gif --s 'Hello World!' -c '#888000' -b '#333000' -fs 80 -h 50 -w 435
```

![foo](examples/1.gif)

#### 2.) 
```
./typewriter2gif --s 'Loop Forever!' -c '#000888' -b '#000222' -fs 65 -h 60 -w 435 -l 0 -va top
```

![foo](examples/2.gif)

#### 3.) 
```
./typewriter2gif --s 'Twice from the bottom right now!' -c '#008880' -b '#004440' -fs 25 -h 50 -w 430 -va bottom -ha right -l 1 -d 100
```

![foo](examples/3.gif)
