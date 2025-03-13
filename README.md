# Bingo

A program for running a basic custom Bingo-game and creating printable sheets that can be printed out for participants to use.

## Installation

Install dependencies

    pip install -r requirements.txt

For the font size to work, you need to have some font file in the "fonts/" folder. The font must be a .ttf-file.

## How to use

Insert correct parameters to `main.py`:
* `count` = desired amount of bingo sheets
* `midImg` = path to the desired middle image in `img/` directory (see example.jpg for reference)
* `font` = path to the desired font in `fonts/` directory

If you want to use the program to run an actual Bingo, you can use the draw()-method to get the values out of the machine one by one:
~~~
while b.nonEmpty():
    out = b.draw()
    print(out)
~~~

## Bingo sheet example

![PDF image](img/example.jpg)
