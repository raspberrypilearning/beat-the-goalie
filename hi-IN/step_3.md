## क्या यह एक गोल था?

एक बार जब गेंद गोल तक पहुँच गई, तो बनाने का निर्णय है। __if__ गेंद गोलकीपर को छू रही है फिर उसे बचा लिया गया है, __else__ यह एक गोल है।

--- task ---

इस कोड को अपने फुटबॉल स्प्राइट कोड के अंत में जोड़ें, ताकि आप जांच सकें कि गेंद गोलकीपर को छू रही है या नहीं।

![फुटबॉल स्प्राइट](images/football-sprite.png)

```blocks3
repeat (15)
change y by (10)
end
+if <touching (goalie v)> then
else
end
```

--- /task ---

--- task ---

`Start the 'rattle' sound`{:class="block3sound"} `अगर गोलकीपर गेंद को बचाया है`{:class="block3control"}.

![फुटबॉल स्प्राइट](images/football-sprite.png)

```blocks3
if <touching (goalie v)> then
+start sound (rattle v)
else
end
```

--- /task ---

--- task ---

आप गोलकीपर को एक संदेश भी प्रसारित कर सकते हैं, ताकि वे आपको बता सकें कि गेंद बच गई है।

जब गेंद सेव हो गई हो तो एक 'सेव' संदेश प्रसारित करें।

![फुटबॉल स्प्राइट](images/football-sprite.png)

```blocks3
if <touching (goalie v)> then
start sound (rattle v)
+broadcast (save v)
else
end
```

--- /task ---

--- task ---

अब आप अपने गोलकीपर को 'सेव!' कहने के लिए कोड कर सकते हैं। जब वे संदेश प्राप्त करते हैं।

![गोलकीपर स्प्राइट ](images/goalie-sprite.png)

```blocks3
when I receive [save v]
say [Save!] for (1) seconds
```

--- /task ---

--- task ---

एक गोल करने की कोशिश करके अपने कोड का परीक्षण करें। यदि आपका गोलकीपर गोल बचाता है, तो उन्हें 'सेव!' कहना चाहिए।

![स्क्रीनशॉट](images/goalie-save-test.png)

--- /task ---
