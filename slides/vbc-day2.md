%title: Vim Bootcamp - Day 2
%author: Brandon Schrader
%date 2018-03-16

-> # Into the details <-

-> *You're problem with Vim is you don't grok Vi* <-

^
* _Day 2 Topics:_
    ^
    - motions
    ^
    - registers (delete/\yank/\put)
    ^
    - substitutions

---

-> # Motions <-

Learning the Language of Vim

Talk to Vim in *verb, modifier, object* sentences
^

|   *verb*   | *modifier* |  *object* |
|----------|----------|---------|
| *c* change | *i* inside | *w* word  |
| *d* delete | *a* around | *"* quote |
| *y* yank   | *t* till   | *(* paren |
| *v* visual | *f* find   | *t* tag   |

^
* _Verb Object_
    - *dw* delete word
    ^
    - *cw* change word
    ^
    - *ct[c]* change to character
    ^
    - problems with verb object or verb modifier
    ^

* _Verb Modifier Object_
    - *diw* delete inside word
    ^
    - *daw* delete around word (word + 1 space)
    ^
    - *ciw* change inside word
    ^
    - *ci"* change inside quote
    ^

Aim for repeatability so you can use *.*

---

-> # Registers <-

Cut *delete*, Copy *yank* and Paste *put* the Vim way

^
register    *:registers*
verbs       *y* *yy* yank selection or line
            *d* *dd* delete selection or line
            *p* *"[#]* put from default register or specific register

^
- yank a sentence and paste it, notice difference between *p* and *P*
^
- yank a word and paste it

^
*:registers* checkout registers
^
- try out a non default register

^
- delete a line and paste
^
- be-careful not to clobber your register

---

-> # Substitutions <-

The find and replace of vim

^
*:s/[find]/[replace]* replace first instance in line
^
*:s/[find]/[replace]/g* replace all instances in line
^
*:[range]s/[find]/[replace]/g* replace all instances in range
^
*:%s/[find]/[replace]/g* replace all instances in file

---

-> # End of Day 2 <-

More resources

blog    [Your Problem with Vim is you dont grok Vi](http://stackoverflow.com/questions/1218390/what-is-your-most-productive-shortcut-with-vim/1220118#1220118)

video   [Vim from novice to professional](http://derekwyatt.org/vim/tutorials/novice/)
