## Did you get it right?

In this step, you will add code so that the player can click on a gift box, to see if it has the crystal inside.

--- task ---

On the **Gift** sprite, add code so that `when this sprite clicked`{:class="block3events"}, it `says yes`{:class="block3looks"} and `switches costume`{:class="block3looks"} to the crystal.

![image of gift sprite](images/gift-sprite.png)

```blocks3
when this sprite clicked
say [Yes!]
switch costume to [Crystal-a]
```

--- /task ---

--- task ---

The **Gift2** sprite should `say No!`{:class="block3looks"} and then `hide`{:class="block3looks"}

![image of gift2 sprite](images/gift2-sprite.png)

```blocks3
when this sprite clicked
say [No!] for (1) seconds
hide
```

--- /task ---

--- task ---

As the sprite can now be hidden, a `show`{:class="block3looks"} block is needed when the program starts, to make sure it is visible.

![image of gift2 sprite](images/gift2-sprite.png)

```blocks3
when green flag clicked
go to x: (0) y: (0)
+ show
```

--- /task ---



--- task ---

Click the green flag to run your code, and test what happens when you click on the boxes.

--- /task ---

You may notice, that you can actually click on the boxes while they are moving around. You can use a `variable`{:class="block3variables"} to stop players cheating like this.

--- no-print ---

![animated gif showing the gifts being clicked on before they have finished moving](images/cheat.gif)_

--- /no-print ---

--- task ---

Create a new variable called `finished`{:class="block3variables"}. This can be set to `false`{:class="block3variables"} when the gifts start moving, and then `true`{:class="block3variables"} when the gifts stop moving.

![image of the gift sprite](images/gift-sprite.png)

```blocks3
when flag clicked
set [speed v] to (1)
+ set [finished v] to [false]
go to x: (150) y: (0)
switch costume to [gift-a v]
wait (1) seconds
switch costume to [Crystal-a v]
wait (2) seconds
switch costume to [gift-a v]
wait (1) seconds
broadcast [move v] and wait
+ set [finished v] to [true]
``` 

--- /task ---

--- task ---

Now an `if`{:class="block3control"} block can be used to test if `finished`{:class="block3variables"} is `true`{:class="block3variables"} or `false`{:class="block3variables"}. The clicking should only be allowed, if `finished = true`{:class="block3operators"}.

![image of gift sprite](images/gift-sprite.png)

```blocks3
when this sprite clicked
+ if <(finished) = [true]> then
say [Yes!]
switch costume to [Crystal-a]
```

--- /task ---

--- task ---

Add the same `if`{:class="block3control"} condition to the **Gift2** sprite.

![image of gift2 sprite](images/gift2-sprite.png)

```blocks3
when this sprite clicked
+ if <(finished) = [true]> then
say [No!] for (1) seconds
hide
```

--- /task ---

--- task ---

Test your program, and you should see that the sprites can only be clicked on when they finish moving around.

--- /task ---

--- save ---
	




