# The Vim way

This is SOME text
This is SOME text
This is SOME text
This is SOME text
This is SOME text
This is SOME text
This is SOME text
This is SOME text
This is SOME text
This is SOME text
This is SOME text



## Launching vim

```bash
vim -u NONE -N
# -u do not source .vimrc, and vim starts as vi, disabling many features
# -N set nocompatable to prevent vim from starting as vi


:h feature-list # to view feature list
:version        # to view vim version
:h gui          # view gui related options (more syntax highlighting and fonts)
:h .


u               # undo the last change
.               # repeat the last change(cmd) (could be char/word/line/file), replay last keystroke
dd              # delete current line
dd . . .        # delete current line and repeat last change (so simple)...
>G              # increase the indentation from current line to end of file
<G
:%s/content/copy/g  # replace content as copy for all lines
*               # search the word under cursor
cw              # delete curren word and put into insert mode
* cwreplace<Esc> n.n.n.n.n. # replace one by one of current word as replace
```

## Learning stuff

* Vim tutor
* Vim SOME


## Tips

* Meet the Dot Command
* Don't Repeat Yourself

## 

* <C-n> to show auto-complete word lis


## Pasting

* `.` command, dot command, - repeat last command


## Searching

* `*` searchs for the word under the current cursor
* 


## Plugin

* markdown
* lua
* complate
* 