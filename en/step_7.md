## Add a distraction

To finish off the game you can add a distraction, to try and stop the player keeping their eyes' on the gift box.

--- task ---

Add a new sprite to your game. You can choose any sprite you like, but in this example the *Duck* sprite will be used.

![image of duck sprite](images/duck-sprite.png)

--- /task ---

When the game begins the duck should be hidden, and only start moving after the boxes start moving. It's also useful to bring the duck to the front layer, so it moves over the top of the boxes.

--- task ---

Add the following blocks to your sprite.

![image of duck sprite](images/duck-sprite.png)

```blocks3
when flag clicked
hide
go to [front v] layer
wait (4) seconds
```

--- /task ---

--- task ---

Next, the duck should wait a random number of seconds then move across the screen and hide itself. This can keep happening until the game has finished.

![image of duck sprite](images/duck-sprite.png)

```blocks3
when flag clicked
hide
go to [front v] layer
wait (4) seconds
+ repeat until <(finished) = (true)>
wait (pick random (1) to (5)) seconds
go to x: (-280) y: (-140)
show
glide (2) seconds to x: (280) y: (140)
hide
```
--- /task ---

--- task ---

Test your game and see if you can keep track of the gift box with a distracting duck flying across the screen.

--- /task ---

--- save ---

