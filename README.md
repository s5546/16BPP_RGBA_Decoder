# 4BPP_RGBA_Decoder
Created for PicoCTF 2019. Decodes 4-char hex groups into RGBA images. 
Was not the answer to the problem, but like... its fun.

also i named the python file the wrong thing, it does RGBA decryption not ARBG decryption


Input files should be formatted in 4 character Hex pairs, like this:
```
ABCD 0241 BAB0 D00D BEEE EEEF 0033 1123
ABAD FAAD 0023 134D A42B 0032 1542 4382
3321 2343 0A3D 
```
etc...
You should probably have all columns be the same width, but I haven't really tested if that actually breaks things- they SHOULD be filled in with a default RGBA value of (0,0,0,0), but truthfully I have no clue if that'll actually happen for any row aside from the last one.

FFFF

|||\\____________Alpha, aka transparency- higher means more opaque

||\\_______Green

|\\____Blue

\\__Red
