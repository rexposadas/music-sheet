# music-sheet
music sheets in text format


Go to editor: 

https://michaeleskin.com/abctools/abctools.html


# Cheat Sheet

Header Keys: 
T - Title
M - Meter
R - Rhythm ( optional )
K - Key (after this line comes the notes)


C> - Key of C stacatto

^C - set key as sharp

-- Example of multiple staves.

This will display two staves, one in treble clef and one in bass clef.

```abc
K: C
V:1 clef=treble
V:2 clef=bass
[V:1] C E G c | d B G F |
[V:2] C, E, G, C | F, G, A, B, |
```

To put more space between measures
%%vskip 2cm

# To transpose

1. Go to : https://michaeleskin.com/abctools/abctools.html
2. Copy and paste the text, that will display the score
3. Use the "Transpose" button