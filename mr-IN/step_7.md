## विकर्षण तयार करा

गेम पूर्ण करण्यासाठी, तुम्ही प्लेयरला भेटवस्तू बॉक्सवर नजर ठेवून थांबवण्याचा प्रयत्न करण्यासाठी, एक विकर्षण जोडू शकता.

--- task ---

तुमच्या गेमला नवीन स्प्राईट जोडा. तुम्हाला आवडणारा कोणताही स्प्राईट तुम्ही निवडू शकता, परंतु या उदाहरणात, आम्ही **Duck** स्प्राईट वापरू.

![duck स्प्राईटची इमेज](images/duck-sprite.png)

--- /task ---

गेम चालू झाल्यावर, बदक लपायला हवे, आणि तो बॉक्सने हलणे चालू केल्यावरच केवळ हलणे चालू करायला हवे. बदकांना पुढच्या थरावर आणणे देखील उपयुक्त आहे, जेणेकरून ते बॉक्सच्या वरच्या बाजूस फिरतील.

--- task ---

**Duck** स्प्राईटला खालील ब्लॉक्स जोडा.

![duck स्प्राईटची इमेज](images/duck-sprite.png)

```blocks3
when flag clicked
hide
go to [front v] layer
wait (4) seconds
```

--- /task ---

--- task ---

पुढे, **Duck** स्प्राईटने `wait`{:class="block3control"}  करायला हवी `random`{:class="block3operators"} सेकंद संख्येची, त्यानंतर स्टेज भोवती `glide`{:class="block3motion"} करायला हवे आणि `hide`{:class="block3looks"} हवे. गेम संपेपर्यंत हे घडत राहू शकते.

![duck स्प्राईटची इमेज](images/duck-sprite.png)

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

तुमच्या गेमची चाचणी घ्या आणि Stage वर उडणाऱ्या विकर्षीत करणार्‍या बदकासह तुम्ही भेटवस्तू बॉक्सचा मागोवा ठेवू शकता का ते पहा.

--- /task ---

--- save ---

