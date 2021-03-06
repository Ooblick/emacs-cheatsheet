# Emacs Cheatsheet

## Definition of bindings

`M-` represents pressing the _meta_ key, followed by a keystroke.
`C-` represents pressing the _ctrl_ key, followed by a keystroke.

When either command should be released before entering another keystroke, this is represented by a space, e.g.:

`C-x z` -- which means "press & hold `ctrl`, then press `x`, then release `ctrl` and press `z`. When there's no space, keep `ctrl` held.

### iTerm2 Setup for OSX
In iTerm2, I have the following keys bound:

`Left option key acts as: Normal`
`Right option key acts as: +Esc`

# Emacs Binds

## Movement
Key      | Meaning              | Key     | Meaning
---------|----------------------|---------|--------
`C-n`    | Next line            |`M-gg`   | GOTO line num
`C-p`    | Previous line        |         |
`C-f`    | Forward 1 char       |`M-f`    | Forward 1 word
`C-b`    | Back 1 char          |`M-b`    | Back 1 word
`C-a`    | Go to start of line  |`M-a`    | Go to start of sentence
`C-e`    | Go to end of line    |`M-e`    | Go to end of sentence
`C-v`    | Scroll page down     |`M-v`    | Scroll page up
`C-a RET`| Insert line above    |`C-e RET`| Insert line below

## Selection (copy, paste, kill)
Key       | Meaning                  | Key     | Meaning
----------|--------------------------|---------|--------
`C-SPC`   | Start visual             |`M-w`    | Copy (save to kill ring)
`C-w`     | Kill selection           |`C-y`    | Paste (yank)
`C-ed`    | Join lines below         |         |
`C-x z`   |

## Searching
Key        | Meaning                  | Key     | Meaning
-----------|--------------------------|---------|--------
`C-s`      | Search forward as-typing |`C-s`    | Backwards search
`C-M-s`    | Begin regexp search      |`C-M-r`  | Backwards regexp search
`M-b C-sws`| Search for word under csr|         |

## Replacing
Key        | Meaning                  | Key     | Meaning
-----------|--------------------------|---------|--------
`M-%`      | Begin search replace     |         |
`SPC`      | Replace & goto next      |`.`      |Skip result, goto next
`!`        | Replace all              |`^`      |Go back to prev replace loc

## Mangling
Key       | Meaning                  | Key     | Meaning
----------|--------------------------|---------|--------
`C-t`     | Transpose two chars      |`M-t`    | Transpose two words
`C-xt`    | Transpose two lines      |`M-c`    | Make first letter UC
`M-u`     | Uppercase rest of word   |`M-l`    | Lowercase rest of word
`C-k`     | DEL rest of line         |`C-ak`   | DEL line
`C-x DEL` | DEL to start of sentence |`M-k`    | DEL to end of sentence
`M-d`     | DEL next word            |`M-DEL`  | DEL previous word
`M-z CHR` | DEL to next occurring CHR|`C-SPC`  | DEL leading spaces

## Markers
Key       | Meaning                  | Key     | Meaning
----------|--------------------------|---------|--------
`C-SPCSPC`|Set mark, do not activate | C-uSPC  | GOTO marker

## Window Management
Key       | Meaning                  | Key     | Meaning
----------|--------------------------|---------|--------
`C-xk`    | Kill buffer              |`C-ak`   | DEL line
`C-x2`    | Split buf vertical       |`C-x3`   | Split buf horizontal
`C-x0`    | Close current buffer     |         |



### Notes:
#### Movement
1. in order for single-space sentences to work, set this in `.emacs`: `(setq sentence-end-double-space nil)`.
