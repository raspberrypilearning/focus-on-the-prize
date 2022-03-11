## ಇನ್ನಷ್ಟು ಉಡುಗೊರೆಗಳನ್ನು ಸೇರಿಸಿ

ಈ ಹಂತದಲ್ಲಿ, ಉಡುಗೊರೆಗಳು ಚಲಿಸುವುದನ್ನು ನಿಲ್ಲಿಸಿದಾಗ ಅವು ಪರಸ್ಪರ ಸ್ಪರ್ಶಿಸುವುದಿಲ್ಲ ಅಥವಾ ಪರದೆಯ ಅಂಚನ್ನು ಸ್ಪರ್ಶಿಸುವುದಿಲ್ಲ ಎಂದು ನೀವು ಖಚಿತಪಡಿಸಿಕೊಳ್ಳುತ್ತೀರಿ. ನಂತರ, ನೀವು ಮೂರನೆಯ ಉಡುಗೊರೆಯನ್ನು ಸೇರಿಸುತ್ತೀರಿ.

ಉಡುಗೊರೆ ಪೆಟ್ಟಿಗೆಗಳು ಒಂದರ ಮೇಲೊಂದರಂತೆ ನಿಲ್ಲುವ ಸಾಧ್ಯತೆಯಿದೆ, ಇದರಿಂದ ಯಾವ ಉಡುಗೊರೆ ಪೆಟ್ಟಿಗೆ ಯಾವುದು ಎಂದು ನೋಡಲು ಕಷ್ಟವಾಗಬಹುದು. ಇದು ಆಗದಂತೆ ಮಾಡಲು, ಅವುಗಳು ಸ್ಪರ್ಶಿಸುತ್ತಿವೆಯೇ ಎಂದು ನೀವು ಪತ್ತೆ ಮಾಡಬಹುದು. ಎರಡು ಪೆಟ್ಟಿಗೆಗಳು ಪರಸ್ಪರ ಸ್ಪರ್ಶಿಸುತ್ತಿವೆಯೇ ಎಂದು ಪತ್ತೆ ಮಾಡಲು ಉಡುಗೊರೆ ಪೆಟ್ಟಿಗೆಯ ರಿಬ್ಬನ್‌ ಬಣ್ಣವನ್ನು ಉಪಯೋಗಿಸಬಹುದು.

ನೀವು ಈ ಕೆಳಗೆ ತೋರಿಸಿರುವ ಬರಹಗಳನ್ನು **Gift** ಮತ್ತು **Gift2** **ಎರಡೂ** ಸ್ಪ್ರೈಟ್‌ಗಳಿಗೂ ಸೇರಿಸಬೇಕು.

--- task ---

ನೀವು `not`{:class="block3operators"} ಆಪರೇಟರ್‌ನ್ನು **ಸರಿ** ಯನ್ನು **ತಪ್ಪು**, ಅಥವಾ **ತಪ್ಪು** ಅನ್ನು **ಸರಿ** ಆಗಿ ಪರಿವರ್ತಿಸಲು ಉಪಯೋಗಿಸಬಹುದು.

`repeat until`{:class="block3control"} ಬ್ಲಾಕ್‌ನ್ನು ನಿಮ್ಮ ಬರಹದ ಕೆಳಗೆ ಸೇರಿಸಿ ಮತ್ತು ಅದರೊಳಗೆ `not`{:class="block3operators"} ಬ್ಲಾಕ್‌ ಇರಿಸಿ.

![ಉಡುಗೊರೆ ಸ್ಪ್ರೈಟ್‌ ಚಿತ್ರ](images/gift-gift2-sprite.png)


```blocks3
when I receive [move v]
repeat (10)
    glide (speed) secs to [random position v]
end
+ repeat until <not <>>
```

--- /task ---

--- task ---

`Sensing`{:class="block3sensing"} ಸ್ಪ್ರೈಟ್‌ ಒಂದು ನಿರ್ದಿಷ್ಟ ಬಣ್ಣವನ್ನು ಸ್ಪರ್ಶಿಸುತ್ತಿದೆಯೇ ಎಂದು ಪತ್ತೆ ಮಾಡುವ ಬ್ಲಾಕ್‌, ಸ್ಪ್ರೈಟ್‌ ಆ ಬಣ್ಣವನ್ನು ಸ್ಪರ್ಶಿಸಿದಾಗ **ಸರಿ** ಮರಳಿಸುತ್ತದೆ.

