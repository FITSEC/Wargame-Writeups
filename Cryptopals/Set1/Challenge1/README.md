Convert hex to base64
=====

#### The string:
49276d206b696c6c696e6720796f757220627261696e206c696b65206120706f69736f6e6f7573206d757368726f6f6d

#### Should produce:
SSdtIGtpbGxpbmcgeW91ciBicmFpbiBsaWtlIGEgcG9pc29ub3VzIG11c2hyb29t


#### Methodology:
The first thing we need to do is make sure that we take the hex string above and create raw bytes instead. I placed the hex string into a text document to be read in with python. Then I made this very ugly one-liner that decodes the hex string into bytes and THEN base64 encodes it before printing the result.

``` python
import base64

with open('hex.txt', 'rb') as fd:
	line = fd.readlines()
	print base64.b64encode(line[0].strip().decode('hex'))
```
