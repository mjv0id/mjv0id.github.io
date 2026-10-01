---
title: "neovim cheatsheet"
date: 2026-09-30 23:52:00 -0300
categories: [study]
tags: [linux]
---

## modes

`i` insert before cursor
`I` insert at beginning
`a` insert after cursor
`A` insert at end
`o` new line below
`O` new line above
`v` visual (character)
`V` visual (line)
`ctrl + v` visual (block)
`:` command mode
`esc` return to normal
`R` replace mode

## navigation

```
  k  
h   l
  j
```

`w` next word
`b` previous word
`e` end of word
`0` line start
`$` line end
`gg / G` file start / end
`:{N}` go to line N
`%` go to matching bracket
`{ / }` prev / next blank line (paragraph)
`ctrl + d / ctrl + u` half page down/up
`ctrl + f / ctrl + b` full page down/up

## edit

`x` delete character 
`dd` delete line
`dw` delete word
`d$ / D` delete to end of line
`yy` yank (COPY) line
`yw` yank word
`p / P` paste after/before cursor
`u` undo
`ctrl + r` redo
`cc / C` change line / to end of line
`cw` change word
`r{char}` replace single character
`~` toggle case
`.` repeat last change

## search

`/pattern` search forward
`?pattern` search backward
`n / N` next / prev match
`*` search word under cursor (fwd)
`#` search word under cursor (bwd)
`s/old/new` replace first on line
`:s/old/new/g` replace all line
`%s/old/new/g` replace all in file
`:s/old/new/gc` replace with confirmation
`:noh` clear search highlight

## splits 

`:sp / :vsp` horizontal / vertical split -> `ctrl + w s / ctrl + w v`
`ctrl + w h/j/k/l` move between splits // i added custom keymaps for this one
`ctrl + w H/J/K/L` move split to edge
`ctrl + w =` equalize split sizes
`ctrl + w _ / |` increase / decrease height
`ctrl + w q` close split
`ctrl + w o` close all other splits

## tabs
`:tabnew` open new tab
`:tabnew {file}` open file in new tab
`gt / gT` next / prev tab
`:tabclose` close current tab
`:tabonly` close all other tabs
`{n}gT` go to tab N

## buffers

`:e {file}` edit file
`:w` save
`:w {file}` write a copy
`:w ++p` save creating parent dirs if needed
`:wq / :x` save and quit
`:q` quit
`q!` quit without saving
`wqa` save all and quit
`:ls / :buffers` list buffers
`:bn / :bp` next / prev buffer
`bd` delete (close) buffer
`b {N}` switch to buffer N
`ctrl + ^` toggle to last buffers
