---
title: Doom Emacs
slug: doom-emacs
type: article
publish_date: 2021-04-03 10:00
---

# Doom Emacs

Please note! This is a living document and will be updated whenever needed.

Trying Emacs once again, this time around not a custom setup but [DOOM Emacs](https://github.com/hlissner/doom-emacs)

While learning I also keep this cheat sheet open: [DOOM cheat sheet](https://gist.github.com/hjertnes/9e14416e8962ff5f03c6b9871945b165)

## Reasoning

### Reasons for DOOM Emacs

- Fully setup for plugins
- Nice GUI setup from the get go
- A nice default key map to start with `SPC h b b` for a quick lookup on key
  bindings
- Nice starter theme to get going
- Sane default plugins
- Some kind of standard for initialization and configuration (not invented by
  me)

### Reasons why I want to use Emacs

- Strong markdown support
- Distraction free writing
- Magit (GIT client)
- ORG Mode for notes
- Possible replacement for Visual Code

## Learning Goals

In order for me to be comfortable enough to use Emacs the list below should at
least be as easy to use as in other editors. For me that means, following a
standard I've grown accustomed to. If
this means I need to re-map keybindings I should be able to do so with minimum
effort.

- [X] Opening and closing files [^](#open-and-closing-files)
- [ ] Quickly go to previous / next open files
- [X] Tabs [^](#tabs)
- [ ] nice list with open files
- [ ] and "action" tool, in PHPStorm I can use `CTRL - SHIFT - A` to open
      actions and access everything I need
- [ ] Having a folder as "project" and being able to switch to these
- [ ] Splitting files or have multiple files open next to each other

## Shortcuts

### Opening and closing files

I try to stay as close to DOOM as possible and only remap when inconvenient.

| Shortcut   | Does                       |
| :--------- | :------------------------- |
| SPC .      | Open a file (global)       |
| SPC SPC    | Open a file (in project)   |
| SPC b k    | Kill a buffer              |

### Splitting views

| Shortcut | Does                                                           |
|:---------|:---------------------------------------------------------------|
| SPC w V  | vertical split (and follow). This is what I'm used to.         |
| SPC w S  | horizontal split (and follow). Again this is what I'm used to. |

### Opening files in split view

I have enabled Treemacs, and from Treemacs this is  easy.

| Shortcut | Does                      |
|:---------|:--------------------------|
| SPC o p  | Open Treemacs             |
| SPC o s  | Open and split Horizontal |
| SPC o v  | Open and split Vertical   |

## Tabs

In order to have a nice tab bar, all I needed to do was open the `init.el` and
enable `tabs`

So in Emacs:

```shell
ESC (go into command mode) -> SPC f p (open configuration file) -> init.el
```

And remove `;;` from tabs

Now do a `doom sync` and restart Emacs.
