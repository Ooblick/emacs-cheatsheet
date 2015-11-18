# Emacs Cheatsheet

## Definition of bindings

`M-` represents pressing the _meta_ key, followed by a keystroke.

`C-` represents pressing the _ctrl_ key, followed by a keystroke.

In iTerm2, I have the following keys bound:

`Left option key acts as: Normal`
`Right option key acts as: +Esc`

## Movement

Key      | Meaning              | Key     | Meaning
---------|----------------------|---------|--------
`C-n`    | Next line            |         |
`C-p`    | Previous line        |         |
`C-f`    | Forward 1 char       |`M-f`    | Forward 1 word
`C-b`    | Back 1 char          |`M-b`    | Back 1 word
`C-a`    | Go to start of line  |`M-a`    | Go to start of sentence
`C-e`    | Go to end of line    |`M-e`    | Go to end of sentence
`C-v`    | Scroll page down     |`M-v`    | Scroll page up
`C-a RET`| Insert line above    |`C-e RET`| Insert line below

### Notes:
1. in order for single-space sentences to work, set this in `.emacs`: `(setq sentence-end-double-space nil)`.

## Mangling
Key       | Meaning                  | Key     | Meaning
----------|--------------------------|---------|--------
`C-k`     | DEL rest of line         |`C-ak`   | DEL line
`C-x DEL` | DEL to start of sentence |`M-k`    | DEL to end of sentence
`M-d`     | DEL next word            |`M-DEL`  | DEL previous word
`M-z CHR` | DEL to next occurring CHR|         |
