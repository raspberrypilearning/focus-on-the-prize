## ಖಾಲಿ ಪೆಟ್ಟಿಗೆಯನ್ನು ರಚಿಸಿ

ಈ ಹಂತದಲ್ಲಿ, ನೀವು ಇನ್ನೊಂದು ಉಡುಗೊರೆ ಪೆಟ್ಟಿಗೆಯನ್ನು ಸೇರಿಸುತ್ತೀರಿ, ಆದರೆ ಇದು ಖಾಲಿಯಾಗಿರುತ್ತದೆ! ಇದೂ ಸಹ ಯಾದೃಚ್ಛಿಕ ದಿಕ್ಕುಗಳಲ್ಲಿ ಚಲಿಸುತ್ತದೆ.

--- task ---

ಎರಡನೆಯ **Gift** ಸ್ಪ್ರೈಟ್‌ ಸೇರಿಸಿ. ಇದನ್ನು ಸ್ಯಂಚಾಲಿತವಾಗಿ **Gift2** ಎಂದು ಹೆಸರಿಸಲಾಗುತ್ತದೆ.

![ಎರಡು ಉಡುಗೊರೆ ಸ್ಪ್ರೈಟ್‌ಗಳನ್ನು ಅಕ್ಕಪಕ್ಕದಲ್ಲಿ ತೋರಿಸುವ ಚಿತ್ರಗಳು](images/two-gifts.png)

ಗಾತ್ರವನ್ನು (ಶೆಕಡಾ) `150`ಕ್ಕೆ ಹೆಚ್ಚಿಸಲು ಮರೆಯಬೇಡಿ.

--- /task ---

--- task ---

**Gift2** ಸ್ಪ್ರೈಟ್‌ ವೇದಿಕೆಯ ಮಧ್ಯದಲ್ಲಿ ಪ್ರಾರಂಭಿಸುವಂತೆ ಹೊಂದಿಸಿ.

![ಉಡುಗೊರೆ2 ಸ್ಪ್ರೈಟ್‌ ಚಿತ್ರ](images/gift2-sprite.png)

```blocks3
when green flag clicked
go to x: (0) y: (0)
```

--- /task ---

--- task ---

ಈ ಸ್ಪ್ರೈಟ್‌ `receives move`{:class="block3events"}ದಾಗ, ಅದು ಯಾದೃಚ್ಛಿಕ ದಿಕ್ಕುಗಳಲ್ಲಿ `glide`{:class="block3motion"} ಮಾಡುವಂತೆ ಬ್ಲಾಕ್‌ಗಳನ್ನು ಸೇರಿಸಿ.

![ಉಡುಗೊರೆ2 ಸ್ಪ್ರೈಟ್‌ ಚಿತ್ರ](images/gift2-sprite.png)

```blocks3
when I receive [move v]
repeat (10)
glide (1) secs to [random position v]
```

--- /task ---

--- task ---

ಹಸಿರು ಬಾವುಟದ ಮೇಲೆ ಕ್ಲಿಕ್ ಮಾಡಿ ಮತ್ತು ಎರಡು ಸ್ಪ್ರೈಟ್‌ಗಳು Stage ಸುತ್ತಲೂ ಚಲಿಸುವುದನ್ನು ವೀಕ್ಷಿಸಿ.

--- no-print ---

![ಪರದೆಯ ಸುತ್ತಲೂ ಎರಡು ಉಡುಗೊರೆ ಪೆಟ್ಟಿಗೆಗಳು ಯಾದೃಚ್ಛಿಕವಾಗಿ ಚಲಿಸುತ್ತಿರುವುರ ಅನಿಮೇಟೆಡ್ ಜಿಐಎಫ್](images/random-motion-2.gif)

--- /no-print ---

--- /task ---

ಪೆಟ್ಟಿಗೆಗಳು ಯಾವಾಗಲೂ ಪರಸ್ಪರ ಒಂದೇ ವೇಗದಲ್ಲಿ ಚಲಿಸಬೇಕು. ಈ ಸಮಯದಲ್ಲಿ, ಅವುಗಳನ್ನು `glide 1 secs`{:class="block3motion"}ಗೆ ಹೊಂದಿಸಲಾಗಿದೆ. ಪೆಟ್ಟಿಗೆಗಳ ವೇಗವನ್ನು ಸುಲಭವಾಗಿ ಬದಲಾಯಿಸಲು, ನೀವು `variable`{:class="block3variables"} ಉಪಯೋಗಿಸಬಹುದು.

--- task ---

`speed` ಎನ್ನುವ ಹೊಸ `variable`{:class="block3variables"} ರಚಿಸಿ ಮತ್ತು ಅದನ್ನು `glide 1 secs to random position`{:class="block3motion"} ಬ್ಲಾಕ್‌ಗೆ ಸೇರಿಸಿ. ಈ ಬ್ಲಾಕ್‌ನ್ನು **Gift** ಮತ್ತು **Gift2** ಎರಡೂ ಸ್ಪ್ರೈಟ್‌ಗಳಿಗೆ ಸೇರಿಸಿ.

![ಉಡುಗೊರೆ ಸ್ಪ್ರೈಟ್‌ ಚಿತ್ರ](images/gift-gift2-sprite.png)

```blocks3
when I receive [move v]
repeat (10)
+ glide (speed) secs to [random position v]
```

--- /task ---

--- task ---

**Gift** ಸ್ಪ್ರೈಟ್‌ನ ಕೋಡ್‌ನಲ್ಲಿ, ನೀವು `set`{:class="block3variables"} ಕೋಡ್‌ನ್ನು `speed`{:class="block3variables"} ವೇರಿಯೇಬಲ್‌ಗೆ ಸೇರಿಸಬಹುದು. ನೀವು ಇಷ್ಟಪಡುವ ಯಾವುದೇ ಮೌಲ್ಯವನ್ನು ಆಯ್ದುಕೊಳ್ಳಿ.

![ಉಡುಗೊರೆ ಸ್ಪ್ರೈಟ್ ಚಿತ್ರ](images/gift-sprite.png)

```blocks3
when flag clicked
+ set [speed v] to (1)
go to x: (-150) y: (0)
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

ನಿಮಗೆ ಇಷ್ಟವಾಗುವ ವೇಗ ಸಿಗುವವರೆಗೂ, ಬೇರೆ ಬೇರೆ ಮೌಲ್ಯಗಳೊಂದಿಗೆ ಪ್ರಯೋಗ ಮಾಡಿ.

--- /task ---

--- save ---




