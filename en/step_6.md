## More gifts

In this step you will make sure the gifts are not touching each other, or the edge of the screen when they stop moving, and then add a third gift.

It is possible that the gift boxes will finish their motion on top of each other, which might make it difficult to see which gift is which. To stop this from happening, you can detect if they are touching. The colour of the gift's ribbon, can be used to detect if two boxes are touching each other. 

**The scripts shown below need to be added to both Gift and Gift2**

--- task ---
The `not`{:class="block3operators"} operator can be used to turn a **True** into a **False**, or a **False into a **True**.

A `sensing`{:class="block3sensing"} block that detects if a sprite is touching a colour, would return **True**, when the sprite touches that colour.

By using the `not`{:class="block3operators"} operator, you can detect if a sprite is `not`{:class="block3operators"} `touching`{:class="block3sensing"} a color.

Add a `repeat until`{:class="block3control"} block to the bottom of your script, and place a `not`{:class="block3operators"} block inside it.


![image of gift sprite](images/gift-sprite.png)
![image of gift2 sprite](images/gift2-sprite.png)

```blocks3
when I receive [move v]
repeat (10)
glide (speed) secs to [random position v]
+ repeat until <not <>>
```

--- /task ---

--- task ---

Add in a `touching color`{:class="block3sensing"} block, and use the color picker to select the color of the ribbon.

--- no-print ---

![animated gif showing the colour picker being used to select the colour of the gift ribbon](images/color-picker.gif)

--- /no-print ---

![image of gift sprite](images/gift-sprite.png)
![image of gift2 sprite](images/gift2-sprite.png)

```blocks3
when I receive [move v]
repeat (10)
glide (speed) secs to [random position v]
end
+ repeat until <not <touching color (#F9C780)>>
```

--- /task ---

--- task ---

Within the `repeat until`{:class="block3control"} block, add in another block to keep the box moving to a random position.

![image of gift sprite](images/gift-sprite.png)
![image of gift2 sprite](images/gift2-sprite.png)

```blocks3
when I receive [move v]
repeat (10)
glide (speed) secs to [random position v]
end
repeat until <not <touching color (#F9C780) ?>>
+ glide (speed) secs to [random position v]
```

--- /task ---

--- task ---

Click the green flag a few times to make sure that the boxes always move to an empty area of the stage, before they stop moving.

--- /task ---

It would also be nice, if the boxes didn't stop when they are off the edge of the stage. An `and`{:class="block3operators"} operator can be used to test for two different conditions.

--- task ---

Add in a `and`{:class="block3operators"} into the `repeat until`{:class="block3control"} condition. Then add in a `touching edge`{:class="block3sensing"} block to go with the `not`{:class="block3operators"} `touching color`{:class="block3sensing"} blocks.

![image of gift sprite](images/gift-sprite.png)
![image of gift2 sprite](images/gift2-sprite.png)

```blocks3
when I receive [move v]
repeat (10)
glide (speed) secs to [random position v]
end
+ repeat until < <not <touching color (#F9C780) ?>> and <not <touching [edge v] ?>>
glide (speed) secs to [random position v]
```

--- /task ---

--- task ---

Test your code again, to make sure that the boxes now do not stop at the edge of the stage.

--- /task ---

Now that the code for *Gift* and *Gift2* are complete, you can duplicate *Gift2* to add a third box to the game.

--- task ---
Right click on *Gift2* and select **duplicate** from the drop down menu.

![image showing drop down menu with duplicate selected](images/duplicate-sprite.png)

--- /task ---

--- task ---

All the code has been duplicated as well, but *Gift3* needs a different starting position.

![image of gift3 sprite](images/gift3-sprite.png)

```blocks3
when flag clicked
+ go to x: (150) y: (0)
show
```
--- /task ---

--- task ---

Test you game again, clicking the green flag.

--- /task ---

--- save ---
