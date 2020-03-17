Bandit Level 2
=====

###### Solver: ap3xsh0t

> https://overthewire.org/wargames/bandit/bandit4.html

> The password for the next level is stored in a hidden file in the inhere directory.

#### Solution:
After SSHing into this level, ls shows a directory. Cd into this directory and ls -la to view all (even hidden) files. You can see there is a file called .hidden.

> cat .hidden

> pIwrPrtPN36QITSp3EQaw936yaFoFgAB
