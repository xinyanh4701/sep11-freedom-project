# Entry 2
##### 12/18/22

After writing the [1st entry](entry01.md), learning the tool is the next step.
For the first few weeks, I played more on the [kaboom js playground](https://kaboomjs.com/play?demo=add) which is a sandbox where you can tinker with the tool. Afterwards, I searched up on Google for [kaboom js](https://kaboomjs.com/) tutorials and I found a [video on YouTube](https://www.youtube.com/watch?v=4OaHB0JbJDI) that helped me learn more about the tool.

I created a kaboom template (it is the first one that pops up) on [replit](https://replit.com/~) (this was part of the tutorial). On the left side of the page where it says `Kaboom`, I looked down to see `Learn` and I learned my tool from there.

Some of the concepts I learned:
* game object - a character in the game
* `add()` - a function that adds all of the components you want in a character
* `area()` - gives a character an area like how we give a rectangle an area of 50 in.
* `body()` - gives the object physical world characteristics
* `onKeyPress()` - runs code when a certain key is played
* `pos()` - object's position on the display
* `color()` - inside the parenthesis, you input 3 values: `r(red), g(green), b(blue` ranging from 0 - 255
* `solid()` - makes the object not invisible meaning another object can't go through it

As I followed along the tutorial, I tinkered with the code they gave me to start with.

<!-- ![kaboom-sandbox-1](img/kaboom-sandbox-1.png) -->
<img src="img/kaboom-sandbox-1.png" width="300">

*The original code*
```js
// add platform
add([
	rect(width(), 48),
	pos(0, height() - 48),
	outline(4),
	area(),
	solid(),
	color(127, 200, 255),
])
```
<!-- ![kaboom-sandbox-2](img/kaboom-sandbox-2.png) -->
<img src=">

*My tinkered version*
```js
add([
	rect(width(), 48),
	pos(0, height() - 100),
	outline(10),
	area(),
	solid(),
	color(255, 200, 255),
])
```
The platform ended up not touching the bottom of the screen and actually stay off the bottom of the screen. That made me wonder, so I went back to the markdown (where I learned some Kaboom) to find the reason why.

Here is what I found:

* `rect()` renders a triangle. It accepts 2 arguments, the width and height, which we give it the game width (returned by width()) and height of 48 pixels
* `pos()` position. We give it a x: 0 and y: height() - 48 so it sits right on the bottom of the screen

The original platform has a height of `48px` and I only changed `48` from `pos(0, height() - 48)` to `pos(0, height() - 100)`. The `height()` in `(0, height() - 48)` is 48 because the `rect()` function had 48 at the end of the parameter which defines `height()`. The position of the bottom of the screen is (0 , 0). To cancel out `height()`, you need to type down the height value from the `rect()` function in this case for the platform to touch the bottom of the screem. However, I am still not really sure why the platform is off the bottom of the screen but, at least I know how to make an object touch the bottom of the screen.

I am currently in stages 3 and 4 of the **Engineering Design Process (EDP)** which is to *brainstorm possible solutions* and *plan the most promising solution*. These steps are not really related to what I am doing which is learning the tool. However, learning my tool will definitely help me brainstorm possible solutions and plan the most promising solution. The next step in the **EDP** is to *create a prototype* meaning I am going to build my game which is going to happen in a later time.

I am improving on the skills of *how to learn* and *time management*. Since right now I am learning my tool, I am going have to learn by myself. I have to search tutorials and documentations that will help me understand the game engine. Learning on your own (LOYO) takes time and I need to learn my tool somehow. It made me want to manage my time more efficiently. I started to learn my tool when I have free time.

My goal for the winter break is to find more tutorials to learn and build a miniproject along the way. Every day, I am going to dedicate myself of at least 1 hour and a half to learn and build. To make myself accountable, I will set up a calendar that will alarm me to the do the work. I will use the stopwatch instead of a timer to keep track of the time because I tend to keep looking at the phone when I use the timer.

[Previous](entry01.md) | [Next](entry03.md)

[Home](../README.md)