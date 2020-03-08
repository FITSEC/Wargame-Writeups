Fixed XOR
=====

> https://cryptopals.com/sets/1/challenges/2

###### Solver: ap3xsh0t

##### The string:
1c0111001f010100061a024b53535009181c

##### The XOR key:
686974207468652062756c6c277320657965

##### Should produce:
746865206b696420646f6e277420706c6179

##### Methodology:
First thing I did was create a file to contain the hex values (this is uneccessary but purely habit at this point for me). I read in the values and decoded them. Next, I created a loop that would iterate over all values in the key and string (since they are the same length). I created a list to append the xor operation to and after compleing the xor operation, joined and encoded the result as hex before printing.


``` python
with open('hex.txt', 'rb') as fd:
        lines = fd.readlines()
        val = lines[0].strip().decode('hex')
        key = "686974207468652062756c6c277320657965".strip().decode('hex')

        flag = []
        for x in range(0, len(key)):
                flag.append(chr(ord(val[x]) ^ ord(key[x])))

        print "".join(flag).encode('hex')

```
