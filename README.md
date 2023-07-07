# `cyrillic.nvim`

## Description

This plugin will let you enter command mode (NORMAL) commands using Russian keyboard layout. Also it will let you enter few most used commands in command line mode in safe way (only full commands translated). This is usually enough to avoid switching between Russian and English layouts just to control Vim.

This plugin is a lua port of the [original Vimscript plugin](https://github.com/powerman/vim-plugin-ruscmd/tree/master) for Neovim.

Besides all it adds a support for [which-key.nvim](https://github.com/folke/which-key.nvim) (hides the Cyrillic mappings in it).

## Installation

- [Lazy.nvim](https://github.com/folke/lazy.nvim)
```lua
{
  'nativerv/cyrillic.nvim',
  event = { 'VeryLazy' },
  config = function()
    require('cyrillic').setup({
      no_cyrillic_abbrev = false, -- default
    })
  end,
}
```
