Bandit Level 2
=====

###### Solver: ap3xsh0t

> https://overthewire.org/wargames/bandit/bandit3.html

> The password for the next level is stored in a file called spaces in this filename located in the home directory


#### Solution:
After SSHing into this level we see a file which contains spaces in the file name. In order to print the contents to the screen we must escape the spaces with "\". Tab completition also can help us here.

> cat spaces\ in\ this\ filename

> UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK
