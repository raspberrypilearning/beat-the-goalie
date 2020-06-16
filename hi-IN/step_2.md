## फुटबॉल को हिलाना

चलिए गेंद को मंच के नीचे से ले जाने के लिए कोड करते हैं।

--- task ---

'बीट द गोअली' Scratch स्टार्टर प्रोजेक्ट खोलें।

**ऑनलाइन**: स्टार्टर प्रोजेक्ट को [rpf.io/beat-the-goalie-on](http://rpf.io/beat-the-goalie-on){: target="_blank"} पर खोलें।

यदि आपके पास एक Scratch खाता (account) है तो आप **Remix** पर क्लिक करके कॉपी बना सकते हैं |

**ऑफलाइन**: [स्टार्टर प्रोजेक्ट](http://rpf.io/p/en/beat-the-goalie-go){:target="_blank"} को ऑफलाइन एडिटर में खोलिये।

यदि आपको Scratch ऑफ़लाइन संपादक को डाउनलोड और इंस्टॉल करना है, तो आप इसे [rpf.io/scratchoff](http://rpf.io/scratchoff) {:target="_blank"} पर ढूंढ सकते हैं।

स्टार्टर प्रोजेक्ट में, आपको एक गोल बैकड्रॉप, एक फुटबॉल और गोलकीपर स्प्राइट दिखना चाहिए।

![स्टार्टर प्रोजेक्ट](images/goalie-starter.png)

--- /task ---

--- task ---

अपने फुटबॉल स्प्राइट पर क्लिक करें। इस कोड को जोड़ें, ताकि फ़ुटबॉल स्क्रीन के नीचे तब तक चले जब तक स्पेस बार दबाया न जाए।

![फुटबॉल स्प्राइट](images/football-sprite.png)

```blocks3
when green flag clicked
repeat until <key (space v) pressed?>
move (10) steps
if on edge, bounce
end
```

--- /task ---

--- task ---

अपने खेल का परीक्षण करने के लिए हरे झंडे पर क्लिक करें। जब भी स्पेस बार दबाया जाये तब आपकी फ़ुटबॉल स्क्रीन के नीचे उछलनी चाहिए।

![स्क्रीनशॉट](images/goalie-football-move-test.png)

--- /task ---

--- task ---

इस कोड को अपने फुटबॉल स्प्राइट में जोड़ें, ताकि स्पेस बार के दबाए जाने के बाद फुटबॉल गोल की ओर बढ़े।

![फुटबॉल स्प्राइट](images/football-sprite.png)

```blocks3
when green flag clicked
repeat until <key (space v) pressed?>
move (10) steps
if on edge, bounce
end
+ repeat (15)
change y by (10)
end
```

--- /task ---

--- task ---

अपने खेल का परीक्षण करने के लिए हरे झंडे पर क्लिक करें। इस बार, स्पेस बार दबाएं और आपका फुटबॉल लक्ष्य की ओर बढ़ना चाहिए।

![स्क्रीनशॉट](images/goalie-football-ypos-test.png)

--- /task ---

--- task ---

अपने खेल का परीक्षण करने के लिए हरे झंडे पर क्लिक करें। यदि आप दूसरी बार फ्लैग पर क्लिक करते हैं तो क्या होता है? क्या आप इस समस्या को ठीक कर सकते हैं?

--- hints ---

--- hint ---

जब `green flag पर क्लिक किया जाता है `{:class="block3events"} तब  स्प्राइट को ` से `{:class="block3motion"} वापिस स्टार्ट पॉइंट पे जाना चाहिए I

--- /hint ---

--- hint ---

आपको इन ब्लॉक्स की जरुरत होगी:

```blocks3
go to x:(-200) y:(-140)
```

--- /hint ---

--- hint ---

आपका कोड इस प्रकार दिखना चाहिए:

![फुटबॉल स्प्राइट](images/football-sprite.png)

```blocks3
when green flag clicked
+ go to x:(-200) y:(-140)
repeat until <key (space v) pressed?>
move (10) steps
if on edge, bounce
end
repeat (15)
change y by (10)
end
```

--- /hint ---

--- /hints ---

--- /task ---

