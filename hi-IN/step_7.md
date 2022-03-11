## ध्यान भटकाने के लिए कुछ बनाएँ

खेल खत्म करने के लिए, कुछ ध्यान भटकाने वाला जोड़ सकते हैं, ताकि खिलाड़ी गिफ्ट बॉक्स पर अपनी नजर नही रख पाए।

--- task ---

अपने खेल में एक नया स्प्राइट जोड़ें। आप अपनी पसंद का कोई भी स्प्राइट चुन सकते हैं, लेकिन इस उदाहरण में, हम **Duck** स्प्राइट का उपयोग करेंगे।

![duck स्प्राइट की छवि](images/duck-sprite.png)

--- /task ---

जब खेल शुरू होता है, तो बत्तख को छिपा दिया जाना चाहिए, और बक्सों के हिलने के बाद ही उसे चलना शुरू करना चाहिए। बत्तख को सामने की परत पर लाना भी उपयोगी होता है, ताकि वह बक्सों के ऊपर चले जाए।

--- task ---

निम्नलिखित ब्लॉकों को **Duck** स्प्राइट में जोड़ें।

![duck स्प्राइट की छवि](images/duck-sprite.png)

```blocks3
when flag clicked
hide
go to [front v] layer
wait (4) seconds
```

--- /task ---

--- task ---

इसके बाद, **Duck** Sprite को `wait`{:class="block3control"} एक `random`{:class="block3operators"} सेकंड की संख्या, फिर पूरे Stage पर`glide`{:class="block3motion"}  होना चाहिए और `hide`{:class="block3looks"} होना चाहिए. यह तब तक हो सकता है जब तक कि खेल समाप्त न हो जाए।

![duck स्प्राइट की छवि](images/duck-sprite.png)

```blocks3
when flag clicked
hide
go to [front v] layer
wait (4) seconds
+ repeat until <(finished) = [true]>
wait (pick random (1) to (5)) seconds
go to x: (-280) y: (-140)
show
glide (2) secs to x: (280) y: (140)
hide
```
--- /task ---

--- task ---

अपने खेल का परीक्षण करें और देखें कि क्या जब ध्यान भटकाने वाली बत्तख Stage पर उड़ रही होती है तब क्या आप गिफ्ट बॉक्स का ट्रैक रख सकते हैं या नहीं।

--- /task ---

--- save ---

