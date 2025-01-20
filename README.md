# My nvim config files
## About this repository
This is a backup of the old nvchad version that was used in the video https://www.youtube.com/watch?v=lsFoZIg-oDs 
Credits go out to Dreamsofcode entirely. 
## Dependencies

- https://github.com/neovim/neovim/blob/master/INSTALL.md
- git

## Installation instructions
In Ubuntu/Debian/MacOS run the following command 
``` bash
git clone https://github.com/ddoebel/nvim_config_files ~/.config/nvim && nvim
```
For c++ syntax highlighting run 
```
:TSInstall cpp
```
inside of neovim. 
## Heavily based on https://github.com/NvChad


### Hint: 
You might want to edit the file lua/custom/configs/nvim-dap.lua at line 6 to make it work with your adapter. 

## Remove the autoformatter
You might find the autoformatter anonying, in that case you might consider removing it. Here are the instructions for that:
go to 
```bash
nvim ~/.config/nvim/lua/custom/plugins.lua
```
Now search for the following code snippet by typing `/null-ls` + ENTER in normal mode. 
Remove or comment out (using `--`) the following snippet: 
```lua
{
  "jose-elias-alvarez/null-ls.nvim",
  event = "VeryLazy",
  opts = function()
    return require "custom.configs.null-ls"
  end,
},
```
Now quit and open neovim again, and you should be auto-formatter free. 

