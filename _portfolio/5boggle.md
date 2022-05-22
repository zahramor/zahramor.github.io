---
title: "Implementation of a Boggle game"
excerpt: "2016"
collection: portfolio
---

As a programming assignment on the last year of my Bachelor degree, we had to implement an [algorithm](https://github.com/anebz/Boggle) able to find words in a slightly-varied [Boggle game](http://www.ultraboardgames.com/boggle/game-rules.php). Given a grid of characters and a list of points per character, the algorithm had to find the words with the highest points (that is, the words containint characters which in turn were awarded with the most points), construct a hash for each, and match it with a given hash to find the *secret* word. 

The bottlenecks were predominantly iterating the grid, backtracking and dealing with incomplete words, and creating all possible lowercase-uppercase possibilities for each string. Making the algorithm run fast was essential. 

* A lexicon/dictionary was provided with around 100k words, as well as hash string
* These words were stored in a Trie
* Finding the words in the grid included implementing backtracking
* Additionally, the *secret word* could be composed of words in the grid + no more than one extra character not in the grid. So if the current string in the iteration was "hou", and the next possibility "e", the option of "house" should be considered, since there is one extra character between the strings "hou" and "e". This extra character could be located anywhere in the string (beginning, anywhere in the middle, or the end).
* Constructing the hash involved constructing the hash for each possibility of lowercase-uppercase character from the word. If the candidate word was "house", the hash for "House", "hOuse", "hoUse", ..., "HOUSE" should be calculated. 
* The initial requirement was that the whole project (reading the dictionary, storing it in a Trie, finding all words with the highest score and obtaining all the lowercase-uppercase possibilities) should take less than 1s. At around the middle of the project, my group presented a time of 0.12s. The professor then lowered the limit to 0.1s, and in the end my team was able to make the algorithm run in 0.08s. 

