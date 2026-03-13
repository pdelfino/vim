# vim

![The Great Wave off Kanagawa](./painting.jpg)

*"The Great Wave off Kanagawa" (c. 1831) by Katsushika Hokusai — [Wikipedia](https://en.wikipedia.org/wiki/The_Great_Wave_off_Kanagawa)*

**Personal Vim configuration with Vundle, Molokai, and Portuguese spell checking.**

## About

A lightweight Vim setup used alongside a primary Emacs workflow. This config focuses on sensible defaults -- line numbers, proper indentation, matching delimiters -- with a few plugins managed through [Vundle](https://github.com/VundleVim/Vundle.vim).

## What's Inside

- **Vundle** for plugin management
- **Molokai** color scheme
- **SuperTab** for tab-based completion
- **vim-fugitive** for Git integration
- **WakaTime** for coding activity tracking
- **Portuguese spell checking** support (`pt_BR`)
- Clean indentation defaults: 4-space tabs, smart indent, expand tabs

## Installation

```shell
# Clone
git clone git@github.com:pdelfino/vim.git ~/projects/vim

# Symlink vimrc
ln -sf ~/projects/vim/vimrc ~/.vimrc

# Symlink colors
ln -sf ~/projects/vim/colors ~/.vim/colors

# Install Vundle
git clone https://github.com/VundleVim/Vundle.vim.git ~/.vim/bundle/Vundle.vim

# Install plugins from within Vim
vim +PluginInstall +qall
```

### SuperTab Setup

1. Open `supertab.vmb` in Vim: `vim supertab.vmb`
2. Source the file: `:so %`

### Portuguese Spell Checking

The `vero_pt_br_v208aoc.oxt` file provides Brazilian Portuguese spell checking. For setup instructions, see [this guide](https://www.vivaolinux.com.br/artigo/Corretor-Ortografico-no-Vim-Guia-definitivo).

## Quick Reference

A few commands worth remembering (from `tips.md`):

| Command                  | Action                                    |
|--------------------------|-------------------------------------------|
| Visual select + `U`      | Convert selection to uppercase            |
| `:%s/old/new/g`          | Substitute all occurrences in the file    |
| `:%s/pattern//gn`        | Count matches of a pattern                |
