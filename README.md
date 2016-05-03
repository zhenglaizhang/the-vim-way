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


v{motion}d|y    # cut or copy selection
P               # paste before the cursor



u               # undo the last change
Ctrl+r          # redo
.               # repeat the last change(cmd) (could be char/word/line/file), replay last keystroke
dd              # delete current line
dd . . .        # delete current line and repeat last change (so simple)...
>G              # increase the indentation from current line to end of file
<G
/search         # search for 'search', N->previous, n->forward
:%s/content/copy/g  # replace content as copy for all lines
*               # search the word under cursor
cw              # delete curren word and put into insert mode
cW
c3w             # change the 3 words
* cwreplace<Esc> n.n.n.n.n. # replace one by one of current word as replace
b               # back to word's beginning
w               # forward to next word's beginning
db              # delete backward
dw              # delete forward
daw             # delete current word
dap             # delete a paragraph
dG              # delete from current line to end of file
b dw            # move to beginning of word and delete forward
d2w | 2dw | dw. # delete 2 words
uu | 2u         # undo twice

g~              # swap cases
gu              # make lower case
gU              # make upper case


<               # shift left
>               # shift right
=               # auto indent

guap
gUaw
gul
gUl


:14             # jump to line 14
:$              # jump to end of file
:print | :p     # print current line
:15p            # move cursor to line 15 and echo that line

:7d             # more to line 7 then delete that line
7G dd           # move to line 7 then delete that line
:2,5p           # print line 2 to 5


# . means current line
:.,$p           # print current line to end of file

# % means all lines in current file
:%p             # print all lines in current file 
:1,$p


:%s/old/new     # replace first occurence of 'old' with 'new' in each line


# virtual selection then :
:'<,'>p
# '< means first line of most recent selection
# '> means last line of most recent selection


# Ex commands can accept regex as address
:/<html>/,/<\/html>/p
:/start_pattern/,/end_pattern/{cmd}

# address could be modified with offset
:/commands/+1,/motion/-2p
:.,.+3p




# read content from file and paste here
:read file
:read !ls

# switch to location of last edit
g
```

    c{motion}
    y{motion}
    d{motion}

## Learning stuff

* Vim tutor
* Vim SOME
* Vim Golf score


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