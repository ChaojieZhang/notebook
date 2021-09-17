# vim skill

## escape key too far away? try combine control and [

```
^[
```

## motion

most single motion could prepend a number to repeating number times

| action           | desc                               |
| ---------------- | ---------------------------------- |
| [number][motion] | execute number times of motion     |
| h j k l          | move around                        |
| gg               | move to first line                 |
| [number]gg       | move to line                       |
| G                | move to last line                  |
| %                | move to pared character like {} [] |
| f[character]     | move to character                  |
| F[character]     | move to character                  |
| w                | move to next word head             |
| e                | move to next word end              |
| b                | move to word head                  |
| 0                | move to line head                  |
| $                | move to line end                   |

## edit

| action         | desc                                 |
| -------------- | ------------------------------------ |
| [motion][edit] | apply edit to moved throw characters |
| x              | cut character                        |
| y              | copy character                       |
| yy             | copy line                            |
| dd             | delete line                          |
| r[character]   | replace character                    |
| ~              | switch case                          |
| gU[motion]     | to Upper case                        |
| gu[motion]     | to lower case                        |
| u              | undo                                 |
| ^r             | redo                                 |
| ==             | format code                          |

## switch mode

| action                  | desc                                        |
| ----------------------- | ------------------------------------------- |
| I                       | move to line head and switch to insert mode |
| A                       | move to line end and switch to insert mode  |
| v[motion][edit]         |                                             |
| v[motion]I[modify][esc] | multi line edit                             |

## command

| command             | desc                      |
| ------------------- | ------------------------- |
| :set no[option]     | unset option              |
| :set number         | show lien number          |
| :set relativenumber | show relative line number |
