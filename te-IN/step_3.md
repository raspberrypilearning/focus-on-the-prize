## బహుమతి పెట్టెను తరలించండి

ఇప్పుడు మీరు దానిలో గిఫ్ట్ తో కూడిన బాక్సును కలిగి ఉన్నందున, మీరు దానిని స్క్రీన్ చుట్టూ కదిలేలా చేయాలి.

--- task ---

మొదటి, `go to x: y:`{:class="block3motion"} బ్లాక్ ను ఉపయోగించి గిఫ్ట్ కు Stage మీద ఎడమ వైపు ప్రారంభ స్థానం ఇవ్వండి.

![gift sprite యొక్క చిత్రం](images/gift-sprite.png)

```blocks3
when flag clicked
+ go to x: (-150) y: (0)
switch costume to [gift-a v]
wait (1) seconds
switch costume to [Crystal-a v]
wait (2) seconds
switch costume to [gift-a v]
```

--- /task ---

**Broadcasts** కొన్ని లేదా అన్ని ఇతర sprite లు స్వీకరించడానికి ఒక sprite ద్వారా పంపబడే సందేశాలు.

మీ ప్రోగ్రామ్‌లోని ఈవెంట్‌లు అన్నీ ఏక కాలంలో పూర్తవడానికి broadcasts ఉపయోగపడతాయి.

`Events`{:class="block3events"} బ్లాక్‌ల మెనులో, `broadcast message1 and wait`{:class="block3events"} బ్లాక్‌ని సెలెక్ట్ చేయండి.

--- task ---

తరలించడం ప్రారంభించడానికి కొత్త `broadcast`{:class="block3events"} ని సృష్టించండి. మీ కొత్త broadcast ని `move` అని పిలవండి.

![పేరు ఎంపికలు విస్తరించిన broadcast బ్లాక్‌ని చూపుతున్న చిత్రం](images/broadcastAndWait.png)

!["move" పేరుతో టైప్ చేసిన కొత్త broadcast ని సృష్టించడానికి డైలాగ్ బాక్స్‌ను చూపుతున్న చిత్రం](images/new-message.png)

--- /task ---

--- task ---

`wait`{:class="block3control"} బ్లాక్‌ను జోడించి, ఆపై `broadcast move and wait`{:class="block3events"} బ్లాక్‌ని జోడించండి.

![gift sprite యొక్క చిత్రం](images/gift-sprite.png)

```blocks3
when flag clicked
go to x: (-150) y: (0)
switch costume to [gift-a v]
wait (1) seconds
switch costume to [Crystal-a v]
wait (2) seconds
switch costume to [gift-a v]
+ wait (1) seconds
+ broadcast [move v] and wait
```

--- /task ---

--- task ---

Sprite, `move`{:class="block3events"} broadcast ని `receives`{:class="block3events"} చేసినప్పుడు sprite విభిన్న దిశలలో, `glide`{:class="block3motion"} అవడం ప్రారంభమవుతుంది. దీనిని `10` సార్లు పునరావృతం చేయడానికి, `repeat`{:class="block3control"} బ్లాక్‌ని ఉపయోగించవచ్చు.

![gift sprite యొక్క చిత్రం](images/gift-sprite.png)

```blocks3
when I receive [move v]
repeat (10)
glide (1) secs to [random position v]
```

--- /task ---

--- task ---

ఆకుపచ్చ జెండాపై క్లిక్ చేసి, costume మారిన తర్వాత మీ sprite యాదృచ్ఛికంగా కదలడం ప్రారంభిస్తుందో లేదో తనిఖీ చేయండి.

--- no-print ---

![యానిమేట్ gif గిఫ్ట్, స్క్రీన్ చుట్టూ యాదృచ్ఛికంగా కదులుతున్నట్లు చూపుతుంది](images/random-motion.gif)

--- /no-print ---

--- /task ---

--- save ---


