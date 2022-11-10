# Table of Contents
1. [General Info](#general-info)
2. [Videos](#videos)
3. [Technologies](#technologies)
4. [Installation](#installation)
5. [Run](#run)
6. [Collaboration](#collaboration)
7. [Repository overview](#repository-overview)
8. [License](#license)
### General Info
***
**Lab 5**

You will gain experience with threads and events in this lab.
You will create a rather easy game to accomplish this. 

***Task A***

Create a Micro:bit programme that responds to button click events by moving a pixel left and right across the display.
The button click event handlers must be registered.
Either update the pixel directly in the display handlers or have a display thread (fibre) and use the event handlers to modify the position. 

***Task B***

Add a thread to have a flashing pixel descend from the top of the display. You can randomly choose which column for it to descend using the int microbit_random(range) function. Make the flashing pixel reverse direction when it reaches the bottom and when it reaches the top both reverse direction and choose a new random column.

***Task C***

Place the controlled pixel in the bottom row from section A.
Verify that both pixels are in the same place when the flashing pixel from part B reaches the bottom row.
If they are, the flashing pixel should turn around and head back up.
If they aren't, the system may be reset and a suitable failure notice displayed.
Make sure that while the message is being displayed, the displayed pixels from parts A and B do not appear. 

***Task D - Advanced***

Add an extra feature or two. Examples are:

* Make the flashing pixel faster after each successful bounce. 
* Include a choice to launch the game with a different action, like a shake or two button presses. 
* Make the falling pixel occasionally move left and right and "bounce" off the sides to add more randomness. 

***Marks***

* This lab is worth 2% of the final grade.

***Outcomes***

Once this lab is compleate you should have gain experience with threads and events I have learned alot inregard to the 
C programming language and how multi-threaded tasks are handled accross multi-paged programs. However, due to personal family matters and a change of circumstances, I was unable to 
fix the remaining memory issues which I believed to have caused the results below.

### Videos
***
***Task A***


https://user-images.githubusercontent.com/109124700/201036063-aa3640ec-cc32-4f80-b079-1ab48413bcf8.mp4


* As you can see when you run the program, the leds blinks moves left/right depending on what button you push.

***Task C***


https://user-images.githubusercontent.com/109124700/201036090-983ab4be-a351-4dd6-8613-140e0bb5ca21.mp4


* As you can see when you run the program, the leds moves back up when it hits the bottom bar.

***Task D***


https://user-images.githubusercontent.com/109124700/201036106-1be04afa-ae01-4dcc-9410-f5d7884cb0e4.mp4


* As you can see when you run the program, the leds moves at a random speed and random location once it hits the top border.

## Technologies
***
A list of technologies used within the project:
* [gcc](https://gcc.gnu.org/): Version 9.4.0
* [nano](https://nano-editor.org/): Version 4.8

## Installation
***
A little intro about the installation. 
```
$ git clone https://github.com/lancaster-university/microbit-dal.git
```
## Run
***
**How to run**

To edit the code:
```
$ cd micro\:bit/
$ cd microbit-v2-samples/
$ source/
$ nano main.cpp
```
In a different termial, to compile the code:
```
$ cd micro\:bit/
$ cd microbit-v2-samples/
$ cd build
$ make
```
From this it will make a .hex file that you just need to drag onto the micro:bit which is located in:
```
$ cd micro\:bit/
$ cd microbit-v2-samples/
~"MICROBIT.hex"
```

## Collaboration
***
Just do what you want with this.
> Do what you want, whats done is done. 
## Repository overview
An overview of the directory structure and files:
```
.
├── README.md
├── src
│   ├── main.cpp
│   └── MICROBIT.hex
└── Vids
    ├── partA.mp4
    ├── partC.mp4
    └── partD.mp4

2 directories, 6 files


```
## License
MIT License

Copyright (c) 2022 Cameron Cox

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

https://github-readme-stats.vercel.app/api?username=coxxy12