ನೀವು `not`{:class="block3operators"} ಆಪರೇಟರ್‌ನ್ನು ಸ್ಪ್ರೈಟ್‌ ನಿರ್ದಿಷ್ಟ ಬಣ್ಣವನ್ನು ಸ್ಪರ್ಶಿಸುತ್ತಿದೆಯೇ ಎಂದು ಪತ್ತೆ ಮಾಡಲು `not`{:class="block3operators"} `touching`{:class="block3sensing"} ಉಪಯೋಗಿಸಬಹುದು.

`touching color`{:class="block3sensing"}ಬ್ಲಾಕ್‌ನ್ನು ಸೇರಿಸಿ, ಮತ್ತು **Colour picker** ಟೂಲ್‌ನ್ನು ರಿಬ್ಬನ್‌ ಬಣ್ಣವನ್ನು ಆಯ್ಕೆ ಮಾಡಿಕೊಳ್ಳಲು ಉಪಯೋಗಿಸಿ.

--- no-print ---

![ಉಡುಗೊರೆಯ ರಿಬ್ಬನ್‌ ಬಣ್ಣವನ್ನು ಆಯ್ಕೆ ಮಾಡಲು ಕಲರ್‌ ಪಿಕ್ಕರ್ ಉಪಯೋಗಿಸುತ್ತಿರುವುದನ್ನು ತೋರಿಸುತ್ತಿರುವ ಅನಿಮೇಟೆಡ್‌ ಚಿತ್ರ](images/color-picker.gif)

--- /no-print ---

![ಉಡುಗೊರೆ ಸ್ಪ್ರೈಟ್‌ ಚಿತ್ರ](images/gift-gift2-sprite.png)

```blocks3
when I receive [move v]
repeat (10)
glide (speed) secs to [random position v]
end
+ repeat until <not <touching color (#F9C780)>>
```

--- /task ---

--- task ---

`repeat until`{:class="block3control"} ಬ್ಲಾಕ್‌ ಒಳಗೆ, ಪೆಟ್ಟಿಗೆಯು ಯಾದೃಚ್ಛಿಕ ಸ್ಥಾನಕ್ಕೆ ಚಲಿಸುತ್ತಲೇ ಇರುವಂತೆ ಮಾಡಲು ಇನ್ನೊಂದು ಬ್ಲಾಕ್‌ನ್ನು ಸೇರಿಸಿ.

![ಉಡುಗೊರೆ ಸ್ಪ್ರೈಟ್‌ ಚಿತ್ರ](images/gift-gift2-sprite.png)

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

ಹಸಿರು ಬಾವುಟದ ಮೇಲೆ ಕೆಲವು ಬಾರಿ ಕ್ಲಿಕ್‌ ಮಾಡಿ, ಪೆಟ್ಟಿಗೆಗಳು ಚಲಿಸುವುದನ್ನು ನಿಲ್ಲಿಸುವ ಮೊಸಲು ಯಾವಾಗಲೂ ವೇದಿಕೆಯ ಮೇಲೆ ಖಾಲಿ ಪ್ರದೇಶಕ್ಕೆ ಅವುಗಳು ಚಲಿಸುತ್ತವೆ ಎಂಬುವುದನ್ನು ಖಚಿತಪಡಿಸಿಕೊಳ್ಳಿ.

--- /task ---

ಪೆಟ್ಟಿಗೆಗಳು ವೇದಿಕೆಯ ಅಂಚಿಗೆ ತಲುಪಿದಾಗ ನಿಲ್ಲದೇ ಇದ್ದರೆ ಚೆನ್ನಾಗಿರುತ್ತದೆ. ನೀವು ಎರಡು ಬೇರೆ ಬೇರೆ ಷರತ್ತುಗಳನ್ನು ಪರೀಕ್ಷೆ ಮಾಡಲು `and`{:class="block3operators"} ಆಪರೇಟರ್‌ ಉಪಯೋಗಿಸಬಹುದು.

