## Empty boxes

In this step you will add another gift box, but this one will be empty! It will also move around in random directions.

--- task ---

Add a second **Gift** sprite. This one will automatically be named **Gift2**

![images showing two gift sprites side by side](images/two-gifts.png)

Don't forget to increase it's size to **150%**

--- /task ---

--- task ---

The **Gift2** sprite should start in the centre of the screen.

![image of gift2 sprite](images/gift2-sprite.png)

```blocks3
when green flag clicked
go to x: (0) y: (0)
```

--- /task ---

--- task ---

When this sprite `receives move`{:class="block3events"} it should also move in random directions.

![image of gift2 sprite](images/gift2-sprite.png)

```blocks3
when I receive [move v]
repeat (10)
glide (1) secs to [random position v]
```

--- /task ---

--- task ---

Click the green flag to watch the two sprites move around the screen.

--- no-print ---

![animated gif of the two gift boxes moving randomly around the screen](images/random-motion-2.gif)

--- /no-print ---

--- /task ---

The boxes should always move at the same speed as each other. At the moment they are set to `glide 1 secs`{:class="block3motion"}. To easily change the speed of both boxes, a `variable`{:class="block3variables"} can be used.

--- task ---

Create a new variable called `speed`{:class="block3variables"}, and add it to the `glide 1 secs to random position`{:class="block3motion"} block and add to both the **Gift** and **Gift2** sprites.

![image of gift sprite](images/gift-gift2-sprite.png)

```blocks3
when I receive [move v]
repeat (10)
+ glide (speed) secs to [random position v]
```

--- /task ---

--- task ---

On the first gift sprite, you can add code to set the speed variable. Choose any value you like.

![image of the gift sprite](images/gift-sprite.png)

```blocks3
when flag clicked
+ set [speed v] to (1)
go to x: (150) y: (0)
switch costume to [gift-a v]
wait (1) seconds
switch costume to [Crystal-a v]
wait (2) seconds
switch costume to [gift-a v]
wait (1) seconds
broadcast [move v] and wait
``` 

--- /task ---

--- task ---

Experiment with different speeds, until you find a value you like.

--- /task ---

--- save ---




