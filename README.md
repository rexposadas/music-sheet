# Why this project? 

I could not find an easy and free way to find music in different keys. This is a collection of music sheets in ABCjs, PDF and musicXML format.

I also could not an easy way to transpose music. This repository contains instructions on how to do that. 
 

# Tools used

- [ABCjs editor](https://michaeleskin.com/abctools/abctools.html) main notation tool
- [Musescore](https://musescore.org/en) for converting score from treble clef to alto clef
- [abc2xml](https://wim.vree.org/svgParse/abc2xml.html) converts *.abc (ABCjs file) to xml. The resulting XML file is imported in Musescore.

# ABCjs Cheat Sheet

Header Keys: 
T - Title
M - Meter
R - Rhythm ( optional )
K - Key (after this line comes the notes)
L - Default note length 
    L: 1/4 - default note length is quarter note
    L: 1/8 - default note length is eight note


C> - Key of C staccato

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

# Files 

The files in the directory has different version of the song. 

```text
*.abc - These are the ABCjs notations
*.xml - Converted abc notation to xml using abc2xml tool
*.musicxml - Exported musicxml file from Musescore app
*_original_score.pdf - Some songs have these which files used to transcribe the ABCjs notations. 
This is sometimes needed because the song was not in a hymnal.
*_alto_clef.pdf - PDF transposed for alto instruments such as Violas. This is done using Musescore.
*in_<key>.pdf - transposed to a different key i.e. _in_e.pdf - For convenience, so that the transposed file has been generated. 
*_bass.abc - notation with only bass clef
```
