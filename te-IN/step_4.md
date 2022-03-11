## ఖాళీ బాక్సుని సృష్టించండి

ఈ దశలో, మీరు మరొక గిఫ్ట్ బాక్సును జోడిస్తారు, కానీ ఇది ఖాళీగా ఉంటుంది! ఇది యాదృచ్ఛిక దిశలలో కూడా కదులుతుంది.

--- task ---

రెండవ **gift** spriteను జోడించండి. దీనికి స్వయంచాలకంగా **gift 2** అని పేరు పెట్టబడుతుంది.

![రెండు gift sprite లను పక్కపక్కనే చూపుతున్న చిత్రాలు](images/two-gifts.png)

దీని పరిమాణాన్ని `150` (శాతం) కి పెంచాలని గుర్తు పెట్టుకోండి.

--- /task ---

--- task ---

Stage మధ్యలో ప్రారంభించేలా **gift 2** spriteని సెట్ చేయండి.

![gift2 sprite యొక్క చిత్రం](images/gift2-sprite.png)

```blocks3
when green flag clicked
go to x: (0) y: (0)
```

--- /task ---

--- task ---

బ్లాక్‌లను జోడించండి, తద్వారా ఈ sprite `receives move`{:class="block3events"}, అది విభిన్న దిశలలో, `glide`{:class="block3motion"} అవడం ప్రారంభమవుతుంది.

![gift2 sprite యొక్క చిత్రం](images/gift2-sprite.png)

```blocks3
when I receive [move v]
repeat (10)
glide (1) secs to [random position v]
```

--- /task ---

--- task ---

ఆకుపచ్చ జెండాపై క్లిక్ చేసి, రెండు sprite లు Stage చుట్టూ కదలడాన్ని చూడండి.

--- no-print ---

![రెండు గిఫ్ట్ బాక్స్‌ల యానిమేటెడ్ gif స్క్రీన్ చుట్టూ యాదృచ్ఛికంగా కదులుతుంది](images/random-motion-2.gif)

--- /no-print ---

--- /task ---

బాక్సులు ఎల్లప్పుడూ ఒకదానికొకటి అదే వేగంతో కదలాలి. ప్రస్తుతానికి, అవి `glide 1 secs`{:class="block3motion"} కి సెట్ చేయబడ్డాయి. రెండు బాక్సుల వేగాన్ని సులభంగా మార్చడానికి, మీరు `variable`{:class="block3variables"}ని ఉపయోగించవచ్చు.

--- task ---

`speed`అని పిలువబడే కొత్త `variable`{:class="block3variables"}ని సృష్టించండి మరియు దానిని `glide 1 secs to random position`{:class="block3motion"} బ్లాక్‌కి జోడించండి. ఈ బ్లాక్‌ని **Gift** మరియు **Gift2** sprite లకు జోడించండి.

![gift sprite యొక్క చిత్రం](images/gift-gift2-sprite.png)

```blocks3
when I receive [move v]
repeat (10)
+ glide (speed) secs to [random position v]
```

--- /task ---

--- task ---

**Gift** sprite చెందిన కోడ్ లో, వేరియబుల్ యొక్క `speed`{:class="block3variables"} `set`{:class="block3variables"} చేయడానికి కోడ్‌ని జోడించవచ్చు. మీకు నచ్చిన ఏదైనా విలువను ఎంచుకోండి.

![gift sprite యొక్క చిత్రం](images/gift-sprite.png)

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

మీకు నచ్చిన వేగాన్ని కనుగొనే వరకు విభిన్న విలువలతో ప్రయోగం చేయండి.

--- /task ---

--- save ---




