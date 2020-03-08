Single-byte XOR cipher
=====

> https://cryptopals.com/sets/1/challenges/3

###### Solver: ap3xsh0t

##### Hex string:
1b37373331363f78151b7f2b783431333d78397828372d363c78373e783a393b3736

##### Methodology:
Instead of XORing equal length hex strings like last challenge, now we need to brute force the key. There are letter frequency attacks and all that jazz, but this should be easy enough to brute force with python. I created a list of letters and then iterated over each letter. For each letter, we iterate over each byte in the hex string and print the results of the XOR operation between the two. I used sys.stdout.write this time so that I can print each character individually without injecting whitespace or newline charactars that python's print keyword creates when used.

Yes, I know. My python is very "c" like. I learned to program in c/c++. Sue me.

``` python
import sys

with open('hex.txt', 'rb') as fd:
        lines = fd.readlines()
        val = lines[0].strip().decode('hex')
        letters = "a b c d e f g h i j k l m n o p q r s t u v w x y z A B C D E F G H I J K L M N O P Q R S T U V W X Y Z"
        letterList = letters.split()

        for letter in letterList:
                sys.stdout.write("Letter: " + letter + " Plain text: ")
                for char in val:
                        sys.stdout.write(chr(ord(char) ^ ord(letter)))
                print "\n"

```
