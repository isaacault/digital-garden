---
title: My NeoVim Config
id: nvim-config
tags:
  - vim
  - neovim
  - config
  - dotfiles
published: true
layout: page
---

# My Perfect Neovim

<!--
## Preface

The most daunting thing about migrating to (neo)vim is having to configure it 
for your liking. Thankfully, there exists a plethora of pre-built configurations
available to be easily downloaded and get you going. For example, any of 
[LunarVim](https://www.lunarvim.org/), [LazyVim](https://www.lazyvim.org/), or 
[NvChad](https://nvchad.com/) are common examples that can be downloaded and 
installed in one step to achieve an IDE-like experience in the terminal using
Neovim. These 
-->

## Structure

```
$XDG_CONFIG_HOME/nvim
├── init.lua                     # The file which will load the rest.
├── lazy-lock.json               # Plugin manager versioning file. More later...
├── lua
│   └── isaacault
│       ├── config               # Local configurations.
│       │   ├── autocmds.lua
│       │   ├── init.lua
│       │   ├── remap.lua
│       │   └── set.lua
│       ├── lazy.lua             # Plugin manager.
│       └── plugins              # Plugins and their configurations.
│           ├── autopairs.lua
│           ├── colorscheme.lua
│           ├── harpoon.lua
│           ├── lsp.lua
│           ├── neogen.lua
│           ├── snippets.lua
│           ├── telescope.lua
│           ├── treesitter.lua
│           └── trouble.lua
└── README.md
```


## Plugin Manager

For my Neovim config I'm going to use the [lazy.nvim](https://lazy.folke.io/) 
plugin manager developed by the established and trustworthy 
[folke](https://github.com/folke).

<!--
## Plugins

A complete list of all my installed plugins, and what I use them for.

* [catpuccin](https://github.com/catppuccin/nvim)
* Configures Neovim to the desired catpuccin theme.

* [Harpoon](https://github.com/ThePrimeagen/harpoon/tree/harpoon2)
* Easily mark/unmark frequently used files for switching between.

* [Neogen](https://github.com/danymat/neogen)
* Generate snippets.

* [nvim-autopairs](https://github.com/windwp/nvim-autopairs)
* As named, provides auto-completion of pairs for common characters (quotes, 
        brackets, etc.).
* [!NOTE] I'm not actually sure if I want to keep this, I don't think I mind 
typing my own brackets and sometimes it gets it wrong.
-->
