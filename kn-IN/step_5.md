## ಉತ್ತರಗಳನ್ನು ಪ್ರಕಟಿಸಿ

ಈ ಹಂತದಲ್ಲಿ, ಉಡುಗೊರೆಯ ಪೆಟ್ಟಿಗೆಯಲ್ಲಿ ಹರಳು ಇದೆಯೇ ಎಂದು ನೋಡಲು ಆಟಗಾರ ಅದರ ಮೇಲೆ ಕ್ಲಿಕ್‌ ಮಾಡಬಹುದಾದ ಕೋಡ್‌ನ್ನು ನೀವು ಸೇರಿಸುತ್ತೀರಿ.

--- task ---

**Gift** ಸ್ಪ್ರೈಟ್‌ ಕೋಡ್‌ನಲ್ಲಿ, ಕೋಡ್‌ ಸೇರಿಸಿ ಇದರಿಂದ `when this sprite clicked`{:class="block3events"}, ಅದು `says`{:class="block3looks"} `Yes!` ಮತ್ತು ಹರಳಿಗೆ `switches costume to`{:class="block3looks"} ಸೇರಿಸಿ.

![ಉಡುಗೊರೆ ಸ್ಪ್ರೈಟ್‌ ಚಿತ್ರ](images/gift-sprite.png)

```blocks3
when this sprite clicked
say [Yes!]
switch costume to [Crystal-a v]
```

--- /task ---

--- task ---

**Gift2** ಸ್ಪ್ರೈಟ್‌ ಮೇಲೆ ಕ್ಲಿಕ್‌ ಮಾಡಿ ಮತ್ತು ಬ್ಲಾಕ್‌ಗಳನ್ನು ಸೇರಿಸಿ ಇದರಿಂದ ಅದು `says`{:class="block3looks"} `No!`. `say`{:class="block3looks"} ಬ್ಲಾಕ್ ಮೌಲ್ಯವನ್ನು `1` ಸೆಕೆಂಡ್‌ಗೆ ಬದಲಾಯಿಸಿ. `hide`{:class="block3looks"} ಬ್ಲಾಕ್‌ ಸೇರಿಸಿ ಆಗ ಸ್ಪ್ರೈಟ್‌ ಕಾಣೆಯಾಗುತ್ತದೆ.

![ಉಡುಗೊರೆ2 ಸ್ಪ್ರೈಟ್‌ ಚಿತ್ರ](images/gift2-sprite.png)

```blocks3
when this sprite clicked
say [No!] for (1) seconds
hide
```

--- /task ---

--- task ---

**Gift2** ಸ್ಪ್ರೈಟ್‌ನ್ನು ಈಗ ನಾವು ಮರೆಮಾಚಬಹುದಾದುರಿಂದ, ಪ್ರೋಗ್ರಾಮ್‌ ಪ್ರಾರಂಭವಾದಾಗ ಅದು ಕಾಣುತ್ತದೆ ಎಂದು ಖಚಿತಪಡಿಸಿಕೊಳ್ಳಲು ನೀವು `show`{:class="block3looks"} ಬ್ಲಾಕ್‌ ಸೇರಿಸಬೇಕು.

![ಉಡುಗೊರೆ2 ಸ್ಪ್ರೈಟ್‌ ಚಿತ್ರ](images/gift2-sprite.png)

```blocks3
when green flag clicked
go to x: (0) y: (0)
+ show
```

--- /task ---

--- task ---

ನಿಮ್ಮ ಕೋಡ್ ಅನ್ನು ರನ್ ಮಾಡಲು ಹಸಿರು ಬಾವುಟದ ಮೇಲೆ ಕ್ಲಿಕ್ ಮಾಡಿ ಮತ್ತು ನೀವು ಪೆಟ್ಟಿಗೆಗಳ ಮೇಲೆ ಕ್ಲಿಕ್ ಮಾಡಿದಾಗ ಏನಾಗುತ್ತದೆ ಎಂಬುದನ್ನು ಪರೀಕ್ಷಿಸಿ.

--- /task ---

