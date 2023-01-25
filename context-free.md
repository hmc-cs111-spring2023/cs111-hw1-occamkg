# Context Free

##  Who is this programming language for?

This language appears to be for people who want to create graphics programmatically (with repeated, recursive, random, etc. structures).

## What is easy to do in this language? Why is it easy?

It is easy to make basic shapes because the components are built in (lines, curves, circles, triangles, squares, etc.). A large advantage of this program is that it can iteratively create shapes which makes patterns easier. It can also recursively create shapes which makes complex structures like fractals relatively straightforward to draw (although it does need a minimum resolution, so I guess it's not quite a fractal).

## What is hard to do in this language? Why is it hard?

It is difficult to draw realistic images (e.g. a face) since every part of every shape needs to be defined. Unlike in traditional drawing programs or on paper, in this program, you need to know the coordinates of everything.

## How did you learn how to program in this language?

I read through parts of the ContextFree [wiki](https://github.com/MtnViewJohn/context-free/wiki).

## What is the underlying _computational model_ for this programming language? 

The program gives rules for graphics to be drawn on a 2D canvas. The program creates these graphics in the order they are defined and overlays them. A single graphic can be broken into smaller components that can be more manageable to conceptualize and understand in the code.

## What do you think is interesting about the ContextFree program you wrote?

It was interesting to draw triangles where each corner coordinate of the triangle varies throughout a loop. I also liked how easy it was to change the hue in a loop.