--- task ---

`and`{:class="block3operators"} ಬ್ಲಾಕ್‌ನ್ನು `repeat until`{:class="block3control"} ಷರತ್ತಿನೊಳಗೆ ಸೇರಿಸಿ. ನಂತರ, `not`{:class="block3operators"} ಬ್ಲಾಕ್‌ ಮತ್ತು `touching edge`{:class="block3sensing"} ಬ್ಲಾಕ್‌ನ್ನು `not`{:class="block3operators"} `touching color`{:class="block3sensing"} ಬ್ಲಾಕ್‌ಗಳೊಂದಿಗೆ ಹೋಗಲು ಸೇರಿಸಿ.

![ಉಡುಗೊರೆ ಸ್ಪ್ರೈಟ್‌ ಚಿತ್ರ](images/gift-gift2-sprite.png)

```blocks3
when I receive [move v]
repeat (10)
glide (speed) secs to [random position v]
end
repeat until < <not <touching color (#F9C780) ?>> and <not <touching [edge v] ?>>::operator +
glide (speed) secs to [random position v]
```

--- /task ---

--- task ---

ಬಾಕ್ಸ್‌ಗಳು ಈಗ Stage ಅಂಚಿನಲ್ಲಿ ನಿಲ್ಲುವುದಿಲ್ಲ ಎಂದು ಖಚಿತಪಡಿಸಿಕೊಳ್ಳಲು ನಿಮ್ಮ ಕೋಡ್‌ನ್ನು ಮತ್ತೊಮ್ಮೆ ಪರೀಕ್ಷಿಸಿ.

--- /task ---

ಈಗ **Gift** ಮತ್ತು **Gift2** ಸ್ಪ್ರೈಟ್‌ಗಳ ಕೋಡ್‌ ಪೂರ್ಣವಾಗಿರುವುದರಿಂದ, ನೀವು ಆಟಕ್ನೆ ಮೂರನೆಯ ಪೆಟ್ಟಿಗೆಯನ್ನು ಸೇರಿಸಲು **Gift2** ಸ್ಪ್ರೈಟ್ ನಕಲು ಮಾಡಬಹುದು.

--- task ---

Sprite ಲಿಸ್ಟ್‌ನಲ್ಲಿ **Gift2** ಸ್ಪ್ರೈಟ್‌ ಮೇಲೆ ರೈಟ್‌-ಕ್ಲಿಕ್‌ ಮಾಡಿ ಮತ್ತು ಡ್ರಾಪ್-ಡೌನ್‌ ಮೆನುನಲ್ಲಿ **duplicate** ಆಯ್ಕೆ ಮಾಡಿ.

![ಡುಪ್ಲಿಕೇಟ್‌ ಆಯ್ಕೆಯೊಂದಿಗೆ ಡ್ರಾಪ್‌ ಡೌನ್‌ ಮೆನು ತೋರಿಸುತ್ತಿರುವ ಚಿತ್ರ](images/duplicate-sprite.png)

--- /task ---

--- task ---

ಎಲ್ಲಾ ಕೋಡ್‌ಗಳನ್ನೂ ನಕಲು ಮಾಡಲಾಗಿದೆ, ಆದರೆ ನೀವು **Gift3** ಸ್ಪ್ರೈಟ್‌ಗೆ ಬೇರೆ ಪ್ರಾರಂಭಿಕ ಸ್ಥಾನ ಕೊಡಬೇಕು.

![ಉಡುಗೊರೆ3 ಸ್ಪ್ರೈಟ್‌ ಚಿತ್ರ](images/gift3-sprite.png)

```blocks3
when flag clicked
+ go to x: (150) y: (0)
show
```
--- /task ---

--- task ---

ನಿಮ್ಮ ಆಟವನ್ನು ಮತ್ತೆ ಪರೀಕ್ಷೆ ಮಾಡಲು, ಹಸಿರು ಬಾವುಟದ ಮೇಲೆ ಕ್ಲಿಕ್‌ ಮಾಡಿ.

--- /task ---

--- save ---
