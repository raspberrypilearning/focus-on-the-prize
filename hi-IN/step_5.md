## उत्तरों को दिखाएँ

इस चरण में, आप कोड जोड़ेंगे ताकि खिलाड़ी उपहार बॉक्स पर क्लिक करके देख सके कि उसके अंदर क्रिस्टल है या नहीं।

--- task ---

**Gift** स्प्राइट के कोड में, एक कोड जोड़ें ताकि `when this sprite clicked`{:class="block3events"} क्लिक करे, तो यह `says`{:class="block3looks"} `Yes!` और `switches costume to`{:class="block3looks"} क्रिस्टल में बदल देते हैं।

![गिफ्ट स्प्राइट की छवि](images/gift-sprite.png)

```blocks3
when this sprite clicked
say [Yes!]
switch costume to [Crystal-a v]
```

--- /task ---

--- task ---

**Gift2** स्प्राइट पर क्लिक करें और ब्लॉक जोड़ें ताकि यह `says`{:class="block3looks"} `No!`. `say`{:class="block3looks"} ब्लॉक के मान को `1` सेकंड में बदलें। एक `hide`{:class="block3looks"} ब्लॉक जोड़ें ताकि स्प्राइट गायब हो जाए।

![गिफ्ट2 स्प्राइट की छवि](images/gift2-sprite.png)

```blocks3
when this sprite clicked
say [No!] for (1) seconds
hide
```

--- /task ---

--- task ---

चूंकि **Gift2** स्प्राइट को अब छिपाया जा सकता है, आपको `show`{:class="block3looks"} ब्लॉक जोड़ना होगा यह सुनिश्चित करने के लिए कि यह प्रोग्राम शुरू होने पर वह दिखाई दे रहा है।

![गिफ्ट2 स्प्राइट की छवि](images/gift2-sprite.png)

```blocks3
when green flag clicked
go to x: (0) y: (0)
+ show
```

--- /task ---

--- task ---

अपना कोड चलाने के लिए हरे झंडे पर क्लिक करें, और परीक्षण करें कि जब आप बक्से पर क्लिक करते हैं तो क्या होता है।

--- /task ---

आप देख सकते हैं कि जब बॉक्स घूम रहे हों तो आप उन पर क्लिक कर सकते हैं। खिलाड़ियों को इस तरह से धोखा देने से रोकने के लिए `variable`{:class="block3variables"} का उपयोग कर सकते हैं।

--- no-print ---

![एनिमेटेड जीआईएफ दिखा रहा है कि गिफ्ट हिलना बंद करने पहले क्लिक किए जा रहे हैं](images/cheat.gif)_

--- /no-print ---

--- task ---

एक नया `variable`{:class="block3variables"} बनाएं, जिसे `finished`कहा जाता है। `set`{:class="block3variables"} में ब्लॉक जोड़ें `finished`{:class="block3variables"} वेरिएबल को `false` में जब गिफ्ट हिलना शुरू करते हैं, और फिर `true` जब गिफ्ट हिलना बंद हो कर देते

![गिफ्ट स्प्राइट की छवि](images/gift-sprite.png)

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

अब, आप `if … then`{:class="block3control"} ब्लॉक का उपयोग यह जांचने के लिए कर सकते हैं कि `finished`{:class="block3variables"} सही है या गलत। `Operators`{:class="block3operators"} ब्लॉक जोड़ें ताकि क्लिक का कोई प्रभाव तभी पड़े जब `finsihed`{:class="block3variables"} `=`{:class="block3operators"} `true` हो।

![गिफ्ट स्प्राइट की छवि](images/gift-sprite.png)

```blocks3
when this sprite clicked
+ if <(finished) = [true]> then
say [Yes!]
switch costume to [Crystal-a]
```

--- /task ---

--- task ---

उसी `if`{:class="block3control"} कंडीशन को **Gift2** स्प्राइट में जोड़ें।

![गिफ्ट2 स्प्राइट की छवि](images/gift2-sprite.png)

```blocks3
when this sprite clicked
+ if <(finished) = [true]> then
say [No!] for (1) seconds
hide
```

--- /task ---

--- task ---

अपने प्रोग्राम का परीक्षण करें, और आपको यह देखना चाहिए कि आप स्प्राइट्स पर तभी क्लिक कर सकते हैं जब वे घूमना बंद कर लें।

--- /task ---

--- save ---
	




