# Neovim Seth Phaeno Setup Guide

- nvim configuration goes in `.config/nvim`

- He created directory `after` that he said he would talk about later: `mkdir .config/nvim/after`

- He created the file `init.lua`: `touch init.lua` 

- He also created a directory called `lua`: `mkdir .config/nvim/lua`

- He then created a directory called `Sethy`: `mkdir .config/nvim/lua/Terry` in my case. Not necessary he says but I'll see what I think. 

- Then a directory for settings and keybindings: `mkdir .config/nvim/lua/Terry/core`

- Inside core he pressed the `%` sign to create a file and named it `options.lua` and saved it as an empty file 

- `:Ex` to get back to the file tree. And `%` to create `keymaps.lua` also saved as an empty file

- `d` to create a directory in the file explorer and `%` to create a file (He'll change that later)

- Back to the `init.lua` file and `require("Terry.core")`   - Bunch of errors because required directories have to have an `init.lua` file

  ``` lua title=".config/nvim/lua/Terry/core/init.lua"
  require("Terry.core.options")
  require("Terry.core.keymaps")
  ```

- Now some options in `options.lua`

  ``` lua title="options.lua"
  vim.cmd("let g:netrw_banner = 0")
  
  vim.opt.guicursor = ""
  vim.opt.nu = true
  vim opt.relativenumber = true
  
  vim.opt.tabstop = 4
  vim.opt.softtabstop = 4
  vim.opt.shiftwidth = 4
  vim.opt.expandtab = true
  vim.opt.autoindent = true
  vim.opt.smartindent = true
  vim.opt.wrap = false
  
  vim.opt.swapfile = false
  vim.opt.backup = false
  vim.opt.undofile = true
  
  
  ```

  