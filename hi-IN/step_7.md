## गोलकीपर को नियंत्रित करें

एक गोल करना बहुत आसान है! आइए एक दूसरे खिलाड़ी को लक्ष्य बनाने और बचाने की अनुमति दें।

--- task ---

अपने __ Goalie  __ sprite पर क्लिक करें , दिए गए कोड को जोड़े और गोलकीपर की जगह बादलने के लिए गोलकीपर की x पोज़िशन को दायें और बायें तीर को दबा कर बदलें I

![गोलकीपर स्प्राइट ](images/goalie-sprite.png)

```blocks3
when [left arrow v] key pressed
change x by (-10)
```

--- /task ---

--- task ---

अपने नए कोड का परीक्षण करने के लिए बायाँ तीर दबाएँ। अपने गोलकीपर को बाईं ओर जाना चाहिए।

![स्क्रीनशॉट](images/goalie-move-left-test.png)

--- /task ---

--- task ---

जब दायां तीर कुंजी दबाया जाता है __ Goalie __ दाईं ओर जाएं `  ` {: class = "block3events"}, इसके लिए  ऊपर के समान (similar) दिए ब्लॉक का उपयोग करें I

--- hints ---

--- hint ---

अपने कोड में ब्लॉक जोड़ें ताकि ` जब दायां तीर कुंजी दबाया जाए ` {= class = "block3events"}, __ Goalie __ ` x स्थिति 10 से बदल जाये ` {: class = "block3motion"}।

--- /hint ---

--- hint ---

आपको इन ब्लॉकों की जरुरत होगी:

```blocks3
change x by (10)

when [right arrow v] key pressed
```

--- /hint ---

--- hint ---

आपका कोड इस प्रकार दिखना चाहिए:

![गोलकीपर स्प्राइट ](images/goalie-sprite.png)

```blocks3
when [right arrow v] key pressed
change x by (10)
```

--- /hint ---

--- /hints ---

--- /task ---
