Bandit Level 0
=====

###### Solver: ap3xsh0t

> https://overthewire.org/wargames/bandit/bandit1.html

> The password for the next level is stored in a file called readme located in the home directory. Use this password to log into bandit1 using SSH. Whenever you find a password for a level, use SSH (on port 2220) to log into that level and continue the game.

#### Solution:
This level is pretty basic. It wants the player to ssh to bandit.labs.overthewire.org on port 2220 with the username of bandit0 and password of bandit0

> ssh bandit0@bandit.labs.overthewire.org -p 2220

Once logged in, there is a readme in the home directory. Cat this to recover the password for the next level.

> boJ9jbbUNNfktd78OOpsqOltutMc3MY1
