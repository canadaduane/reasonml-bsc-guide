# Setting Up Your Editor

ReasonML is a new syntax, but it has great support for several editors thanks to [Merlin](https://github.com/the-lambda-church/merlin).

To install Merlin, run:
```
opam install merlin
```

See [Getting Started](getting-started.md) for more info about `opam`.

## Sublime Text 3

The [Sublime Text Merlin](https://github.com/cynddl/sublime-text-merlin) plugin for Sublime Text 3 supports OCaml syntax.

**Installation:**

- in Sublime Text, press Cmd+Shift+P
- type in "Install" which should bring up the "Package Control: Install Package" option (NOTE: you need to have [Package Control](https://packagecontrol.io/installation) installed)
- type "Merlin" to install the sublime-text-merlin package

There is a [sublime-reason](https://github.com/facebook/reason/tree/master/editorSupport/sublime-reason) plugin for Sublime Text 3. (Is it necessary to install the Merlin plugin at all?)

## Atom

The Atom editor supports Reason syntax, see the [Installation Instructions](http://facebook.github.io/reason/tools.html#merlin-atom) on the Tools page of the Reason home page.

See also https://github.com/the-lambda-church/merlin/wiki/atom-from-scratch and https://ocaml.io/w/Reason#Merlin

## Visual Studio Code

[OCaml Support](https://marketplace.visualstudio.com/items?itemName=hackwaly.ocaml) supports OCaml syntax. (How to set it for Reason syntax?)

## Vim

Merlin has built-in support for Vim. You can enable it for Reason by installing the [VimReason](https://github.com/facebook/reason/tree/master/editorSupport/VimReason) plugin for Vim.

## Emacs

Merlin has built-in support for Emacs. There is a [reason-mode](https://github.com/facebook/reason/tree/master/editorSupport/emacs) available as a plugin.
