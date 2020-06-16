--- challenge ---

## चुनौती: मैनुअल कंट्रोल

गेंद के बाएं और दाएं घूमने के बजाय, क्या आप अपने खिलाड़ी को `a` और `d` बटन के साथ गेंद को नियंत्रित करने की अनुमति दे सकते हैं ?

ऐसा करने के लिए आपको बाएं और दाएं गेंद को स्थानांतरित करने के लिए कोड को हटाना होगा।

```blocks3
when green flag clicked
forever
    go to x:(-200) y:(-140)
    repeat until <key (space v) pressed?>
-       move (10) steps
-       if on edge, bounce
    end
    repeat (15)
        change y by (10)
    end
    if <touching (goalie v)> then
        start sound (rattle v)
        broadcast (save v)
    else
        start sound (cheer v)
        broadcast (goal v)
    end
end
```

जब आप बटन दबाते हैं तो आप गेंद को हिलाने के लिए कोड जोड़ सकते हैं। आपकी मदद करने के लिए यहां कुछ कोड ब्लॉक दिए गए हैं:

```blocks3
change x by (-5)

if <> then 
end

<key (a v) pressed>
```

--- /challenge ---