ಪೆಟ್ಟಿಗೆಗಳು ಚಲಿಸುತ್ತಿರುವಾಗ ನೀವು ಅವುಗಳ ಮೇಲೆ ಕ್ಲಿಕ್‌ ಮಾಡಬಹುದು ಎಂಬುವುದನ್ನು ನೀವು ಗಮನಿಸಬಹುದು. ಆಟಗಾರರು ಈ ರೀತಿ ಮೋಸ ಮಾಡುವುದನ್ನು ನಿಲ್ಲಿಸಲು ನೀವು `variable`{:class="block3variables"} ಉಪಯೋಗಿಸಬಹುದು.

--- no-print ---

![ಉಡುಗೊರೆಗಳು ಚಲಿಸುವುದನ್ನು ನಿಲ್ಲಿಸುವ ಮೊದಲೇ ಅವುಗಳ ಮೇಲೆ ಕ್ಲಿಕ್‌ ಮಾಡುವುದನ್ನು ತೋರಿಸುವ ಅನಿಮೇಟೆಡ್‌ ಜಿಐಎಫ್](images/cheat.gif)_

--- /no-print ---

--- task ---

`finished` ಎನ್ನುವ ಹೊಸ `variable`{:class="block3variables"} ರಚಿಸಿ. `finished`{:class="block3variables"} ಉಡುಗೊರೆಯು ಚಲಿಸಲು ಪ್ರಾರಂಭಿಸಿದಾಗ ವೇರಿಯೇಬಲ್‌ `false` ಗೆ ಮತ್ತು ನಂತರ ಉಡುಗೊರೆಯು ಚಲಿಸುವುದನ್ನು ನಿಲ್ಲಿಸಿದಾಗ `true`ಗೆ `set`{:class="block3variables"} ಬ್ಲಾಕ್‌ಗಳನ್ನು ಸೇರಿಸಿ.

![ಉಡುಗೊರೆ ಸ್ಪ್ರೈಟ್ ಚಿತ್ರ](images/gift-sprite.png)

```blocks3
when flag clicked
set [speed v] to (1)
+ set [finished v] to [false]
go to x: (-150) y: (0)
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

ಈಗ, ನೀವು `finished`{:class="block3variables"} ಸರಿ ಅಥವಾ ತಪ್ಪು ಎಂದು ಪರಿಶೀಲಿಸಲು `if … then`{:class="block3control"} ಬ್ಲಾಕ್‌ನ್ನು ಉಪಯೋಗಿಸಬಹುದು. `Operators`{:class="block3operators"} ಬ್ಲಾಕ್‌ನ್ನು ಸೇರಿಸಿ, ಅದರಿಂದ `finished`{:class="block3variables"} `=`{:class="block3operators"} `true` ಆದರೆ ಮಾತ್ರ ಕ್ಲಿಕ್ ಮಾಡುವುದು ಯಾವುದಾದರು ಪರಿಣಾಮ ಬೀರುತ್ತದೆ.

![ಉಡುಗೊರೆ ಸ್ಪ್ರೈಟ್‌ ಚಿತ್ರ](images/gift-sprite.png)

```blocks3
when this sprite clicked
+ if <(finished) = [true]> then
say [Yes!]
switch costume to [Crystal-a]
```

--- /task ---

--- task ---

ಅದೇ `if`{:class="block3control"} ಷರತ್ತನ್ನು **Gift2** ಸ್ಪ್ರೈಟ್‌ಗೆ ಸೇರಿಸಿ.

![ಉಡುಗೊರೆ2 ಸ್ಪ್ರೈಟ್‌ ಚಿತ್ರ](images/gift2-sprite.png)

```blocks3
when this sprite clicked
+ if <(finished) = [true]> then
say [No!] for (1) seconds
hide
```

--- /task ---

--- task ---

ನಿಮ್ಮ ಪ್ರೋಗ್ರಾಮ್‌ನ್ನು ಪರೀಕ್ಷೆ ಮಾಡಿ, ಮತ್ತು ಸ್ಪ್ರೈಟ್‌ಗಳು ಸುತ್ತಲೂ ಚಲಿಸುವುದನ್ನು ಮುಗಿಸಿದಾಗ ಮಾತ್ರ ನೀವು ಅವುಗಳ ಮೇಲೆ ಕ್ಲಿಕ್‌ ಮಾಡಬಹುದು ಎನ್ನುವುದನ್ನು ನೀವು ನೋಡಬೇಕು.

--- /task ---

--- save ---
	




