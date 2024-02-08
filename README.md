# hoon-runes.vim

Vim help file for Hoon Runes in disguise of a plugin.

## Installation

Using [vim-plug](https://github.com/junegunn/vim-plug):
```
Plug 'matthiasschaub/hoon-runes.vim', { 'branch': 'main' }
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

The content is based on the [docs.urbit.org repository](https://github.com/urbit/docs.urbit.org).
The only changes made to the content has been the removal of markdown links and reformatting of custom From/Syntax tables.
The syntax has been changed from markdown to Vim helptext (Vimdoc) with [`decipher`](https://github.com/matthiasschaub/decipher).

See also [hoon-stdlib.vim](https://github.com/matthiasschaub/hoon-stdlib.vim).

Reach out to `~talfus-laddus` on Urbit for anything related to this plugin.

## Vimdoc / Vim helpfile Resources

- Essay about Vimdoc: https://github.com/nanotee/vimdoc-notes
- Cheatsheet about helpfiles: https://devhints.io/vim-help
- A linter: https://github.com/machakann/vim-vimhelplint
- And of course: `:help help-writing`
