# hoon-runes.vim

Vim help file for Hoon Runes in disguise of a plugin.

## Installation

Using [vim-plug](https://github.com/junegunn/vim-plug):
```
Plug 'https://git.sr.ht/~talfus-laddus/hoon-runes.vim'
```

## Usage

Run the help command with the Rune:
```
:help $=
```
Or run the help command with the pronounceable name of the Rune:
```
:help buctis
```

<img src="https://minio.mutualisten.de/talfus-laddus/hoon-runes.vim/demo.gif" alt="drawing" width="600"/>

## Limitation

All runes containing `*` or `|` can not be *help tags* because those symbols (tar and
bar) are used to define *tags* and *link to tags* in Vimdoc. For example `:help |=` will
not work. Use `help buctis` instead.

## About

The content is based on the [developers.urbit.org repository](https://github.com/urbit/developers.urbit.org/tree/main/content/reference/hoon/rune).
The only changes made to the content has been the removal of markdown links and reformatting of custom From/Syntax tables.
The syntax has been changed from markdown to Vim helptext (Vimdoc) using
[`decipher`](https://git.sr.ht/~talfus-laddus/decipher) tool on the Markdown source files.

Reach out to `~talfus-laddus` on Urbit for anything related to this plugin.

## Vimdoc / Vim helpfile Resources

- Essay about Vimdoc: https://github.com/nanotee/vimdoc-notes
- Cheatsheet about helpfiles: https://devhints.io/vim-help
- A linter: https://github.com/machakann/vim-vimhelplint
- And of course: `:help help-writing`
