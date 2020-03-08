Bandit Level 0
=====

###### Solver: ap3xsh0t

> https://overthewire.org/wargames/bandit/bandit0.html

>The goal of this level is for you to log into the game using SSH. The host to which you need to connect is bandit.labs.overthewire.org, on port 2220. The username is bandit0 and the password is bandit0. Once logged in, go to the Level 1 page to find out how to beat Level 1.

#### Solution:
This level is pretty basic. It wants the player to ssh to bandit.labs.overthewire.org on port 2220 with the username of bandit0 and password of bandit0

> ssh bandit0@bandit.labs.overthewire.org -p 2220

Once logged in, there is a readme in the home directory. Cat this to recover the password for the next level.

> boJ9jbbUNNfktd78OOpsqOltutMc3MY1
