--- challenge ---

## التحدي: التحكم اليدوي

بدلاً من تحريك الكرة يمينًا ويسارًا تلقائيًا، هل يمكنك السماح الاعب بالتحكم في الكرة باستخدام مفاتيح `a` و `d`؟

للقيام بذلك، ستحتاج إلى إزالة الكود البرمجي لتحريك الكرة إلى اليسار وإلى اليمين.

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
    if <touching (حارس المرمى v)> then
        start sound (rattle v)
        broadcast (رد الكرة v)
    else
        start sound (cheer v)
        broadcast (رد الهدف v)
    end
end
```

يمكنك بعد ذلك إضافة الكود البرمجي لتحريك الكرة عند الضغط على المفاتيح. هنا التعليمات البرمجية التي ستحتاج اليها:

```blocks3
change x by (-5)

if <> then 
end

<key (a v) pressed>
```

--- /challenge ---
