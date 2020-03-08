Bandit Level 1
=====

###### Solver: ap3xsh0t

> https://overthewire.org/wargames/bandit/bandit1.html

> The password for the next level is stored in a file called readme located in the home directory. Use this password to log into bandit1 using SSH. Whenever you find a password for a level, use SSH (on port 2220) to log into that level and continue the game.

#### Solution:
Upon logging in with the previous level's flag, we see a file in the home directory titled "-". When using commandline tools such as cat, the "-" character may be interpreted as a flag, meaning cat won't actually cat the flag. Instead, we can specify that we would like to cat the flag by giving a relative path to the file.

> cat ./-

This gives us the flag (and password for the next level)

> CV1DtqXWVFXTvM2F0k09SHz0YwRINYA9
