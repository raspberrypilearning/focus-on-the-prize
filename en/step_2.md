## Add a gift in a box

In this step, you will add a gift box that will briefly show what is hidden inside it.

--- task ---

Open a new Scratch project.

**Online:** open a new online Scratch project at [rpf.io/scratch-new](http://rpf.io/scratch-new){:target="_blank"}.

**Offline:** open a new project in the Scratch offline editor. If you need to, you can [download and install Scratch here](http://rpf.io/scratchoff){:target="_blank"}.

--- /task ---

--- task ---

Delete the **Scratch cat** sprite. To do this, click on the **Rubbish bin** icon in the corner of the image in the Sprite list.

![image showing Scratch cat icon, with trashcan in the top right hand corner](images/delete-cat.png)

--- /task ---

--- task ---

Click on **Choose a Sprite** to search for a new sprite to add to your game.

![image showing the choose sprite icon with expanded options](images/choose-sprite.png)

--- /task ---

--- task ---

Search for the **Gift** sprite, then add it to your game.

![image showing the search bar with "gift" typed in and the gift sprite below it](images/add-gift.png)

--- /task ---

--- task ---

The sprite is a little small at the moment. To increase the sprite's size, you can either use the `set size to`{:class="block3looks"} block, as you may have done in other projects, or you can change the sprite's **properties**.

Set the sprite's size to `150` (percent).

![image showing properties for the sprite with the size set to 150 percent](images/set-size.png)

--- /task ---

--- task ---

Go to the **Costumes** tab to look at the costumes for the **Gift** sprite. You will see two costumes called **gift-a** and **gift-b**.

![image showing the costumes tab for the gift sprite, along with the two default costumes](images/gift-costumes.png)

Click on the **Choose a Costume** icon to add a new costume to the sprite.

![image showing the expanded choose a costume icon](images/choose-costume.png)

--- /task ---

--- task ---

Choose the gift that you would like to put inside the gift box. In this example, we will use the **Crystal-a** costume.

![image showing the search for a crystal costume, with Crystal-a and Crystal-b shown](images/choose-crystal-costume.png)

--- /task ---

--- task ---

Switch back to the **Code** tab so that you can begin to work on the program.

![image showing code tab selected](images/code-tab.png)

Add some blocks to make the starting costume for the **Gift** sprite `switch`{:class="block3looks"} to `Crystal-a`{:class="block3looks"} and then back to `gift-a`{:class="block3looks"} again. Use `wait`{:class="block3control"} blocks in between the costume changes.

The `wait`{:class="block3control"} blocks give the player a chance to see the costume changes.

![image of the gift sprite](images/gift-sprite.png)

```blocks3
when flag clicked
switch costume to [gift-a v]
wait (1) seconds
switch costume to [Crystal-a v]
wait (2) seconds
switch costume to [gift-a v]
``` 

--- /task ---

--- task ---

Click on the green flag, and make sure that your gift box changes costumes.

--- /task ---

--- save ---
