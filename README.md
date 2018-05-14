# cipher
A web-based ASCII XOR cipher

This small web app written in Python encrypts and decrypts a string by converting characters to their ASCII binary representations and performing an exclusive or (XOR) operation with the key string.

```
String to encrypt: hello
My secret key string: jon (could be of any length)

"h": "1101000",
"e": "1100101",
"l": "1101100",
"l": "1101100",
"o": "1101111"

"j":"1101010",
"o":"1101111",
"n":"1101110"

XOR Truth Table
Inputs   Output
1 1      0
1 0      1 
0 1      1
0 0      0

h       e       l       l       o
1101000 1100101 1101100 1101100 1101111
j       o       n       j       o
1101010 1101111 1101110 1101010 1101111
XOR output
0000010 0001010 0000010 0000110 0000000
```
And that's our encrypted string: `00000100001010000001000001100000000`. Just remember the key to decrypt it by performing XOR again.
