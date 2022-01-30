# Ruby-Wordle

A set of ruby scripts to generate word-lists and solve Wordle

⬜️⬜️⬜️⬜️⬜️ \
⬜️⬜️⬜️🟨🟨 \
⬜️🟩⬜️🟩⬜️ \
🟩🟩⬜️🟩🟩 \
🟩🟩🟩🟩🟩

----

### Ruby Scripts

🟢 `script-solver.rb`

A solver script for Wordle

**Usage Example**

```plain-text
> ruby script-solver.rb

STEP 1) 🟩 Input letters and positions using alphabets and dots. Then press Enter
           [e.g. s...h]
        ＞ .r..e
STEP 2) 🟨 Input pairs of a position (starting from 1) and a letter. Then press Enter.
           [e.g. 1g 2e 5a]
        ＞ 3e 4e 4r
STEP 3) ⬛︎ Input letters not used in the word. Then Press Enter.
           [e.g. ieagh]
        ＞ hotlquypic
------------------------------------------------
arage, arake, arase, brake, brame, brave, braze, 
drake, drame, drave, erade, erase, frame, frase, 
fraze, grade, grame, grane, grave, graze
------------------------------------------------
```

🟢 `script-filter.rb`

A filter script to generate *n*-letter word lists (`word-list.txt` and `word-list-uniq.txt`)

The default *n* value is 5. Change `NUM_LETTERS` if necessary, and execute the following command in the same directory where the script is located. A directory will be created automatically with the title having the number specified in the script (e.g. `word-lists/5-letters`, `word-lists/6-letters`).

**Usage Example**

```
> ruby script-filter.rb
```
----

### Lists of English Words of 5 Letters (useful to solve Wordle)

🟢 `word-lists/5-letters/word-list.txt`

A list of five-letter words, generated using a ruby script and the original word list.

🟢 `word-lists/5-letters/word-list-uniq-letters.txt`

A list of five-letter words consisting of five different letters, generated using a script and the original word list.

----

### Original List of English Words

🟢 `word-lists/word-list-original.txt`

A word list used to generate more useful word lists above. It is based on `words_alpha.txt` in [dwyl/english-words](https://github.com/dwyl/english-words).

----

### Author

Yoichiro HASEBE

----

### License

MIT
