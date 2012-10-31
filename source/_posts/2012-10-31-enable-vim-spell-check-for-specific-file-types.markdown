---
layout: post
title: "Enable Vim Spell Check For Specific File Types"
date: 2012-10-31 11:02
comments: true
categories: VIM
---

You can enable spell check in vim, gvim, or macvim by entering *command mode[^1]* and typing `:set spell`.

To make this permanent for every time you open a file in vim you can add this line to your `~/.vimrc`[^2] file:

``` vim
set spell
```

If you use vim for programming you might not want it to spell check every file.  If, for example, you use vim to edit your markdown files for your [Octopress Blog](http://octopress.org) AND you also use vim to edit your ruby project you will want to use the autocmd instead:

``` vim
autocmd FileType Markdown setlocal spell
```

This will only enable spell check if you open a file with type "Markdown"

---
[^1]: You can enter *command mode* by pressing the `ESC` key.
[^2]: `~` represents the current users home directory.  Similar to the `$HOME` environment variable.

