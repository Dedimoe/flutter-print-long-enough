# flutter-print-long-enough
Flutter print long enough for logging

```
void printLongEnough(String text) {
    //supaya bisa print ke console log tanpa terpotong dan bisa panjang
    final pstr = RegExp('.{1,800}'); // 800 dipotong setiap 800 character
    pstr.allMatches(text).forEach((match) => print(match.group(0)));
}
```

usage:
```
   //<your code> 
   printLongEnough('very-very long string here');
}
```

just it.
